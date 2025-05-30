# OpenWrt专用插件源，实时同步上游（适用于官方OpenWrt）

### 在此感谢所有插件作者的辛苦付出

```shell
# OpenWrt插件源
git clone -b openwrt-package https://github.com/zouchanggan/package package/openwrt-package

# 更新 golang 1.24 版本
rm -rf feeds/packages/lang/golang
git clone https://github.com/sbwml/packages_lang_golang -b 24.x feeds/packages/lang/golang
```
