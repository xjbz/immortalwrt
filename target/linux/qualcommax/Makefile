include $(TOPDIR)/rules.mk

ARCH:=aarch64
BOARD:=qualcommax
BOARDNAME:=Qualcomm Atheros 802.11ax WiSoC-s
FEATURES:=squashfs ramdisk fpu nand rtc emmc
KERNELNAME:=Image
CPU_TYPE:=cortex-a53
SUBTARGETS:=ipq807x ipq60xx ipq50xx

KERNEL_PATCHVER:=6.12

include $(INCLUDE_DIR)/target.mk
# REMOVED FOR AX1800: automount, e2fsprogs, f2fs-tools, losetup, kmod-fs-ext4, kmod-fs-f2fs, kmod-usb3, kmod-usb-dwc3, kmod-usb-dwc3-qcom 
# REMOVED HERE TO LET .config CONTROL: luci, wpad-openssl
# REMOVED HERE TO LET .config CONTROL: kmod-nss-ifb, kmod-qca-nss-drv-bridge-mgr, kmod-qca-nss-drv-eogremgr, kmod-qca-nss-drv-gre, kmod-qca-nss-drv-igs, kmod-qca-nss-drv-l2tpv2, kmod-qca-nss-drv-lag-mgr, kmod-qca-nss-drv-map-t, kmod-qca-nss-drv-match, kmod-qca-nss-drv-mirror, kmod-qca-nss-drv-netlink, kmod-qca-nss-drv-pppoe, kmod-qca-nss-drv-pptp, kmod-qca-nss-drv-qdisc, kmod-qca-nss-drv-tun6rd, kmod-qca-nss-drv-tunipip6, kmod-qca-nss-drv-vlan-mgr, kmod-qca-nss-drv-vxlanmgr, kmod-qca-nss-drv-wifi-meshmgr
DEFAULT_PACKAGES += \
	autocore cpufreq uboot-envtools \
	kmod-ath11k kmod-ath11k-ahb kmod-ath11k-pci kmod-dsa kmod-dsa-qca8k kmod-phy-aquantia kmod-phy-qca83xx \
	kmod-gpio-button-hotplug kmod-leds-gpio kmod-leds-pwm \
	kmod-qca-nss-dp \
	kmod-qca-nss-ecm \
	kmod-qca-nss-drv \

$(eval $(call BuildTarget))
