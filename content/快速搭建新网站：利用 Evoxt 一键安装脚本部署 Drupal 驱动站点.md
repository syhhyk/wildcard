# 快速搭建新网站：利用 Evoxt 一键安装脚本部署 Drupal 驱动站点

Drupal 是一个基于 PHP 开发的免费开源内容管理框架，广泛应用于全球至少 13% 的前 10,000 个网站，涵盖个人博客、企业官网以及政府门户等多样化场景。自 2001 年 1 月 15 日首次发布以来，Drupal 已拥有超过 20 年的发展历程，以其灵活性和强大功能受到用户青睐。本文将为您详细介绍如何通过 Evoxt 的一键安装脚本快速搭建 Drupal 网站，让建站过程更加高效。

## 第一步：接收虚拟机信息

在开始安装之前，请完成以下准备工作：

- **检查邮箱**：我们已将虚拟机（VM）的详细信息发送至您的注册邮箱。
- **注意垃圾邮件**：若未在收件箱找到，请查看垃圾邮件或垃圾箱。
- **联系支持**：若仍未收到信息，请及时联系我们获取帮助。

确认信息后，您即可进入 Drupal 网站的安装流程。

## 第二步：启动 Drupal 安装

Evoxt 提供的一键安装脚本能极大简化 Drupal 的部署过程。具体步骤如下：

1. **等待系统初始化**  
   系统需要一些时间完成 Drupal 的预配置。请耐心等待，完成后访问 `YOUR_VM_IP` 以进入安装界面。

2. **选择语言**  
   在安装页面，选择您所需的语言，然后点击 **Save and continue** 继续。

3. **挑选安装模式**  
   Drupal 提供三种配置选项，满足不同用户需求：
   - **Standard（标准版）**：内置常用功能，适合快速建站。
   - **Minimal（简化版）**：提供基础功能，适合有自定义需求的高级用户。
   - **Demo: Umami Food Magazine（实验版）**：展示 Drupal 功能的演示站点。

👉 [2025年最新Evoxt优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

## 第三步：配置数据库

数据库是 Drupal 网站运行的核心。使用以下命令完成配置：

bash
mysql -uroot -p'DATABASE_PASSWORD' -e "CREATE DATABASE IF NOT EXISTS drupal; GRANT ALL ON drupal.* TO 'root'@'localhost'; FLUSH PRIVILEGES"

运行示例：
bash
[root@TEST ~]# mysql -uroot -p'ZmM1MGU5ZWFmNzJlMmNkYm' -e "CREATE DATABASE IF NOT EXISTS drupal; GRANT ALL ON drupal.* TO 'root'@'localhost'; FLUSH PRIVILEGES"
mysql: [Warning] Using a password on the command line interface can be insecure.
[root@TEST ~]#

执行后，数据库即可正常支持 Drupal 运行。

## 第四步：完成安装与域名绑定

### 安装完成
数据库配置完成后，Drupal 将自动完成剩余安装步骤，您很快就能看到网站雏形。

### 域名设置
为确保网站正常访问，请将域名指向您的虚拟机 IP。具体操作可参考 Evoxt 提供的指南：[如何将域名指向您的虚拟机](https://bit.ly/evoxt)。正确配置 DNS 后，您的 Drupal 网站将通过域名正式上线。

## 第五步：管理数据库与附加功能

Evoxt 的一键安装脚本还预装了 phpMyAdmin，让数据库管理更加便捷：

- **访问 phpMyAdmin**：输入 `YOUR_VM_IP/phpMyAdmin`（注意大小写）。
- **登录信息**：用户名为 `root`。
- **获取密码**：通过 SSH 连接虚拟机，运行以下命令查看密码：
  bash
  cat /var/log/mysqld.log
  
  示例输出：
  bash
  [root@TEST ~]# cat /var/log/mysqld.log
  ZmM1MGU5ZWFmNzJlMmNkYm
  [root@TEST ~]#
  

完成以上步骤后，您的 Drupal 网站即可投入使用。借助 Evoxt 的高效工具，快速部署并优化您的在线项目吧！