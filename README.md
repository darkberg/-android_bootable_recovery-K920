# K920_recovery

Lenovo VIBE Z2 Pro(K920) recovery

打开文件：device/lenovo/kingdom_row.mk 
添加以下代码。
========================================
#TWRP
TW_THEME := portrait_hdpi
RECOVERY_GRAPHICS_USE_LINELENGTH := true
TW_NO_USB_STORAGE := true
TW_INCLUDE_CRYPTO := true
BOARD_SUPPRESS_SECURE_ERASE := true
RECOVERY_SDCARD_ON_DATA := true
BOARD_HAS_NO_REAL_SDCARD := true
TW_SCREEN_BLANK_ON_BOOT := true
BOARD_HAS_NO_SELECT_BUTTON := true
TARGET_RECOVERY_PIXEL_FORMAT := "RGBX_8888"
TW_EXTRA_LANGUAGES := true
TW_DEFAULT_LANGUAGE := zh_CN

#Recovery
TARGET_RECOVERY_FSTAB := device/lenovo/kingdom_row/rootdir/etc/fstab.qcom

=========================================
