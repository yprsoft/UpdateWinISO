# 在`Github Actions`上使用`Win_ISO_Patching_Scripts`自动集成`Windows 10/11`更新

## 说明
1. 本项目的主要目的是：使用`Win_ISO_Patching_Scripts`自动集成`Windows 10/11`更新(使用`Github Actions`自动构建)

## 地址
1. 本仓库地址: https://github.com/yuanpeirong/UpdateWinISO
2. `Win_ISO_Patching_Scripts`地址: https://github.com/adavak/Win_ISO_Patching_Scripts

## 目前已构建
- Windows 10 22H2(2025.10) amd64：
  - 母盘：`zh-cn_windows_10_consumer_editions_version_22h2_updated_oct_2025_x64_dvd_38efd00d.iso`
  - 集成后：`19045.6691.251205-1411.22H2_RELEASE_SVC_PROD1_CLIENT_X64FRE_ZH-CN.iso`
- Windows 10 LTSC 2021 amd64：
  - 母盘：`zh-cn_windows_10_enterprise_ltsc_2021_x64_dvd_033b7312.iso`
  - 集成后：`19044.6691.251205-1411.21H2_RELEASE_SVC_PROD1_CLIENT_X64FRE_ZH-CN.iso`

## 关于`W10UI.ini`
- 本仓库默认使用`Win_ISO_Patching_Scripts`的**预设**`W10UI.ini`
- 若要修改预设，可在本仓库修改`myini\W10UI.ini`，并在相应`yml`文件上将
  `:: copy D:\a\UpdateWinISO\UpdateWinISO\myini\W10UI.ini D:\a\UpdateWinISO\Win_ISO_Patching_Scripts\W10UI.ini /Y`
  改为
  `copy D:\a\UpdateWinISO\UpdateWinISO\myini\W10UI.ini D:\a\UpdateWinISO\Win_ISO_Patching_Scripts\W10UI.ini /Y`
