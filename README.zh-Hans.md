# OpenWRT Galaxy

OpenWRT 的三方软件包仓库

享受稳定，不再折腾。

你是否厌倦了一遍又一遍编译系统，在论坛等待“大神”发布各种“魔改版”，仅仅为了预装某个应用、甚至是只是为了个好看的 LuCI 主题。

这一切原本跟系统无关，只不过现行生态下没有简单的方式可以安装三方软件包  
现在有了 OpenWRT Galaxy，便可以使用可靠的官方系统，自由安装需要的软件

*其他语言版本: [English](README.md), [简体中文](README.zh-Hans.md).*

## 使用方法

1. 导入我们的签名公钥，在 ssh 里执行
```bash
wget https://openwrt-galaxy.nekoneko.today/key-build.pub
opkg-key add key-build.pub
rm key-build.pub
```

2. 添加源，在网页里 系统 - 软件包 - 配置 opkg
/etc/opkg/customfeeds.conf 最后面添加
```bash
src/gz openwrt_galaxy https://openwrt-galaxy.nekoneko.today/releases/22.03.0/packages/x86_64/galaxy
```

3. 更新列表，之后就能搜到想要的软件了

## 有哪些软件包
### LuCI 主题
- luci-theme-argon

### LuCI 应用

### 命令行应用
- speedtest
### 驱动
- kmod-r8168

## 支持哪些平台
目前起步阶段，为了开发方便我们暂时只支持 x86/64  
稳定之后会逐步扩展到所有官方支持的平台  
也可能会再加入一些官方不支持但很流行的硬件  

## 镜像
我们欢迎各大高校镜像站加入 OpenWRT Galaxy 镜像支持  
由于项目正在起步，我们希望能保持联络以便处理问题，因此请镜像站方联系下方维护人员来获取 rsync 地址。

## 维护人员
- https://t.me/nanamicat
- https://t.me/lty041127

## 社群
https://t.me/openwrt_galaxy
