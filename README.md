# Intranet Panel


> The goal of this project is to make the easiest, fastest, and most painless way of Linux VPS management. This project has been forked from VPSMate since 11 Jan 2017 but changed a lot.

Official Website: [intranet.pub](https://intranet.pub "Intranet")

#### Installation

```shell
# stable version
curl -O https://raw.githubusercontent.com/intranet-panel/intranet/master/install.py
python install.py

# beta version
curl -O https://raw.githubusercontent.com/intranet-panel/intranet/dev/install.py
python install.py --dev
```

#### Uninstall

```shell
service intranet stop
rm -rf /usr/local/intranet
rm -f /etc/init.d/intranet
```

#### Username and Password

```shell
/usr/local/intranet/config.py username 'your-username'
/usr/local/intranet/config.py password 'your-password'
```

#### Features

- 免费、简洁、开源
- 快速在线安装、小巧且节省资源
- 当前支持 CentOS/Redhat 5.4+、6.x
- 基于发行版软件源的软件管理机制
- 轻松构建 Linux + Nginx + MySQL + PHP 环境
- 强大的在线文件管理和回收站机制
- 快速创建和安装多种站点
- 丰富实用的系统工具

#### from VPSMate to Intranet

本管理面板只是在 UI 层面对系统服务及功能进行管理配置，并不会在系统中生成多余的依赖及配置文件，不管VPSMate 还是 Intranet，只是工具而已，卸载或安装，对系统已配置好的服务是没有影响的。

~~现阶段两者使用同一个进程服务文件，所以**只需要卸载 VPSMate ，再安装 Intranet 即可**。~~

从版本 Intranet v1.1.1b16 开始，不再使用 vpsmate 进程名，改用进程名为 intranet，在全新安装 Intranet 面板时，可以对已安装的 VPSMate 进行保留（或者删除）操作。

> 希望你用得愉快 ！
