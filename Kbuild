#
# focaltech_ft8756_spi_ts.ko
#
# Kbuild: for kernel building external module
#
# Note:
# - Please refer to modules/sample/Kbuild to find out what should be
#   done is this Kbuild file
#

#
# Source List
#

KO_MODULE_NAME := focaltech_ft8756_spi_ts
KO_MODULE_PATH := $(src)
KO_MODULE_SRC  :=

KO_MODULE_SRC += $(wildcard $(KO_MODULE_PATH)/*.c)

#
# Build Options
#
ccflags-y += -DDEBUG

#
# Final Objects
#
obj-m := $(KO_MODULE_NAME).o
# Comment it if the only object file has the same name with module
$(KO_MODULE_NAME)-y := $(patsubst $(src)/%.c,%.o,$(KO_MODULE_SRC))
