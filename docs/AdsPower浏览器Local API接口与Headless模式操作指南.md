# AdsPower浏览器Local API接口与Headless模式操作指南

## 概述

最新版本的AdsPower客户端（应用版本v3.3.2及以上，内核版本v2.4.2.8及以上）现已支持**headless模式**结合**api-key**启动无界面服务，并通过Local API实现高效操作。这一功能为需要多设备管理账号的用户提供了极大的便利。

> **注意**：此功能仅限拥有Local API权限的用户使用。如需开通权限，可联系在线客服进行申请。

---

## 核心概念

- **Headless**：用于启动“无界面服务”的参数，帮助用户在后台运行浏览器。
- **API-Key**：无界面服务中调用Local API接口的身份凭证，每个账号对应一个唯一的api-key，支持多设备同时操作。

---

## 获取API-Key的步骤

获取api-key是使用Local API的第一步，以下是具体操作流程：

1. **打开AdsPower客户端**  
   进入“账号管理-设置”界面。

2. **生成API-Key**  
   在“基础API接口”选项中，点击“生成api-key”按钮。

3. **复制API-Key**  
   生成后，复制你的专属api-key以备后续使用。

---

## 使用命令行启动无界面服务

在获取api-key后，可通过命令行启动无界面服务。以下是详细步骤：

### 1. 确认命令行环境
确保已在AdsPower安装目录中打开命令行工具（CMD或Terminal）。  
- **Windows默认路径**：`C:\Program Files (x86)\AdsPower`  
- **MacOS默认路径**：`/Applications/adsPower.app/Contents/MacOS`

### 2. 输入启动命令
将复制好的api-key填入以下命令中：

#### Windows系统

AdsPower.exe --headless=true --api-key=XXXX --api-port=50325

#### MacOS系统

/Applications/adsPower.app/Contents/MacOS/Adspower --args --headless=true --api-key=XXXX --api-port=50325

#### 支持的参数说明
| 参数         | 是否必填 | 说明                              |
|--------------|----------|-----------------------------------|
| `--headless` | 是       | 设置为`true`时启用无界面服务      |
| `--api-key`  | 是       | 操作Local API的身份凭证           |
| `--api-port` | 否       | 指定Local API的服务端口，默认可选 |

### 3. 验证启动成功
启动成功后，命令行会返回Local API的访问地址，表明服务已正常运行。

---

## 有界面服务与无界面服务的区别

- **有界面服务**：同一账号仅限单设备登录，适合简单操作场景。
- **无界面服务**：支持同一账号在多设备同时运行，非常适合需要自动化管理的用户。

如果你需要在多个设备上实现账号自动化操作，推荐使用**headless模式**结合api-key调用Local API接口。

> **推荐工具**：AdsPower指纹浏览器，一款专为多账号运营打造的防关联、防封号神器，致力于解决出海账号矩阵安全管理问题，目前已通过市面100%指纹安全网站检测！  
> 👉 [【限时福利】点击此处或使用邀请码：VIPFreeTrial 即可免费领取VIP会员专业功能试用！](https://bit.ly/adspower_free)

---

## 常见问题解答（FAQ）

### Q：更换api-key后，旧的api-key还能继续使用吗？
**A**：不能。系统会提示旧api-key失效。每个账号仅对应一个有效api-key，重置后需使用新值重新启动服务。

### Q：如何重置api-key？
**A**：在客户端“账号管理-设置”界面，点击“重置api-key”按钮生成新值。重置后请妥善保存新api-key。

### Q：更换api-key后，已运行的服务可以直接更新吗？
**A**：不行。需先关闭现有服务，再使用新api-key重新启动。

---

## 总结

通过headless模式和Local API接口，AdsPower为多账号管理和自动化操作提供了强大支持。掌握api-key的生成与命令行启动技巧，你可以轻松实现多设备协同工作，提升运营效率。