---
title: "openclaw 龙虾养成日记"
date: 2026-03-03T13:11:39+08:00
draft: false
description: "学习使用opneclaw"
tags:
- AI
categories:
- openclaw
comment : true
---


# openclaw 龙虾养成日记day1

26年春节期间，一只龙虾引爆了整个AI圈，由于这段时间忙着过年和写一篇agent的科研论文的投稿工作，每天我只是刷着手机和视频各种关于龙虾的资讯，还未亲手去实操一下，现在开学了，也投稿完了，刚到合肥第一天，看到导师在微信群里说了openclaw这个事情，于是现在才开始着手养一个自己的龙虾。

![alt text](/images/openclaw/image.png)


## 环境安装
我是直接用的官网的命令一键安装的
```
curl -fsSL https://openclaw.ai/install.sh | bash
```

![alt text](/images/openclaw/image1.png)

![alt text](/images/openclaw/image2.png)
![alt text](/images/openclaw/image3.png)
![alt text](/images/openclaw/image4.png)
![alt text](/images/openclaw/image5.png)

现在用kimi送的15元额度配置一下，用的是kimi2.5的模型

![alt text](/images/openclaw/image6.png)
![alt text](/images/openclaw/image7.png)
![alt text](/images/openclaw/image8.png)
![alt text](/images/openclaw/image9.png)
![alt text](/images/openclaw/image10.png)
![alt text](/images/openclaw/image11.png)
![alt text](/images/openclaw/image12.png)
![alt text](/images/openclaw/image13.png)
![alt text](/images/openclaw/image14.png)
![alt text](/images/openclaw/image15.png)

在搜索框内搜索「im:」勾选全部相关权限名称，最后点击「确认开通权限」；

![alt text](/images/openclaw/image16.png)
![alt text](/images/openclaw/image17.png)
![alt text](/images/openclaw/image18.png)
![alt text](/images/openclaw/image19.png)

下载飞书插件，在终端输入下方代码，然后回车，输入开机密码执行；
```
openclaw plugins install @m1heng-clawd/feishu
```
![alt text](/images/openclaw/image20.png)

安装完成

![alt text](/images/openclaw/image21.png)

在输入下方输入代码；
```
openclaw config
```
选择「Local (this machine)」;

![alt text](/images/openclaw/image22.png)
选择「Channels;

![alt text](/images/openclaw/image23.png)
选择「Configure/link」;

![alt text](/images/openclaw/image24.png)
选择「Feishu/Lark（飞书）」;

![alt text](/images/openclaw/image25.png)
打开飞书开放平台，在「应用凭证」里，复制 AppID 和 AppSecrect；

![alt text](/images/openclaw/image26.png)
安装一下feishu plugin 在终端对应位置分别输入飞书的 AppID 和 AppSecrect;

![alt text](/images/openclaw/image27.png)
参考图片进行选择，最后选择「Finished」

![alt text](/images/openclaw/image28.png)


![alt text](/images/openclaw/image29.png)
配置完成，关闭终端；

![alt text](/images/openclaw/image30.png)

 重新打开终端，然后输入下方代码，重启配置；
```
openclaw gateway
```
打开飞书开放平台，选择「事件与回调」→「订阅方式」→「使用长连接接收事件」→「保存」；

![alt text](/images/openclaw/image31.png)
然后点击同一页面内的「添加事件」；在弹出的列表中，搜索并添加 「接收消息」、「消息已读」、「机器人进群」、「机器人被移出群」，最后点击 「确认添加」；

![alt text](/images/openclaw/image32.png)

点击「权限管理」→搜索「通讯录」→选中「获取通讯录基本信息」→「确认开通权限」；

![alt text](/images/openclaw/image33.png)
配置完成后我们需要重新发布新版本，然后飞书搜索这个机器人就可以对话了；

![alt text](/images/openclaw/image34.png)

![alt text](/images/openclaw/image35.png)


参考：
https://zhuanlan.zhihu.com/p/2002370444339212951
https://zhuanlan.zhihu.com/p/2003776974779330870