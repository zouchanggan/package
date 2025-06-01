# 科学插件防炸上游备份

### 防止插件上游进行激进的改动，导致一些问题的出现，备份并按需同步可以确保编译时插件始终可用

```shell
# 移除 openwrt feeds 自带的核心包
rm -rf feeds/packages/net/{xray-core,v2ray-core,v2ray-geodata,sing-box}
git clone --depth 1 -b openwrt_helloworld https://github.com/zouchanggan/package package/openwrt_helloworld

# 更新 golang 1.24 版本
rm -rf feeds/packages/lang/golang
git clone https://github.com/sbwml/packages_lang_golang -b 24.x feeds/packages/lang/golang
```
