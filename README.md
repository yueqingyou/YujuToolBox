# yuesir
一个Shell脚本工具箱

## 简介
本工具箱集成了一系列有用的系统管理工具和脚本，旨在帮助用户轻松管理和优化Linux服务器。

## 支持列表
仅支持Debian、Ubuntu系统

## 使用方法
### 准备
安装curl
```
apt update -y  && apt install -y curl
```
或者
```
apt update -y  && apt install -y wget
```

或者手动下载本脚本至服务器

### 下载并执行
用curl下载
```
curl -sS -O https://raw.githubusercontent.com/yueqingyou/YujuToolBox/main/yuesir.sh && chmod +x yuesir.sh && ./yuesir.sh
```
用wget下载
```
wget -q https://raw.githubusercontent.com/yueqingyou/YujuToolBox/main/yuesir.sh && chmod +x yuesir.sh && ./yuesir.sh
```

## 功能介绍
- 系统管理：更新、清理、TCP调优、BBR、洛杉矶时区、SWAP、随机SSH端口、fail2ban、UFW最小防火墙（含Docker转发防护）、密钥登录。
- 账户加固：关闭root用户密码登录，创建`yuesir`普通用户，配置免密码sudo/docker权限并同步root的`authorized_keys`。
- 测试脚本：SpeedTest、IP质量检测、nxtrace回程测试、yabs性能测试、IPv4/IPv6优先级测试、硬盘I/O测试。
- 常用工具：curl、wget、nano、unzip、tar、tmux、iftop、btop、gdu、fzf、zsh+Starship。
- Docker管理：安装、状态查看、清理、换源、IPv6开关、卸载。

## 项目参考
https://github.com/kejilion/sh

https://github.com/xykt/IPQuality
