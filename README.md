# 云编译 N1 OpenWrt Docker固件
![Cloud OpenWrt](https://github.com/sj8023ld/Cloud-N1-OpenWrt/workflows/Cloud%20OpenWrt/badge.svg)


说明：
- 本项目使用 Github Actions 下载 [Lean](https://github.com/coolsnowwolf/lede) 的 `Openwrt` 源码仓库，进行云编译。
- 本项目编译固件适配斐讯 N1 盒子，如需刷机，另需使用打包工具生成刷机固件。
- 本项目相对源码默认设置做了如下更改：

**增强项**：（**打勾项**默认**编译**入固件；**未打勾项**默认**不编译**入固件。）
  - [x] 修改架构适配斐讯 N1 盒子
  - [x] 添加 Perl 依赖（待测试）
  - [x] 修改登录IP为 10.0.0.10，网关、DNS为 10.0.0.1，关闭DHCP服务
  - [x] 添加主题 opentomacat 并设置为默认
  - [x] 添加第三方插件 luci-app-openclash
  - [x] 添加第三方插件 subconventer

**精简项**：
  - [x] luci-app-accesscontrol
  - [x] luci-app-adbyby-plus
  - [x] luci-app-airplay2
  - [x] luci-app-ddns
  - [x] luci-app-ipsec-vpnd
  - [x] luci-app-upnp
  - [x] luci-app-vsftpd
  - [x] luci-app-xlnetacc
  - [x] luci-app-zerotier

## 感谢 ❤️
- 源码来源： Lean 的 Openwrt 源码仓库 https://github.com/coolsnowwolf/lede
- 脚本来源： P3TERX 的 使用 GitHub Actions 云编译 OpenWrt https://github.com/P3TERX/Actions-OpenWrt
- 自定义脚本来源：huangqian8 https://github.com/huangqian8/Cloud-N1-OpenWrt
