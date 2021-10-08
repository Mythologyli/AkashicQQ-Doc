# 安装

在介绍如何安装 AkashicQQ 前，我们对 AkashicQQ 的架构进行一下介绍，这将有助于我们理解 AkashicQQ 的安装过程。

## AkashicQQ 架构

AkashicQQ 由以下几个模块构成，模块之间通过网络连接：

+ [AkashicQQ 机器人本体](https://github.com/Mythologyli/AkashicQQ)（一个 Python 程序）
+ [Prism Console](https://github.com/Mythologyli/Prism)（一个 Python 程序）
+ cqhttp(onebot) 协议实现程序，如 [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)、[onebot-kotlin](https://github.com/yyuueexxiinngg/onebot-kotlin)、[OneBot-YaYa](https://github.com/Yiwen-Chan/OneBot-YaYa) 等等

可能有读者觉得模块太多，但正是这样的实现增强了 AkashicQQ 的可拓展性、可自定义性，提升了 AkashicQQ 的性能。你甚至可以将三个模块安装在三个服务器上，自由地分配服务器性能。

Prism Console 与每个 Minecraft 服务器安装在一起。安装了 Prism Console 后，它将接管您的服务器控制台，以实现上报消息、执行命令等功能。

AkashicQQ 可以安装在任意位置，只要此位置能与每个 Prism Console 通过网络连接。AkashicQQ 负责异步地接收、处理 Prism Console 上报的消息，并控制 Prism Console 的行为。

AkashicQQ 并不能直接与腾讯的服务器通讯，而要借助 cqhttp(onebot) 协议实现程序。AkashicQQ 与 cqhttp(onebot) 协议实现程序交换信息，后者将信息与 QQ 群交换。您的机器人 QQ 号就是在 cqhttp(onebot) 协议实现程序上登录的。同样，cqhttp(onebot) 协议实现程序可以安装在任意位置，只要此位置能与 AkashicQQ 通过网络连接。

您当然可以将这三个模块安装在同一台服务器上。这三个模块都可以在 Windows 或 Linux 上运行，您无需担心平台问题。

## 安装前的准备

## 安装 Prism Console

## 安装 cqhttp(onebot) 协议实现程序

## 安装 AkashicQQ 本体