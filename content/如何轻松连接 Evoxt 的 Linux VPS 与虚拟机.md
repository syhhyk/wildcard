# 如何轻松连接 Evoxt 的 Linux VPS 与虚拟机

Secure Shell（SSH）是一种基于 UNIX 的命令接口和协议，能够让用户安全地连接并访问远程计算机。它广泛应用于远程命令行操作、登录以及执行命令。SSH 的安全性极高，客户端与服务器之间的通信通过加密网络进行，即使在不安全的网络环境下也能确保数据安全。

## 获取 Evoxt 虚拟机的必要信息

在使用 SSH 连接之前，您需要先获取 Evoxt 提供的虚拟机详情，包括 **IP 地址**、**用户名** 和 **密码**。这些信息通常会通过电子邮件发送给您，请仔细检查收件箱。如果未找到邮件，不妨查看一下垃圾邮件或垃圾箱文件夹。

若仍未收到相关信息，可随时联系支持团队获取帮助，快速解决问题。

## 通过 SSH 连接您的 Linux VPS 或虚拟机

以下是针对不同操作系统的详细连接步骤，让您轻松上手。

### Windows 用户操作指南

对于 Windows 用户，您可以通过内置的命令提示符（CMD）进行连接。具体步骤如下：

1. 打开命令提示符（按 Win + R，输入 `cmd` 并回车）。
2. 输入以下命令，替换为您的用户名和虚拟机 IP 地址：
   bash
   ssh USERNAME@Your-VM-IP
   
3. 首次连接时，系统会提示验证主机真实性，输入 `yes` 确认。
4. 接着输入您的虚拟机密码，即可成功登录。

示例命令及提示：
bash
ssh root@192.168.0.1  
The authenticity of host '192.168.0.1 (192.168.0.1)' can't be established.  
RSA key fingerprint is SHA256:GY4yCL+HfYQXaKXePGlJvGcgKdvQR8OGTbmwbpiQbDE.  
Are you sure you want to continue connecting (yes/no/[fingerprint])?

### 使用 PuTTy 连接（推荐方式）

PuTTy 是一款简单易用的 SSH 客户端，特别适合 Windows 用户。连接步骤如下：

- 下载并安装 PuTTy。
- 启动 PuTTy，在“Host Name”字段输入您的 **虚拟机 IP 地址**。
- 确保端口号为默认值 `22`，然后点击“Open”按钮。
- 接受主机真实性提示（输入 `yes`），然后输入用户名和密码即可登录。

👉 [2025年最新 Evoxt 优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

### Linux 用户操作指南

如果您使用的是 Linux 系统，连接过程更为简便，只需以下步骤：

1. 打开终端（Terminal）。
2. 输入以下命令，替换为您的用户名和虚拟机 IP 地址：
   bash
   ssh USERNAME@Your-VM-IP
   
3. 首次连接时，确认主机真实性（输入 `yes`），然后输入密码即可完成登录。

通过以上方法，您可以快速、安全地连接到 Evoxt 的 **Linux VPS** 或 **虚拟机**，开始您的远程操作之旅。