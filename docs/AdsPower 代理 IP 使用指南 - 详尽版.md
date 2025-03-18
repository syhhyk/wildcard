# AdsPower 代理 IP 使用指南 - 详尽版

## 产品简介

代理 IP 分为两大类：**动态住宅 IP** 和 **静态住宅 IP**。动态住宅 IP 的特点是 IP 地址会不断变化，而静态住宅 IP 则保持固定不变。所谓住宅 IP，是指国外网络运营商分配给真实家庭用户的宽带 IP，这种 IP 不易被目标网站封禁。相比之下，**机房 IP（数据中心 IP）** 则是由物理机房生成的 IP 类型。

此外，基于 IP 轮换机制，代理还可分为 **轮换代理** 和 **非轮换代理（粘性 IP）**。轮换代理通过额外的轮换系统实现 IP 自动更换，用户无需手动提取，操作更加便捷。

---

## 使用动态住宅 IP 的详细步骤

> **重要提示**：动态住宅 IP 仅支持海外环境使用，不兼容大陆环境！

### 步骤 1：配置 AdsPower 指纹浏览器

在 **AdsPower 指纹浏览器** 中直接设置代理信息即可。登录后，您可以在账户后台查看代理的域名、端口、账号和密码。

#### 参数说明：
- **代理地址**：`proxy.ipipgo.com`（固定域名）
- **代理端口**：`31212`（固定端口）
- **代理账号**：  
  示例格式：`customer-account-Country-US-Session-region-NewYork-AAABBB-Time-3`  
  - 可选参数：  
    - `Country`（国家，如 US）  
    - `Session`（粘性 IP 会话标识）  
    - `region`（地区，如 NewYork，国家下一级行政单位）  
    - `Time`（粘性 IP 保持时长，单位分钟）  
  - 不区分大小写，可根据需求删减参数。
- **代理密码**：在 IPIPGO 官网后台生成。

#### 会话类型说明：
1. **轮换代理**：每次浏览器请求更换一次 IP  
   - 全球 IP 轮换：`customer-account`  
   - 美国 IP 轮换：`customer-account-Country-US`  
   - 美国纽约 IP 轮换：`customer-account-Country-US-region-NewYork`  
     （地区列表可联系客服获取）

2. **粘性代理**：IP 在指定时间段内保持不变，最长支持 60 分钟  
   - 全球 IP 粘性 30 分钟：`customer-account-session-7a9b4d6a92e9495-time-30`  
   - 美国 IP 粘性 30 分钟：`customer-account-country-US-session-42de00178ce144f-time-30`  
   - 美国纽约 IP 粘性 30 分钟：`customer-account-country-US-region-NewYork-session-42de00178ce144f-time-30`

![获取代理信息](https://198301.xyz/img/506844386263348.webp)

### 步骤 2：安装并设置 AdsPower 指纹浏览器

1. 下载并安装 **AdsPower 指纹浏览器**。
2. 登录后，点击“添加浏览器”，自定义浏览器名称，其他设置可保持默认。
3. 进入“配置”页面，输入代理地址、端口、账号和密码。

![新建浏览器](https://198301.xyz/img/280141571045.webp)  
![设置代理](https://198301.xyz/img/38318858670708.webp)

> **注意**：支持 HTTP/HTTPS/SOCKS5 协议，不支持 SOCKS4。检测到的 IP 以 IPv6 格式显示，但不影响实际使用。

AdsPower 指纹浏览器是一款专为多账号运营设计的防关联、防封号神器，致力于解决出海账号矩阵的安全管理问题，目前已通过市面 100% 指纹安全网站检测！  
👉 [**【限时福利】点击此处或使用邀请码：VIPFreeTrial 免费领取 VIP 会员专业功能试用！**](https://bit.ly/adspower_free)

### 步骤 3：验证代理（可选）

配置完成后，可在 AdsPower 浏览器中输入 `ipinfo.io` 检查代理 IP。若设置为美国 IP，检测结果显示美国地址，即表示代理成功。

![验证代理](https://198301.xyz/img/0407083301.webp)

---

## 使用静态住宅 IP 与数据中心 IP 的步骤

1. 在官网购买 **静态住宅 IP** 或 **数据中心 IP** 后，登录账户后台查看 IP 地址、端口、账号和密码。
2. 将相关信息填入 AdsPower 指纹浏览器的代理配置中，步骤与动态住宅 IP 设置相同。

![静态 IP 信息](https://198301.xyz/img/02728199644.webp)  
![端口与账密](https://198301.xyz/img/514705021486.webp)  
![配置详情](https://198301.xyz/img/5710317014.webp)

---

通过以上步骤，您可以轻松在 AdsPower 指纹浏览器中配置并使用动态住宅 IP、静态住宅 IP 或数据中心 IP，保障多账号运营的安全性与稳定性！