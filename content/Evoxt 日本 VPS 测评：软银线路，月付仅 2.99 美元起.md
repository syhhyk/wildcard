# Evoxt 日本 VPS 测评：软银线路，月付仅 2.99 美元起

## 测试 IP Looking Glass

以下是用于测试的 IP 地址：  
- IPv4: `107.165.195.226`  
- IPv6: `2400:8d60:8:0000:0000:0000:c65e:3969`

## 流媒体解锁测试

### IPv4 解锁情况  
网络环境：Evoxt Enterprise (107.165.*.*)  

#### 多国家流媒体支持  
- **Dazn**: 支持 (日本地区)  
- **HotStar**: 不支持  
- **Disney+**: 不支持  
- **Netflix**: 仅原创内容  
- **YouTube Premium**: 支持 (日本地区)  
- **Amazon Prime Video**: 支持 (日本地区)  
- **TVBAnywhere+**: 支持  
- **iQyi 海外地区**: 美国  
- **Viu.com**: 不支持  
- **YouTube CDN**: 大阪  
- **Netflix 首选 CDN**: 大阪  
- **Spotify 注册**: 不支持  
- **Steam 货币**: 日元 (JPY)  
- **ChatGPT**: 支持  
- **Bing 地区**: 日本  

#### 日本本地流媒体  
- **DMM**: 支持  
- **DMM TV**: 不支持  
- **Abema.TV**: 不支持  
- **Niconico**: 不支持  
- **music.jp**: 不支持  
- **Telasa**: 支持  
- **U-NEXT**: 支持  
- **Hulu Japan**: 支持  
- **TVer**: 支持  
- **GYAO!**: 支持  
- **WOWOW**: 测试失败  
- **VideoMarket**: 测试失败 (404 错误)  
- **FOD (Fuji TV)**: 不支持  
- **Radiko**: 不支持  
- **Karaoke@DAM**: 不支持  
- **J:com On Demand**: 支持  

#### 日本游戏支持  
- **Kancolle Japan**: 不支持  
- **Pretty Derby Japan**: 测试失败 (网络连接问题)  
- **Konosuba Fantastic Days**: 支持  
- **Princess Connect Re:Dive Japan**: 测试失败 (网络连接问题)  
- **World Flipper Japan**: 支持  
- **Project Sekai: Colorful Stage**: 不支持  

### IPv6 解锁情况  
网络环境：Evoxt Enterprise (2400:8d60:8:*:*)  

#### 多国家流媒体支持  
- **Dazn**: 测试失败 (网络连接问题)  
- **HotStar**: 支持 (马来西亚地区)  
- **Disney+**: 即将支持 [Disney+ MY]  
- **Netflix**: 支持 (马来西亚地区)  
- **YouTube Premium**: 支持 (马来西亚地区)  
- **Amazon Prime Video**: 不支持  
- **TVBAnywhere+**: 测试失败 (网络连接问题)  
- **iQyi 海外地区**: 测试失败  
- **Viu.com**: 测试失败  
- **YouTube CDN**: 东京  
- **Netflix 首选 CDN**: 大阪  
- **Spotify 注册**: 不支持  
- **Steam 货币**: 测试失败 (网络连接问题)  
- **ChatGPT**: 测试失败  
- **Bing 地区**: 马来西亚  

#### 日本本地流媒体  
- **DMM**: 不支持  
- **DMM TV**: 不支持  
- **Abema.TV**: 测试失败 (网络连接问题)  
- **Niconico**: 测试失败 (网络连接问题)  
- **music.jp**: 不支持  
- **Telasa**: 不支持  
- **Paravi**: 测试失败 (网络连接问题)  
- **U-NEXT**: 支持  
- **Hulu Japan**: 支持  
- **TVer**: 测试失败 (网络连接问题)  
- **GYAO!**: IPv6 不支持  
- **WOWOW**: 测试失败  
- **VideoMarket**: IPv6 不支持  
- **FOD (Fuji TV)**: 不支持  
- **Radiko**: 不支持  
- **Karaoke@DAM**: 测试失败 (网络连接问题)  
- **J:com On Demand**: 支持  

#### 日本游戏支持  
- **Kancolle Japan**: 不支持  
- **Pretty Derby Japan**: 支持  
- **Konosuba Fantastic Days**: 测试失败 (网络连接问题)  
- **Princess Connect Re:Dive Japan**: 测试失败 (网络连接问题)  
- **World Flipper Japan**: 支持  
- **Project Sekai: Colorful Stage**: 测试失败 (网络连接问题)  

👉 [2025年最新Evoxt优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

## TCP 回程路由测试

### 上海电信  
以下是 Evoxt 日本 VPS 到上海电信的回程路由测试结果：  

1   107.165.195.1   AS149440  日本 大阪府 大阪市  evoxt.com              2.31 ms  
2   203.96.239.240  AS4785    日本 大阪府 大阪市  xtom.com               7.81 ms  
4   203.96.236.9    AS4785    日本 大阪府 大阪    xtom.com               9.94 ms  
6   211.15.42.254   AS17676   日本 大阪府 大阪    softbank.jp            0.93 ms  
7   211.15.42.253   AS17676   日本 大阪府 大阪    softbank.jp            1.81 ms  
11  221.111.202.18  AS17676   中国 上海          softbank.jp           27.02 ms  
15  61.152.64.130   AS4812    中国 上海 浦东新区  chinatelecom.cn       45.23 ms  
16  101.95.52.34    AS4812    中国 上海          chinatelecom.cn        40.37 ms  

### 上海联通 9929  
以下是到上海联通 9929 的路由测试：  

1   107.165.195.1   AS149440  日本 大阪府 大阪市  evoxt.com             1.87 ms  
2   203.96.239.240  AS4785    日本 大阪府 大阪市  xtom.com              6.67 ms  
4   203.96.236.0    AS4785    日本 大阪府 大阪市  xtom.com              0.92 ms  
6   211.15.42.254   AS17676   日本 大阪府 大阪    softbank.jp           0.84 ms  
7   211.15.42.253   AS17676   日本 大阪府 大阪    softbank.jp           1.52 ms  
10  221.111.202.26  AS17676   日本 大阪府 大阪    softbank.jp           2.25 ms  
11  180.87.181.45   AS6453    日本 东京都 东京    tatacommunications.com  57.54 ms  
13  180.87.112.142  AS6453    中国 香港          tatacommunications.com  57.19 ms  
19  218.105.1.17    AS9929    中国 广东 广州      chinaunicom.cn        68.33 ms  
20  218.105.131.198 AS9929    中国 上海          chinaunicom.cn        66.22 ms  

### 教育网  
以下是到中国教育网的路由测试：  

1   107.165.195.1   AS149440  日本 大阪府 大阪市  evoxt.com             1.50 ms  
2   203.96.239.240  AS4785    日本 大阪府 大阪市  xtom.com             10.41 ms  
4   203.96.236.0    AS4785    日本 大阪府 大阪市  xtom.com              0.60 ms  
6   211.15.42.254   AS17676   日本 大阪府 大阪    softbank.jp           0.58 ms  
7   211.15.42.253   AS17676   日本 大阪府 大阪    softbank.jp           1.53 ms  
10  221.110.131.34  AS17676   日本 东京都 东京    softbank.jp           2.53 ms  
13  101.4.114.181   AS4538    中国 北京 海淀区    cernet.edu.cn         91.86 ms  
18  118.229.4.78    AS4538    中国 北京 海淀区    cernet.edu.cn         92.83 ms  

## IPv6 路由表现

### 常州电信 IPv6 路由  
以下是 Evoxt 日本 VPS 的 IPv6 路由测试（常州电信）：  

1   2400:8d60:8::1          AS149440  马来西亚          evoxt.com             1.78 ms  
2   2a10:481::e             AS4785    日本 大阪府 大阪市  xtom.com             4.23 ms  
5   2001:218:2000:5000::736 AS2914    日本             ntt.net               0.86 ms  
6   2001:218:2000:5000::735 AS2914    日本 大阪府 大阪   ntt.net               0.52 ms  
7   2001:218:0:2000::2a     AS2914    日本 大阪府 大阪   ntt.net               1.24 ms  
9   2001:418:0:2000::152    AS2914    美国 加州 圣何塞    ntt.net             165.81 ms  
15  2001:252:0:10c::1       AS23911   中国 北京 海淀区   cernet.edu.cn       169.61 ms  
20  2001:da8:2:11::1        AS23910   中国 上海         cernet.edu.cn       193.72 ms  

**建议**：IPv6 路由因地区差异较大，推荐用户自行测试以获取准确结果。

## 网络速度与延迟表现

Evoxt 日本 VPS 采用软银线路，目前用户较少且流量有限，但速度表现良好。以下是测试数据：  

节点名称       上传速度     下载速度     延迟  
Speedtest.net  54.75 Mbps   520.19 Mbps  86.68 ms  
新加坡 SG     752.57 Mbps  564.60 Mbps  74.50 ms  
东京 JP       769.01 Mbps  410.47 Mbps  33.13 ms  
美国 US       543.14 Mbps  521.75 Mbps 116.54 ms  
合肥 CT       170.44 Mbps  569.20 Mbps  36.28 ms  
江苏 CT       20.95 Mbps   716.45 Mbps  32.95 ms  
上海 CU       606.78 Mbps  286.05 Mbps  80.75 ms  

这款日本 VPS 的软银线路在东京地区的延迟低至 33.13 ms，下载速度最高可达 769.01 Mbps，非常适合需要高速网络和低延迟的用户。