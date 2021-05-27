---
title: '渠道'
previousText: '实时更新版本'
previousUrl: '/docs/appflow/deploy/builds'
nextText: 'Differentials'
nextUrl: '/docs/appflow/deploy/differentials'
---

一个频道指向指定的应用实时更新，将与任何配置为 监听该频道进行更新的设备共享。 您可以随时更改channel指向的构建，也可以回滚更改。

当你在应用程序中(通过点击channel中的下载介绍)[下载了Appflow SDK](/docs/appflow/quickstart/installation)，任何配置到该channel的本机二进制文件都将在加载通道时检查该通道是否有可用的更新

## 设置Channel

每个应用都有两个默认channel： **Master**和**Production**。

常见的用例是将**Production** Channel 用于App Store二进制文件，并使用** Master ** Channel 是在开发过程中自动在手机上运行本机二进制文件。

设置频道后，只需单击该频道旁边的**安装说明**，它将引导您完成可用的选项并生成应运行的命令行命令。

要创建这两个以上的新channel，必须拥有付费的Ionic Appflow成员资格。 要添加新频道，只需前往部署 -> 目标来查看频道列表，然后点击 `New destination` 按钮。

## 构建Channel

创建频道后，请返回到应用的**Builds**部分。 在每个内部版本的右侧，您将看到一个"Deploy live updates"按钮。

![构建Channel](/docs/assets/img/appflow/assign-to-channel.png)

点击此处设置 Build为Channel的活动。

一旦构建被设置为一个频道活动。任何已经用Ionic Live Update 设置的本地二进制文件将在下次检查时收到新的更新。

## 从Git分支自动部署

如果您有兴趣从git自动化部署到将其部署到某个channel，请使用我们的[Automation](/docs/appflow/automation/intro)功能，如果您的[计划](/pricing)包含这些功能，。