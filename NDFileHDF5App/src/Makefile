TOP=../..

include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE
#=============================

#==================================================
# build a support library

-include $(ADCORE)/ADApp/commonDriverMakefile
USR_CXXFLAGS_Linux += -DH5Gopen_vers=2

LIBRARY_IOC = NDFileHDF5_Batch

DBD += NDFileHDF5_Batch.dbd

LIB_SRCS += NDFileHDF5_Batch.cpp
LIB_SRCS += NDFileHDF5Dataset.cpp
LIB_SRCS += NDFileHDF5AttributeDataset.cpp
LIB_SRCS += NDFileHDF5LayoutXML.cpp
LIB_SRCS += NDFileHDF5Layout.cpp

NDFileHDF5_Batch_SRCS += NDPluginFile_Batch.cpp
NDFileHDF5_Batch_LIBS += $(EPICS_BASE_IOC_LIBS)

#===========================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE
