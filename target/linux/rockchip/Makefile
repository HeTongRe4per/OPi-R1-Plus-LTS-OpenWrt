# SPDX-License-Identifier: GPL-2.0-only

include $(TOPDIR)/rules.mk

BOARD:=rockchip
BOARDNAME:=Rockchip
FEATURES:=audio usb usbgadget display gpio fpu rootfs-part boot-part squashfs
SUBTARGETS:=armv8 armv8spi

KERNEL_PATCHVER=5.4

define Target/Description
	Build firmware image for Rockchip SoC devices.
endef

include $(INCLUDE_DIR)/target.mk

DEFAULT_PACKAGES += uboot-envtools partx-utils e2fsprogs mkf2fs kmod-gpio-button-hotplug

KERNELNAME:=Image dtbs

$(eval $(call BuildTarget))
