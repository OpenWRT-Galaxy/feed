include $(TOPDIR)/rules.mk

PKG_NAME:=speedtest
PKG_VERSION:=1.2.0
PKG_RELEASE:=1
PKG_LICENSE:=https://www.speedtest.net/about/eula
PKG_SOURCE:=ookla-speedtest-$(PKG_VERSION)-linux-x86_64.tgz
PKG_SOURCE_URL:=https://install.speedtest.net/app/cli/
PKG_HASH:=5690596c54ff9bed63fa3732f818a05dbc2db19ad36ed68f21ca5f64d5cfeeb7

include $(INCLUDE_DIR)/package.mk

define Package/speedtest
	SECTION=:net
 	CATEGORY:=Network
	TITLE:=Ookla Speedtest CLI
	URL:=https://www.speedtest.net/
	MAINTAINER:=nanamicat77@gmail.com
	PKGARCH:=x86_64
endef

define Package/speedtest/description
	Official Ookla Speedtest CLI for personal, non-commercial use
endef

define Build/Prepare
	$(Build/Prepare/Default)
endef

define Build/Compile
endef

define Package/speedtest/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(BUILD_DIR)/speedtest $(1)/usr/bin/speedtest
endef

$(eval $(call BuildPackage,speedtest))
