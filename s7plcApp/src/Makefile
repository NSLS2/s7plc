TOP=../..
include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE

LIBRARY_IOC = s7plc

s7plc_SRCS += drvS7plc.c
s7plc_SRCS += devS7plc.c

# API for the IOC
INC = drvS7plc.h

# formerly internal API exposed for non-IOC
# servers (like the CA-Gateway)
INC += compat3_13.h

s7plc_DBD += base.dbd
s7plc_DBD += calc.dbd
s7plc_DBD += s7plcBase.dbd
s7plc_DBD += s7plcCalcout.dbd
s7plc_DBD += s7plcReg.dbd
DBD += s7plc.dbd

s7plc_LIBS += calc
s7plc_LIBS += $(EPICS_BASE_IOC_LIBS)

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE
