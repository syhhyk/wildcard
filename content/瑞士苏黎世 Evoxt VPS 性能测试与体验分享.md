# 瑞士苏黎世 Evoxt VPS 性能测试与体验分享

## 购买概览

本次测试的 VPS 配置如下：

- **规格**: 1 vCore / 512 MB 内存 / 5 GB 存储 / 500 GB 流量  
- **价格**: 约 2.99 美元/月  

这是一款性价比不错的基础套餐，适合轻量级应用或测试使用。

## 使用体验

Evoxt 最新推出的瑞士苏黎世数据中心表现令人期待。当前 IP 显示为马来西亚，可能是数据库尚未更新，需稍作等待。服务器采用 AMD EPYC Genoa 处理器，性能表现强劲，带宽资源也较为充裕，适合高负载任务。不过，由于内存和存储配置偏低，若用于建站可能需要升级套餐以满足需求。

此外，IPv6 分配为 /48 子网，但目前存在连接问题，官方正在修复中，值得后续关注。

## 性能测试

以下是详细的测试数据，涵盖系统信息、硬件性能和网络表现，供大家参考。

### 系统信息

-> 系统信息

CPU 型号:                AMD EPYC-Genoa 处理器
CPU 缓存:                L1: 32.00 KB / L2: 1.00 MB / L3: 32.00 MB
CPU 规格:                1 vCPU
虚拟化支持:              无
虚拟化类型:              KVM
内存使用:                72.09 MiB / 459.85 MiB
交换分区:                未检测到交换分区或文件
磁盘使用:                2.05 GiB / 4.83 GiB
启动盘:                  /dev/vda1
操作系统:                Debian GNU/Linux 12 (bookworm) (x86_64)
内核版本:                6.13.4-x64v3-xanmod1

-> 网络信息

IPv4 地址:               [MY] 38.225.209.73
IPv4 AS信息:             AS149440 - Evoxt Enterprise
IPv4 地理位置:           马来西亚 吉隆坡

### 硬件性能

-> CPU 性能测试 (快速模式，单次 5 秒)

单线程测试:              6112.02 分 (1.00x)

-> 磁盘性能测试 (FIO, 直接模式, 32 IO 深度)

写入 (4K 块):            219.30 MB/s (56140 IOPS)
读取 (4K 块):            704.22 MB/s (180281 IOPS)
写入 (128K 块):          3846.15 MB/s (30769 IOPS)
读取 (128K 块):          9090.91 MB/s (72727 IOPS)

磁盘读写速度表现优异，尤其是大块数据传输，适合需要高吞吐量的场景。

### 网络速度 (iperf3)

iperf3 网络速度测试 (IPv4):
---------------------------------
提供商          | 地点                     | 发送速度        | 接收速度        | 延迟
-----           | -----                    | ----            | ----            | ----
Clouvider       | 伦敦, 英国 (10G)         | 3.85 Gbits/s    | 5.15 Gbits/s    | --
Eranium         | 阿姆斯特丹, 荷兰 (100G)  | 5.15 Gbits/s    | 3.54 Gbits/s    | --
Uztelecom       | 塔什干, 乌兹别克斯坦 (10G)| 1.32 Gbits/s    | 4.65 Gbits/s    | --
Leaseweb        | 新加坡 (10G)             | 893 Mbits/s     | 1.26 Gbits/s    | --
Clouvider       | 洛杉矶, 美国 (10G)       | 579 Mbits/s     | 1.39 Gbits/s    | --
Leaseweb        | 纽约, 美国 (10G)         | 1.62 Gbits/s    | 1.35 Gbits/s    | --
Edgoo           | 圣保罗, 巴西 (1G)        | 583 Mbits/s     | 1.19 Gbits/s    | --

网络表现因地区差异明显，欧洲节点速度更快，而亚太和美洲地区稍逊一筹。

👉 [2025年最新Evoxt优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

### Speedtest 测速

root@jam-zhlr-01:~# speedtest -s 5396
   Speedtest by Ookla
   服务器: 中国电信江苏 5G - 苏州 (id: 5396)
   ISP: Evoxt Enterprise
空闲延迟:   185.11 ms (抖动: 0.08ms, 最低: 185.04ms, 最高: 185.19ms)
下载速度:  1484.97 Mbps (数据使用: 1.8 GB)
           287.71 ms (抖动: 74.79ms, 最低: 184.56ms, 最高: 1339.39ms)
上传速度:   631.76 Mbps (数据使用: 680.2 MB)
           298.23 ms (抖动: 74.82ms, 最低: 198.17ms, 最高: 395.34ms)

root@jam-zhlr-01:~# speedtest -s 24447
   Speedtest by Ookla
   服务器: 中国联通 5G - 上海 (id: 24447)
   ISP: Evoxt Enterprise
空闲延迟:   200.74 ms (抖动: 0.03ms, 最低: 200.72ms, 最高: 200.81ms)
下载速度:  3608.40 Mbps (数据使用: 4.9 GB)
           305.86 ms (抖动: 75.09ms, 最低: 200.09ms, 最高: 399.85ms)
上传速度:   591.13 Mbps (数据使用: 681.0 MB)
           311.01 ms (抖动: 75.82ms, 最低: 207.89ms, 最高: 415.32ms)
丢包率:     0.0%

国内节点测试显示下载速度可观，尤其是联通线路表现突出，延迟则因地理距离稍高。

### 流媒体解锁情况

** IPv4 解锁测试
--------------------------------
网络提供商: Cogent Communications (38.225.*.*)

============[ 全球服务 ]============
Dazn:                  是 (地区: 马来西亚)
Disney+:               即将推出 [Disney+ MY]
Netflix:               是 (地区: 马来西亚)
YouTube Premium:       是 (地区: 马来西亚)
Amazon Prime Video:    是 (地区: 美国)
TVBAnywhere+:          是
Spotify 注册:          是 (地区: 马来西亚)
iQyi 海外地区:         美国
Bing 地区:             马来西亚
YouTube CDN:           华盛顿特区
Netflix 首选 CDN:      苏黎世
ChatGPT:               是
Google Gemini:         是 (地区: 马来西亚)
Claude:                是
Steam 货币:            MYR

============[ 欧洲服务 ]============
Paramount+:            失败 (错误: 406)
Discovery+:            否 (亚太暂不可用)
HBO Max:               是 (地区: 美国)
SkyShowTime:           否
BritBox:               是
Rakuten TV:            否

目前 IPv4 支持多种主流流媒体服务，但部分欧洲地区服务受限。IPv6 测试因主机不支持而跳过。

### 路由追踪 (Traceroute)

#### 中国电信 (北京)

NextTrace v1.3.5
traceroute to 45.126.112.33, 最大 30 跳
1   38.225.209.1       3.10ms  AS149440, 苏黎世, 瑞士, evoxt.com
3   213.248.83.116     0.24ms  AS1299, 苏黎世, 瑞士, arelion.com
4   62.115.126.198     9.76ms  AS1299, 法兰克福, 德国, arelion.com
9   202.97.61.213    201.13ms  AS4134, 北京, 中国, chinatelecom.com.cn
17  45.126.112.33    237.59ms  AS4847, 北京, 中国, chinatelecom.cn

#### 中国联通 (上海)

NextTrace v1.3.5
traceroute to 103.116.79.1, 最大 30 跳
1   38.225.209.1       2.47ms  AS149440, 苏黎世, 瑞士, evoxt.com
3   213.248.83.116     0.32ms  AS1299, 苏黎世, 瑞士, arelion.com
6   219.158.41.97      9.89ms  AS4837, 法兰克福, 德国, chinaunicom.cn
12  139.226.230.181  199.41ms  AS17621, 上海, 中国, chinaunicom.cn
15  103.116.79.1     232.85ms  AS17621, 上海, 中国, chinaunicom.cn

#### 中国移动 (广州)

NextTrace v1.3.5
traceroute to 183.232.48.167, 最大 30 跳
1   38.225.209.1      10.07ms  AS149440, 苏黎世, 瑞士, evoxt.com
3   149.6.176.76       1.01ms  AS174, 苏黎世, 瑞士, cogentco.com
20  223.120.6.69     217.19ms  AS58453, 圣何塞, 美国, cmi.chinamobile.com
23  221.183.89.33    317.53ms  AS9808, 上海, 中国, chinamobileltd.com
30  183.232.48.167   490.76ms  AS56040, 广州, 中国, gd.10086.cn

路由测试显示国内三大运营商延迟较高，尤其是移动线路，需优化网络路径。