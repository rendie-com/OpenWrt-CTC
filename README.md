# OpenWrt-CTC 在线编译项目

![OpenWrt](https://openwrt.org/_media/logo.png)
<div align="center">
<img width="768" src="https://cdn.jsdelivr.net/gh/haiibo/OpenWrt/images/openwrt.png"/>
<h1>OpenWrt — 多设备固件云编译</h1>
## 项目简介

此仓库用于在线编译 OpenWrt 固件，支持多种设备。你可以通过 GitHub Actions 自动化编译你的固件，无需在本地配置编译环境。编译后的固件可直接用于设备刷机。

## 功能特点

- 多设备支持：支持多种设备型号，可自由选择和配置。
- 自动化工作流：基于 GitHub Actions 的在线编译系统，每次提交代码后自动触发编译。
- 插件集成：集成了常用的 OpenWrt 插件，你可以根据需要自定义编译的固件功能。
- 每日自动更新：通过 GitHub Actions 自动拉取最新的代码并进行编译，保持固件的最新状态。

## 使用说明

### 1. Fork 仓库

点击右上角的 Fork 按钮，将此仓库 Fork 到你自己的 GitHub 账户。


### 2. 配置参数

在 .config 文件中配置你需要的设备型号和插件包。如果需要自定义编译，可以修改 config.seed 文件中的相关设置。

### 3. 启动编译

1.Fork本仓库
2.加入自己的Token
3.可以手动运行或者点击Start触发编译程序


### 4. 下载固件

编译完成后，生成的固件会自动上传到 GitHub Releases，你可以在 Releases 页面下载。


## 注意事项

- Fork 后请手动触发一次编译：Fork 仓库后需要进入 Actions 标签页手动触发一次编译，以激活 GitHub Actions。
- 自定义插件和主题：你可以根据需要修改 .config 文件，选择需要的插件和主题。
- 编译失败处理：如果编译过程中遇到错误，请检查 .config 文件的配置是否正确，或查看 GitHub Actions 日志了解详细信息。

## 致谢

特别感谢以下项目和个人对本项目的支持与贡献：

- [OpenWrt](https://openwrt.org/): 提供了强大的开源路由器固件平台。
- [ImmortalWrt](https://github.com/immortalwrt/immortalwrt): 在 OpenWrt 基础上扩展了更多功能和插件支持。
- [haibo](https://github.com/haibo): 为本项目提供了启发性指导和模板参考。
- [QiuSimons](https://github.com/QiuSimons): 在 OpenWrt 和 ImmortalWrt 项目中做出了卓越的贡献，特别是在插件开发方面。

感谢你们的辛勤付出和无私贡献，让这个项目能够顺利进行！
