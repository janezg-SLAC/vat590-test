IOC_TOP=/reg/g/pcds/epics/ioc/common/ads-ioc/R0.5.0
IOC_INSTANCE_PATH := $(shell pwd)

# Set PRODUCTION_IOC to 1 to move from a testing to a production IOC:
PRODUCTION_IOC := 0

PROJECT_NAME := vat590-test
PROJECT_PATH := ../../vat590-test/vat590-test.tsproj
PLC := plc_vat_test

PYTMC_OPTS := 
PREFIX := PLC:$(PLC)

# With two $$, as in $$(IOC) below, this will be expanded in the
# environment of st.cmd:
DB_PARAMETERS := 'PREFIX=$(PREFIX):,IOCNAME=$$(IOC),IOC=$$(IOC)'

include $(IOC_TOP)/iocBoot/templates/Makefile.base
