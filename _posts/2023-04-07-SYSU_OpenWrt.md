---
layout: post
title:  "SYSU_OpenWrt记录"
date:   2023-04-07 22:20:39 +0800
categories: OpenWrt
---

声明：该篇博客仅作学习交流使用，禁止转载。图片源自网络，皆为非商业化用途，若存在侵权情况请联系作者要求删除。

自用校园网配置，硬件基于星际宝盒CM520-79F，目前还不够稳定，原因未知，有空会优化

## 支持情况

链接：<https://wiki.ubuntu.org.cn/锐捷、赛尔认证MentoHUST>

## 步骤

1. 安装VMware Workstation 15.5 Pro，激活方法自己找 (链接是16：<https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html>)
2. 创建虚拟机，基于Ubuntu 20.04.2 LTS，建议版本不要过旧 (链接：<https://ubuntu.com/download/desktop>)
3. clone Lean的Openwrt源码仓库 (链接：<https://github.com/coolsnowwolf/lede>)
4. 在package目录下clone openwrt-mentohust-sysu (链接：<https://bitbucket.org/etnperlong/openwrt-mentohust-sysu/src/sysu/>)
5. 在package目录下clone luci-app-mentohust-sysu (链接：<https://bitbucket.org/etnperlong/luci-app-mentohust-sysu/src/sysu/>)
6. 按照Lean的Openwrt源码仓库的教程编译固件 (记得勾选mentohust)
7. 路由器安装opboot (链接：<http://pandorabox.tuuz.cc:8000/星际宝盒/opboot/>)
8. 路由器通过opboot安装编译的固件
