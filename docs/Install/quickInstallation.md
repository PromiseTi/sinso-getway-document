---
id: Quick installation
title: Quick Installation!
sidebar_position: 2
---

To install the sinso node, you need to complete the following procedure

1. Install the sinso GUI mining program

2. Configure the sinso parameter

3. Run sinso

4. Add the sinso node

5. Use TSINSO token to provide funds for your node for main network interaction

6. NAT address

7. Start the sinso node and check whether your sinso is working

## Install sinso

Currently supported systems:

1. Ubuntu 18.04

2. Windows 10

3. Mac (Intel chip)

# Download

To install the. exe file using our Express Installer, please download it at the following link

Ubuntu 18.04 Download address:

https://github.com/sinsoio/sinso-mine-ui/releases/download/v0.0.1/mine-ui-ubuntu-amd64.tar.gz

Windows 10 Download address:

https://github.com/sinsoio/sinso-mine-ui/releases/download/v0.0.1/mine-ui-windows-amd64.tar.gz

Mac （Intel chip） Download address:

https://github.com/sinsoio/sinso-mine-ui/releases/download/v0.0.1/mine-ui-mac-intel.tar.gz

## Configure sinso

The first time you start sinso, you need to configure it to meet your needs.

Edit Configuration Information

1. Node management account

Helps you query the nodes you created when pledging nodes. It also provides gas for the nodes you create

2. Node startup password

Help you start the node to verify security and export private keys. This password program will not be saved for you, so please back it up by yourself. If it is lost, we can't help you to retrieve it

3. Data storage directory

Sinso is decentralized storage, so you need to set your data storage directory. The minimum is not less than 100g.

![Coinlist ](../img/in1.jpg)

## Running sinso

After SINSO is configured, the performance of your device running sinso will be displayed, which will directly lead to the number of sinso nodes that your device can set up.

![Coinlist ](../img/in2.jpg)

## Add sinso node

You can directly enter a number less than or equal to the number prompted by the system, and click Auto Generate after input

![Coinlist ](../img/in3.jpg)

Of course, you can also manually configure your sinso node

![Coinlist ](../img/in4.jpg)

## Funding your nodes

After the Sinso node is configured, you need to provide funds for your node before the next step of sinso node startup. TSINSO is used as the consumption of gas on the chain. You can get the corresponding TSINSO GAS through the faucet

![Coinlist ](../img/in5.jpg)

After the above steps are completed successfully, you can start your node

![Coinlist ](../img/in6.jpg)

## NAT address

Sinso excitation network is about sharing and storing data. To enable other nodes to connect to your node, you must broadcast your public IP address and ensure that the node is accessible on the correct p2p port. We recommend that you manually configure your external IP and check the connection to ensure that your node can receive connections from other nodes.

- You can check whether your Internet port has been opened by displaying the status of the Internet port on the interface.

![Coinlist ](../img/in10.jpg)

If the interface shows that it is not open, you can also check it in the following way

First, determine your public IP address. Different systems have different detections. Let's take Ubuntu 18.04 as an example. (Other systems can search relevant operations online)

Command line input:curl icanhazip.com

```html preview
curl icanhazip.com
```

After accessing, you will get an IP address, which is your Internet IP address

```html preview
123.123.123.123
```

Then configure according to the node p2p port assigned by the system (for example, the port is 1634)

```html preview
nat-addr: “123.123.123.123 1634”
```

Check whether your node's p2p port is open. You can also judge by the following operations:

```html preview
nc -zv 123.123.123.123 1634
```

If the following message appears, the port is open

![Coinlist ](../img/in7.jpg)

If the following information appears, it means that the port is not opened or the network is wrong

![Coinlist ](../img/in8.jpg)

be careful

1. If the server has an independent Internet IP address, check whether the p2p port of the server to be configured is available on other servers. If not, check whether the machine and network have firewalls.

2. If there is no independent IP, you need to configure port mapping on the router or the network entrance device of the computer room. The external IP: port is mapped to the internal IP: port of the server that needs to open a port. Check whether the set internet ip: port is connected to other servers.

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
