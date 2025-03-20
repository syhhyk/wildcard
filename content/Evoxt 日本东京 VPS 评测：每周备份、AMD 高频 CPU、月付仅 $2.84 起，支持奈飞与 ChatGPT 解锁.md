# Evoxt 日本东京 VPS 评测：每周备份、AMD 高频 CPU、月付仅 $2.84 起，支持奈飞与 ChatGPT 解锁

## 商家简介

Evoxt 是一家成立于 2020 年的美国 VPS 服务商，拥有自有 ASN 212083。创始人来自马来西亚，支持中文沟通，方便国内用户交流。其数据中心覆盖英国伦敦、美国洛杉矶、马来西亚、德国等地，并支持多种支付方式，包括 PayPal、信用卡、加密货币以及支付宝。近期，Evoxt 新上线了日本东京 VPS，以其高性价比和流媒体解锁能力受到关注。本文将对这款东京 VPS 的性能、网络和功能进行详细评测。

## 线路概况

日本东京 VPS 采用自有 ASN，上游接入 Hydra Communications Ltd，支持 IPv4 和 IPv6 双栈网络。主要线路包括 Telia 和 PCCWG，整体带宽资源充足。不过需要注意的是，这款 VPS 未针对中国大陆进行优化。如果你需要更低的延迟和更稳定的国内访问体验，可以选择 Evoxt 接入日本软银的大阪机房 VPS。

## 配置与性能

以下是日本东京 VPS 的核心配置信息：

- **测试 IP**：`2400:8d60:10::1`
- **CPU**：AMD EPYC-Genoa 处理器，1 核心，主频 3693.060 MHz
- **内存**：总计 457 MB（可用 73 MB，含 150 MB 缓存）
- **存储**：总空间 4.9 GB（已用 1.3 GB），平均 I/O 速度 1809.1 MB/s
- **系统**：Debian GNU/Linux 12（64 位），KVM 虚拟化
- **内核**：6.1.0-9-amd64，TCP 拥塞控制算法为 BBR + FQ

这款 VPS 配备高频 AMD CPU，性能表现强劲，适合轻量级应用或个人项目。每周自动备份功能也为数据安全提供了额外保障。

👉 [2025 年最新 Evoxt 优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

## 流媒体解锁能力

日本东京 VPS 在流媒体解锁方面表现出色，以下是 IPv4 和 IPv6 的测试结果：

### IPv4 解锁情况
- **Netflix**：支持（地区：日本）
- **YouTube Premium**：支持（地区：日本）
- **Disney+**：支持（地区：日本）
- **TikTok**：支持（地区：美国）
- **iQIYI 国际版**：支持（地区：美国）
- **ChatGPT**：支持（地区：马来西亚）
- **Amazon Prime Video**：支持（地区：日本）

### IPv6 解锁情况
- **Netflix**：支持（地区：日本）
- **YouTube Premium**：支持（地区：日本）
- **Disney+**：支持（地区：日本）
- **TikTok**：支持（地区：美国）
- **ChatGPT**：不支持（网络连接失败）

从测试结果来看，IPv4 解锁能力更全面，适合追求流媒体体验的用户。IPv6 在部分服务上存在连接问题，建议根据实际需求选择网络协议。

## 网络速度测试

以下是全球主要节点的测速结果（IPv4）：

Node Name       Upload Speed    Download Speed    Latency
Speedtest.net   3224.57 Mbit/s  2107.64 Mbit/s    0.72 ms
Hong Kong CN    1107.54 Mbit/s  4918.90 Mbit/s    49.32 ms
Tokyo JP        1281.90 Mbit/s  9223.89 Mbit/s    0.97 ms
Singapore SG    790.35 Mbit/s   4279.06 Mbit/s    78.46 ms
Los Angeles US  633.59 Mbit/s   2930.83 Mbit/s    108.21 ms
London UK       279.91 Mbit/s   1699.52 Mbit/s    234.57 ms

测试显示，日本东京 VPS 在亚太地区（尤其是日本本地和香港）拥有极高的下载速度，带宽表现优异。欧美地区延迟较高，但仍能满足基本需求。

## 回程路由分析

以下是部分回程路由的测试数据：

### 到上海电信

1   10.1.1.21       RFC1918          0.29 ms
3   63.222.112.186  AS3491  南非 pccwglobal.com  0.72 ms
9   202.97.27.213   AS4134  中国 上海 电信  254.32 ms
16  101.227.191.14  AS4812  中国 上海 电信  251.73 ms

### 到广州移动

3   63.222.112.186  AS3491  南非 pccwglobal.com  0.74 ms
9   223.120.22.10   AS58453 中国 广东 广州 移动  217.25 ms
19  183.240.65.191  AS9808  中国 广东 汕头 移动  213.10 ms

回程路由表明，东京 VPS 到中国大陆的路径较长，未经过特别优化，延迟在 200-300 ms 之间，适合对延迟要求不高的场景。

## 性能基准测试

以下是 YABS 测试结果：

Processor  : AMD EPYC-Genoa Processor
CPU cores  : 1 @ 3693.060 MHz
RAM        : 457.8 MiB
Disk       : 4.8 GiB
iperf3 (IPv4):
- Singapore SG: 1.57 Gbits/sec (发送) / 1.22 Gbits/sec (接收)
- Los Angeles US: 1.15 Gbits/sec (发送) / 476 Mbits/sec (接收)

磁盘 I/O 速度高达 1809.1 MB/s，读写性能优异，适合需要快速存储操作的应用。

## 总结

Evoxt 日本东京 VPS 以月付 $2.84 的超低价格，提供了 AMD 高频 CPU、每周备份和强大的流媒体解锁能力。网络方面，其国际带宽充足，尤其在亚太地区表现优异，但在国内访问时延迟较高。如果你是流媒体爱好者或需要一台性价比高的海外 VPS，这款产品值得一试。对于追求大陆优化线路的用户，建议选择 Evoxt 其他机房方案。