---
title: CloudDualStackNodeIPs
content_type: feature_gate
_build:
  list: never
  render: false

stages:
  - stage: alpha
    defaultValue: false
    fromVersion: "1.27"
    toVersion: "1.28"
  - stage: beta
    defaultValue: true
    fromVersion: "1.29"
    toVersion: "1.29"
  - stage: stable
    defaultValue: true
    fromVersion: "1.30"
---
<!--
Enables dual-stack `kubelet --node-ip` with external cloud providers.
See [Configure IPv4/IPv6 dual-stack](/docs/concepts/services-networking/dual-stack/#configure-ipv4-ipv6-dual-stack)
for more details.
-->
允许在外部云驱动中通过 `kubelet --node-ip` 设置双协议栈。
有关更多详细信息，请参阅[配置 IPv4/IPv6 双栈](/zh-cn/docs/concepts/services-networking/dual-stack/#configure-ipv4-ipv6-dual-stack)。