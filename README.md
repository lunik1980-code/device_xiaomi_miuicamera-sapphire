<h1>⚠️WARNING⚠️</h1>
The original author made this repository private. This is the latest open version of the repository. This is actually a fork. Original autor: <a href="https://github.com/kibria5">Mohammad Kibria</a>

---

<h1>⚠️License extension⚠️</h1>
It is prohibited to include components of this repository in closed projects, as well as build firmware without publishing the source code of the trees.
Also, not only the authorship of the repository author should be mentioned, but also the original author

---

# MIUICamera For Sapphire

Prebuilt stock MIUI Camera for the Redmi Note 13 4G (sapphire/sapphiren), for included in custom ROM builds.

Extracted from the HyperOS.

## How to Use

### 1. Clone the Device MIUICamera Repo

```bash
git clone https://github.com/ReStranger/device_xiaomi_miuicamera-sapphire.git -b 14.0 device/xiaomi/miuicamera-sapphire
```

### 2. Clone the Vendor MIUICamera Repo

```bash
git clone https://gitlab.com/ReStranger/vendor_xiaomi_miuicamera-sapphire.git -b 14.0 vendor/xiaomi/miuicamera-sapphire
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
