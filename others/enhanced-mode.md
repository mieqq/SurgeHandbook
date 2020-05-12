# 增强模式

*仅 Surge Mac 2.1.0 以上版本支持此功能*

有些应用可能不会遵循系统代理设置，使用增强模式可以处理让 Surge 处理所有应用。

- Surge 会安装一个虚拟网卡并设置为默认路由。所有的 DNS 响应会返回 198.18.0.0/15 地址段的一个虚拟 IP 地址。
- Surge 虚拟网卡只能处理 TCP，UDP 和 ICMP 流量，仅在必要时开启此功能。
- ICMP 流量不能被代理，Surge 虚拟网卡将直接返回响应结果。