
# Use USERINCLUDE when you must reference the UAPI directories only.
USERINCLUDE     += \
                -I$(srctree)/techpack/audio/include/uapi \

# Use LINUXINCLUDE when you must reference the include/ directory.
# Needed to be compatible with the O= option
LINUXINCLUDE    += \
                -I$(srctree)/techpack/audio/include/uapi \
                -I$(srctree)/techpack/audio/include/elliptic \
                -I$(srctree)/techpack/audio/include
		
ifeq ($(CONFIG_ARCH_SM8150), y)
LINUXINCLUDE    += \
	-include $(srctree)/techpack/audio/config/tfa9894autoconf.h
endif


obj-y += soc/
obj-y += dsp/
obj-y += ipc/
obj-y += asoc/
