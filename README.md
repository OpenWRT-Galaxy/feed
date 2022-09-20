# OpenWRT Galaxy

third-party software repository for OpenWRT

be stable, no more compile.  
install your favorite package on official openwrt release.

*Read this in other languages: [English](README.md), [简体中文](README.zh-Hans.md).*

## Usage

1. load our signing pubkey, in ssh:
```bash
wget https://openwrt-galaxy.nekoneko.today/key-build.pub
opkg-key add key-build.pub
rm key-build.pub
```

2. add source. in LuCI: system - software - configure opkg  
at the end of /etc/opkg/customfeeds.conf:
### x86_64
```bash
src/gz openwrt_galaxy https://openwrt-galaxy.nekoneko.today/releases/22.03.0/packages/x86_64/galaxy
```
### mt7620
```bash
src/gz openwrt_galaxy https://openwrt-galaxy.nekoneko.today/releases/22.03.0/packages/mipsel_24kc/galaxy
```
3. update lists.

## Collected Packages
### LuCI theme
- luci-theme-argon
### LuCI app

### command line app
- speedtest
### driver
- kmod-r8168

## Supported Platforms
on start, we only support x86_64
all official supported hardware will be supported.
and maybe some extra popular hardware.

## Mirrors
to host a mirror, please contact authors to get rsync address.

## Authors
- https://t.me/nanamicat
- https://t.me/lty041127

## Community
https://t.me/openwrt_galaxy
