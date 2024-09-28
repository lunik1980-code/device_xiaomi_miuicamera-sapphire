# MIUICamera For Sapphire

Prebuilt stock MIUI Camera for the Redmi Note 13 4G (sapphire/sapphiren), for included in custom ROM builds.

Extracted from the HyperOS.

## How to Use

### 1. Clone the Device MIUICamera Repo

```bash
git clone https://github.com/sm6225-unified/device_xiaomi_miuicamera-sapphire.git -b 14 device/xiaomi/miuicamera-sapphire
```

### 2. Clone the Vendor MIUICamera Repo

```bash
git clone https://gitlab.com/kibria5/vendor_xiaomi_miuicamera-sapphire.git -b 14 vendor/xiaomi/miuicamera-sapphire
```

### 3. Inherit from `BoardConfig.mk` in the Device Tree

```
# Inherit from proprietary files for MIUICamera
-include device/xiaomi/miuicamera-sapphire/BoardConfig.mk
```

### 4. Inherit from `device.mk` in the Device Tree

```
# Call the MIUICamera setup
$(call inherit-product-if-exists, device/xiaomi/miuicamera-sapphire/device.mk)
```

Enjoy!
