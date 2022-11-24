---
id: Quick installation
title: Quick Installation!
sidebar_position: 2
---

要安装 sinso 节点，您需要完成以下过程

1.安装 sinso GUI 挖矿程序

2.配置 sinso 参数

3.运行 sinso

4.添加 sinso 节点

5.用 TSINSO 代币为您的节点提供资金用于主网交互

6.NAT 地址

7.启动 sinso 节点并检查您的 sinso 是否正在工作

## 安装 sinso

当前支持的系统：

1. Ubuntu 18.04

2. Windows 10

3. Mac （Intel 芯片）

# 获取

要使用我们的快速安装程序安装.exe 文件，请在通过下面连接下载获取

Ubuntu 18.04 下载地址：

https://github.com/sinsoio/sinso-mine-ui/releases/download/v0.0.1/mine-ui-ubuntu-amd64.tar.gz

Windows 10 下载地址：

https://github.com/sinsoio/sinso-mine-ui/releases/download/v0.0.1/mine-ui-windows-amd64.tar.gz

Mac （Intel 芯片）下载地址：

https://github.com/sinsoio/sinso-mine-ui/releases/download/v0.0.1/mine-ui-mac-intel.tar.gz

## 配置 sinso

在您第一次启动 sinso，您需要对其进行配置以满足您的需要。

## 编辑配置信息

1. 节点管理账号

帮助您质押节点时查询您所创建的节点。并且为你创建的节点提供 gas

2. 节点启动密码

帮助您启动节点验证安全以及导出私钥。该密码程序不会帮你保存，所以请您自己备份好，如有丢失我们也不能帮您找回

3. 数据存储目录

sinso 为去中心化存储，所以您需要设置您的数据保存目录。最小不低于 100g。

![Coinlist ](../img/in1.jpg)

## 运行 sinso

配置好 SINSO 后，会显示出您的运行 sinso 的设备性能，这将直接导致您设备能够搭建 sinso 节点的数量。

![Coinlist ](../img/in2.jpg)

## 添加 sinso 节点

您可以直接输入小于等于系统提示的数字，输入后点击自动生成

![Coinlist ](../img/in3.jpg)

当然您也可以手动配置您的 sinso 节点

![Coinlist ](../img/in4.jpg)

## 资助您的节点

Sinso 节点配置好以后，再进入下一步 sinso 节点启动之前，您需要为您的节点提供资金，TSINSO 作为链上 gas 的消耗。您可以通过水龙头领取对应的 TSINSO GAS

![Coinlist ](../img/in5.jpg)

以上步骤成功完成后，就可以启动您的节点

![Coinlist ](../img/in6.jpg)

## NAT 地址

sinso 激励网络 是关于共享和存储数据的。要让其他节点连接到您的节点，您必须广播您的公共 IP 地址，并确保 节点在正确的 p2p 端口上可访问。我们建议您手动配置您的外部 IP 并检查连接以确保您的 节点 能够接收来自其他对节点的连接。

- 您可以通过界面显示外网端口状态查看您的外网端口是否已经打开。

如果界面显示未打开的情况，您还可以通过下面方式来检查

首先确定您的公共 IP 地址,不同的系统下检测不一样，下面就用 Ubuntu 18.04 来举例。（其他系统可以上网搜索相关操作）

命令行输入：curl icanhazip.com

```html preview
curl icanhazip.com
```

访问后，会得到一个 ip 地址，这个 ip 就是你的外网 ip 地址

```html preview
123.123.123.123
```

然后根据系统分配的节点 p2p 端口进行配置（比如：端口为 1634）

```html preview
nat-addr: “123.123.123.123 1634”
```

检查您的节点 p2p 端口是否打开，也可以通过以下操作来判断：

```html preview
nc -zv 123.123.123.123 1634
```

如果出现下列信息，则表示端口已打开

![Coinlist ](../img/in7.jpg)

如果出现下面信息，表示该端口未打开或者网络错误

![Coinlist ](../img/in8.jpg)

注意:

1、如果服务器有独立的外网 ip，在其他服务器上检查需要配置的服务器 p2p 端口是否通的。不通再检查机器、网络是不是有防火墙。

2、如果是没有独立 ip，需要在路由器或者机房网络入口设备配置端口映射。外网 ip:端口 映射到需要开端口的服务器内网 ip:端口。在其他服务器检查设置的外网 ip:端口是否通。

## 加入 sinso

如果一切顺利，您将看到您的节点开始正式工作，外网端口也是通畅的，运行也是正常的。

现在您的节点将开始请求属于您职责范围内的数据块——然后您将向在 SINSO 中运行的其他 p2p 客户端提供数据。接下来，您的节点将开始响应其他节点对这些区块的请求，您很快就会在 SINSO 中获得奖励。

## 警告

首次运行 SINSO 时，系统会要求您自动创建或者导入一个节点管理地址，如果您是导入，您需要导入地址的私钥。请放心吧。因为 SINSO 是一个去中心化的网络，所以不会有中心化的处理来窃取你的私钥。在手动添加节点时也是一样。

## 质押奖励。

SINSO 会每 4 小时调用一次工作量证明合约，检查你是否在线，是否存储了全网数据块，节点是否有质押币。如果都满足，您将获得相应的工作量奖励。

## 区块链 RPC 端点

您的 sinso 节点必须能够稳定访问 amstar Chain RPC 端点，以便它可以与您节点进行交互和部署，我们系统会自动分配 amstar Chain RPC 端点，不需要用户再去手动配置。

## 升级 sinso

要升级直接进入 about us 界面 ，点击 check for updates。系统会提示您是否是最新版本，如果不是可以点击下载更新

![Coinlist ](../img/in9.jpg)
