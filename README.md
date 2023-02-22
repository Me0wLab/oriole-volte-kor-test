# oriole-volte-kor-test

## Test Device
* Pixel 6
* SKTelecom

## ROMs to test
* CalyxOS
* ProtonAOSP 

## Solution

[pixel-volte-patch](https://github.com/kyujin-cho/pixel-volte-patch)
> This app uses Shizuku and override carrierconfig without ROOT.



## TODO
- [x] CalyxOS (Official Build supports VOLTE without modding)
> Official CalyxOS Build supports VOLTE without modifying build.prop.

> Cause: Wrong APN
- [x] ProtonAOSP
> Doesn't provide Proprietary files Extraction tools yet.

> Successfully built with aosp_oriole-user and VOLTE Provisioning enabled but, VOLTE doesn't work.

> Possible Causes: Missing Proprietary files provided by Google, Wrong APN

- [x] GrapheneOS
> Doesn't support VOLTE by default
> 
> https://github.com/GrapheneOS/os-issue-tracker/issues/956
