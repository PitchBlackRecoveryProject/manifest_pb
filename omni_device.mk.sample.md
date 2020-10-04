<a href="README.md" >Go Back</a>

### omni_device.mk sample

```bash
# Inherit from those products. Most specific first.
$(call inherit-product, $(SRC_TARGET_DIR)/product/core_64_bit.mk) -- only for 64bit phones

# Inherit from device
$(call inherit-product, device/<path>/device.mk) -- path to main device makefile

# Inherit common product files.
$(call inherit-product, vendor/pb/config/common.mk)

# Set those variables here to overwrite the inherited values.
BOARD_VENDOR := 
PRODUCT_BRAND := 
PRODUCT_DEVICE := 
PRODUCT_NAME := omni_device
PRODUCT_MANUFACTURER := 
PRODUCT_MODEL := 
TARGET_VENDOR := 
```