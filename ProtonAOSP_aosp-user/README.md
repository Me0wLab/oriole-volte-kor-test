# ProtonAOSP (aosp-oriole-user)

## Download
[Download](https://github.com/Me0wLab/oriole-volte-kor-test/releases/tag/ProtonAOSP_aosp-user_v1)

## Patch Method
Add
```
# Force VOLTE
persist.dbg.volte_avail_ovr=1
```
at src/device/google/raviole/device-oriole.mk

## Status
- [x] Initial Build
>>> VOLTE Provisioning enabled.

>>> Cannot see VOLTE Toggle on Settings App

>>> Cannot enable VOLTE

## TODO
- [ ] Adding more Properties | [Reference](https://github.com/edgd1er/voenabler/blob/master/system.prop)
## How to Flash
Before flashing, Make sure that your bootloader is `unlocked`.
1. `fastboot flash boot $PATH/boot.img`
2. `fastboot flash dtbo $PATH/dtbo.img`
3. `fastboot flash vendor_boot $PATH/vendor_boot.img`
4. `fastboot flash --disable-verity --disable-verification vbmeta $PATH/vbmeta.img`
5. `fastboot reboot fastboot`
`fastboot flash system $PATH/system.img`
6. `fastboot flash system_ext $PATH/system_ext.img`
7. `fastboot flash product $PATH/product.img`
8. `fastboot flash vendor $PATH/vendor.img`
9. `fastboot -w`
10. `fastboot reboot`
