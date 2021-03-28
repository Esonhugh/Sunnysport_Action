# Sunnysport_Action
自动获得阳光长跑数据并推到手机


## 简介
> 关闭了阳光长跑的查询业务，我又懒得打开体联的网站查询
>
> 所以干脆就自己做个 Action 监控当日的跑步信息有无更新。
>
> 开源不易，如果本项目对你有帮助，那么就请给个star吧。😄

## 使用方式
1. Fork 本项目
2. 填写项目 Secrets
3. 点上 Star

## YOU Need Know

the time is 11:12 a.m in UTC 

and China is 19:12 p.m in UTC+8

## Secrets 中的参数

NAME|VALUE|e.g
----|-----|---
UID| your Student number |e.g: 20322230 
MINSPEED| The lowest speed in your group |e.g: 2.0 
MINMILEAGE| The shortest distance in your group | e.g: 2000 
PASS | PASSWORD of your accounts when login Sports| e.g: init password is your Student ID
TELEGRAM_BOTAPI| telegram bot api you make | e.g: '1234567890:'+'A'\*35 
TELEGRAM_USERID| telegram user id for your accounts | e.g: 000000000

## F&Q

### Secrets 在哪里设置？

1. 打开你 fork 的库
2. 点击库的 Settings
3. 点击左侧 Secrets
4. 点击 New repository secret



# 更多功能

## 自动同步上游代码

## 将参数填到Secrets

> 注意！为了确保 Push 权限足够，需要 Github Personal access tokens

`token`获取方式如下：

1. [生成新的token](https://github.com/settings/tokens/new)，点击这个链接。
2. 为`token`设置名字，然后把`workflow`勾选上，点击最下方`Generate token`即可生成`token`。

在`Secrets`中的`Name`和`Value`格式如下：

| Name  | Value                         |
| ----- | ----------------------------- |
| TOKEN | Github Personal access tokens |

在最新的代码中，已经加上自动同步上游代码的`Action`，将会定时在每周五`16`点执行，文件地址在`.github/workflows/auto_merge.yml`。

同时您也可以安装[pull](https://github.com/apps/pull)应用，也可实现自动同步上游代码。
