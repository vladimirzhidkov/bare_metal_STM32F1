DEVICE=stm32f103c8t6
PROJECT = miniblink
OPENCM3_DIR=../libopencm3
CFILES := $(addprefix src/, main.c)

# You shouldn't have to edit anything below here.
VPATH += $(SHARED_DIR)
INCLUDES += $(patsubst %,-I%, . $(SHARED_DIR))

include $(OPENCM3_DIR)/mk/genlink-config.mk
include ../rules.mk
include $(OPENCM3_DIR)/mk/genlink-rules.mk
