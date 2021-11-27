---
id: Quick installation
title: Quick Installation!
---

## (Testing phase, functions not fully open)

We provide a convenient installation script that will automatically detect your execution environment and install the latest stable version of the SINSO client on your computer.

Currently supported system: Ubuntu 18.4

To install the binary file using our quick installation script, run any of the following commands in the terminal:

## Wget

`wget -q -O - https://raw.githubusercontent.com/sinsoio/SINSO/master/install.sh | tag= v0.0.3 bash `

## Curl

`curl -s https://raw.githubusercontent.com/sinsoio/sinso/master/install.sh | tag= v0.0.3 bash `

## Run SINSO

After installing SINSO, you can run to test whether it has been successfully installed.

`sinso`

`0.0.3`

Now that your SINSO node has been installed, you can use TSINSO to `fund your node` and join SINSO!

After installing SINSO, just type sinso start in your terminal.

This command will start SINSO for the first time and prompt
you to add your wallet address.

## WARNING

It is strongly recommended to use a service manager, such as systemctl to run SINSO, to avoid various file permission problems that may occur when manually operated without careful file management. If you are running a supported release version, using the attached packages will automatically set up these services for you.

## Import Your Wallet

When you run SINSO for the first time, the system will ask you to import a wallet address, which is the address of the VIP node you applied for. Besides, you need to import the private key of the address. Please rest assured. because SINSO is a decentralized network, there will be no centralized processing to steal your private key. Importing the private key is for the staking. Since the test staking currency is free to receive, so the staking operation does not require manual operation.

## Staking Reward

To join SINSO, you must include configuration parameters that specify a valid BSC RPC endpoint. You can run your own BSC node, or use the RPC provider.

SINSO will call the proof-of-work contract each hour to check whether you are online and whether the node has staked coins. If both are satisfied, you will be rewarded with the corresponding workload.

## Join SINSO

If all goes well, you will see your node automatically start connecting to other SINSO nodes around the world.

`INFO[2021-07-29T11:55:16Z] from other node message <Hello sinso>:b6ae5b22d4dc93ce5ee46a9799ef5975d436eb63a4b085bfc104fcdcbda3b82c`

Now your node will start requesting data blocks that fall within your scope of responsibility - then you will provide data to other p2p clients running in SINSO. Next, your node will start responding to requests from other peers for these blocks, and you will soon be rewarded in SINSO.

## Getting Help

SINSO has built-in documentation.

Run SINSO --help, it has given you an entry point into the documentation.

## Upgrade SINSO

To upgrade the previous version of SINSO installed using the above method, just re-run the above installation commands.
