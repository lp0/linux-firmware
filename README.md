# Source of origin

The GPHY firmware files in this tree are derived from header files in
the Lantiq linux-2.6.32 source tree distributed with Lantiq UGW-5.x.

Referenced files in Lantiq UGW-5.x:

* UGW-5.2-SW-CD/Software/Sources/UGW-5.2/target/linux/ltqcpe/files/include/switch_api/gphy_fw_[fe|ge].h
* UGW-5.3-SW-CD/Software/Sources/UGW-5.3/target/linux/ltqcpe/files-2.6.32/include/switch_api/gphy_fw_[fe|ge].h
* UGW-5.4-SW-CD/Software/Sources/UGW-5.4/target/linux/ltqcpe/files-2.6.32/include/switch_api/gphy_fw_[fe|ge].h

A System Vendor is obliged to publish his GPL sources, thus various
Lantiq UGW based kernel sources from different vendors can be found
in the Internet. Therefore these GPHY firmware files and the reference
headers can be treated as publicly available and are published in this
tree for convenience.

# How to use

Configure kernel with:
CONFIG_FW_LOADER=y
CONFIG_EXTRA_FIRMWARE_DIR="FIRMWARE_DIR"
CONFIG_EXTRA_FIRMWARE="FIRMWARE_FILES"

where FIRMWARE_DIR should point to this git tree and FIRMWARE_FILES is a list
of space separated files from list below.

# Firmware files

## GPHY core on Lantiq XWAY VR9 v1.1
lantiq/vr9_phy11g_a1x.bin
lantiq/vr9_phy22f_a1x.bin

## GPHY core on Lantiq XWAY VR9 v1.2
lantiq/vr9_phy11g_a2x.bin
lantiq/vr9_phy22f_a2x.bin
