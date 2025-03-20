# Evoxt 推出香港VPS全新套餐评测（2.99美元-月，100M端口）

## 香港VPS套餐概览

Evoxt 近期上线了香港地区服务器，最低定价仅为2.99美元/月，提供100M共享带宽的VPS服务。这款性价比极高的套餐适合对带宽需求不高的建站用户。以下是具体的配置详情和性能分析，帮助您了解这款香港VPS的实际表现。

### 套餐配置详情

- **核心**: 1个vCore  
- **内存**: 0.5GB  
- **存储**: 5GB NVMe  
- **位置**: 香港  
- **价格**: 2.99美元/月  
- **流量**: 默认500GB  

这款配置非常适合轻量级网站或小型项目，价格亲民且性能稳定。想了解更多优惠信息，可查看[2025年最新Evoxt优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)。

## 测试IP与Looking Glass

Evoxt 提供了测试IP供用户评估香港VPS的网络表现。以下是基于测试环境的详细数据，方便您判断是否符合需求。

## 流媒体解锁能力

针对流媒体支持情况，我们对多个主流平台进行了测试，结果如下：

- **Netflix**: 支持（地区：香港）  
- **Disney+**: 即将支持（Disney+ MY）  
- **YouTube Premium**: 支持（地区：马来西亚）  
- **Amazon Prime Video**: 不支持  
- **Spotify注册**: 不支持  

============[ Multination ]============
Dazn:              Failed (Network Connection)
HotStar:           No
Disney+:           Available For [Disney+ MY] Soon
Netflix:           Yes (Region: HK)
YouTube Premium:   Yes (Region: MY)
Amazon Prime Video: Unsupported
TVBAnywhere+:      Failed (Network Connection)
iQyi Oversea:      Failed
Viu.com:           Failed
YouTube CDN:       Singapore 
Netflix Preferred CDN: Singapore  
Spotify Registration: No
Steam Currency:    Failed (Network Connection)
=============[ Hong Kong ]=============
Now E:             Failed (Unexpected Result)
Viu.TV:            Failed (Network Connection)
MyTVSuper:         No
HBO GO Asia:       Failed (Network Connection)
BiliBili HK/MO/TW: Failed (Network Connection)

从测试结果来看，这款香港VPS对Netflix和YouTube Premium的支持较为出色，但其他平台的解锁能力有限，适合特定需求的流媒体用户。

## TCP回程路由测试

香港VPS的网络连接表现如何？我们针对多个国内线路进行了TCP回程路由测试，结果如下：

### 上海CN2（电信）

2   45.204.17.251   中国 香港   thegigabit.com   0.78 ms
5   123.255.91.41   中国 香港   hgc-intl.com     6.18 ms
7   59.43.248.109   中国    chinatelecom.cn  37.02 ms
10  101.95.88.206   中国 上海市   chinatelecom.cn  35.82 ms
12  58.32.32.1      中国 上海市 长宁区 chinatelecom.cn  30.29 ms

### 上海电信

2   45.204.17.251   中国 香港   thegigabit.com   0.58 ms
5   121.59.100.81   中国 香港   chinatelecomglobal.com  7.27 ms
10  101.95.88.38    中国 上海市   chinatelecom.cn  31.86 ms
11  61.152.71.66    中国 上海市 杨浦区 chinatelecom.cn  33.86 ms

### 上海联通9929

2   45.204.17.251   中国 香港   thegigabit.com   1.15 ms
5   123.255.91.154  中国 香港   chinaunicomglobal.com  6.01 ms
11  218.105.2.150   中国 上海市   chinaunicom.cn  33.27 ms
14  210.13.84.138   中国 上海市   chinaunicom.cn  38.55 ms

### 上海移动

2   45.204.17.251   中国 香港   thegigabit.com   1.70 ms
6   223.118.2.177   中国 香港   cmi.chinamobile.com  4.44 ms
11  111.24.4.237    中国 广东省 广州市  chinamobile.com  8.30 ms
18  183.232.226.1   中国 广东省 广州市  chinamobile.com  13.08 ms

移动和联通线路表现为直连，延迟较低，但可能存在QOS限速。电信CN2线路延迟稳定，适合对网络质量有一定要求的用户。

## IPv6路由表现

IPv6支持方面，这款香港VPS对教育网和深圳移动用户较为友好。由于不同地区的网络环境差异较大，建议用户自行测试以获取更准确的结果。

## 网络速度与延迟测试

以下是全球多个节点的测速结果，展示了香港VPS的上传、下载速度及延迟表现：

Node Name       Upload Speed  Download Speed  Latency     
Speedtest.net   57.59 Mbps    36.65 Mbps      59.00 ms    
Hongkong CN     66.60 Mbps    74.35 Mbps      3.25 ms     
Singapore SG    56.33 Mbps    56.42 Mbps      32.73 ms    
Tokyo JP        59.89 Mbps    30.39 Mbps      75.11 ms    
USA US          55.14 Mbps    41.84 Mbps      154.90 ms   
Shanghai CT     1.74 Mbps     1.54 Mbps       40.10 ms    
Shanghai CU     46.04 Mbps    32.71 Mbps      311.31 ms   
Gansu CM        67.77 Mbps    46.67 Mbps      55.82 ms

- **香港本地**: 下载速度高达74.35Mbps，延迟仅3.25ms，表现优异。  
- **国内线路**: 电信和移动延迟较低，但带宽受限；联通延迟稍高。  
- **国际节点**: 新加坡和日本延迟适中，美国和欧洲延迟较高，适合亚洲区域使用。

## 总结

Evoxt 的香港VPS以2.99美元/月的超低价格，搭配100M共享带宽和500GB流量，性价比突出。测试表明，其网络连接稳定，特别适合香港本地和亚洲地区的轻量建站需求。流媒体解锁能力有限，但对Netflix用户依然具有吸引力。综合来看，这款香港VPS是预算有限用户的优质选择。