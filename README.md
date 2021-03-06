# v2ray-agent
- [Cloudflare 优化方案](https://github.com/mack-a/v2ray-agent/blob/master/documents/optimize_V2Ray.md)
- [流量中转](https://github.com/mack-a/v2ray-agent/blob/master/documents/traffic_relay.md)
- [手动自建教程](https://github.com/mack-a/v2ray-agent/blob/master/documents/Cloudflare_install_manual.md)
- [TG群](https://t.me/technologyshare)、[订阅频道](https://t.me/v2rayagentshare)、[博客地址](https://blog.v2ray-agent.com/)
- [公益订阅链接【4T】](https://github.com/mack-a/v2ray-agent/blob/master/documents/free_account.md)。

* * *
# 目录
- [1.脚本安装](#1vlesstcptlsvlesswstlsvmesstcptlsvmesswstlstrojan-伪装博客-五合一共存脚本)
  * [组合方式](#组合方式)
  * [组合推荐](#组合推荐)
  * [特性](#特性)
  * [注意事项](#注意事项)
  * [安装脚本](#安装脚本)
* * *

# 1.七合一共存脚本+伪装博客
- 如果没有使用过Cloudflare[点击这里](https://github.com/mack-a/v2ray-agent/blob/master/documents/cloudflare_init.md)查看入门教程

## 组合方式
- VLESS+TCP+TLS
- VLESS+TCP+XTLS
- VLESS+WS+TLS 
- VMess+TCP+TLS
- VMess+WS+TLS
- Trojan[Mux 多路复用]
- Trojan-Go+WS[Mux 多路复用]


## 组合推荐
- 中专/gia ---> VLESS+TCP+TLS/XTL or Trojan
- 移动宽带  ---> VMESS+WS+TLS/Trojan-Go+WS + Cloudflare
- Trojan建议开启Mux[多路复用]，仅需客户端开启，服务端自适应。
- VMess也可开启Mux，但是实测效果不佳，建议自己尝试。仅需客户端开启，服务端自适应。

## 特性
- VLESS/VMess/Trojan-Go三种工具合并为一个脚本，可以体验不同的工具之间的不同特性、兼容更多的设备。
- 支持Debian、Ubuntu、Centos
- 脚本自动检查升级
- 自动更新TLS证书


## 注意事项
- 修改Cloudflare->SSL/TLS->Overview->Full
- Cloudflare ---> A记录解析的云朵必须为灰色
- wget: command not found [这里需要自己手动安装下wget]
- 脚本安装路径[/etc/v2ray-agent]

## 安装脚本
```
wget -N --no-check-certificate "https://raw.githubusercontent.com/mack-a/v2ray-agent/master/install.sh" && chmod +x install.sh && ./install.sh
```
- 示例图
<img src="https://raw.githubusercontent.com/mack-a/v2ray-agent/master/fodder/install/install.jpg" width=700>

# 许可证
[MIT](https://github.com/mack-a/v2ray-agent/blob/master/LICENSE)

## Stargazers over time

[![Stargazers over time](https://starchart.cc/mack-a/v2ray-agent.svg)](https://starchart.cc/mack-a/v2ray-agent)
