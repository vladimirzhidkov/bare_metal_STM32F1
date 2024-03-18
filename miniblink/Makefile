PROJECT = miniblink
BUILD_DIR = bin
SOURCE_DIR = src
OPENOCD_CONGIF_DIR = ../openocd-config
OPENCM3_DIR=../libopencm3

#SHARED_DIR = ../my-common-code
CFILES := $(addprefix $(SOURCE_DIR)/, main.c)
#CFILES += api.c
#AFILES += api-asm.S

# TODO - you will need to edit these two lines!
DEVICE=stm32f103c8t6
# OOCD_FILE = $(OPENOCD_CONGIF_DIR)/stm32f1x.cfg

start: all
flash: $(PROJECT).bin
	st-flash write $< 0x8000000

# You shouldn't have to edit anything below here.
VPATH += $(SHARED_DIR)
INCLUDES += $(patsubst %,-I%, . $(SHARED_DIR))

include $(OPENCM3_DIR)/mk/genlink-config.mk
include ../rules.mk
include $(OPENCM3_DIR)/mk/genlink-rules.mk
