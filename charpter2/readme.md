# chapter2

## cover

- linux command line
- powershell for windows
- using a package manager
- choosing a code editor
- docker toolbox
- docker for mac & docker for windows
- minikube

## linux command line

linux & mac os x 都是派生于unix，所以通常有相同的shell，也就是我们使用的bash，不过有的linux没有bash只有sh，例如alpine。docker最早就是为了linux而开发，而且也是在linux开发，所以我们会需要使用很多的shell command。

## powershell for windows

windows原生的cmd实在太难用，后来microsoft搞了一个pwoer shell，终于可以使用任意的linux tool，比如bash等。

## using a package manager

mac上用homebrew
windows用chocolatey

### installing homebrew on a mac

访问 https://brew.sh/ 使用脚本安装

``` bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

安装成功使用命令来确认

``` bash
brew --version
```

### docker toolbox

- Docker CLI 客户端，用来运行docker引擎创建镜像和容器
- Docker Machine. 可以让你在windows的命令行中运行docker引擎命令
- Docker Compose. 用来运行docker-compose命令
- Kitematic. 这是Docker的GUI版本
- Docker QuickStart shell. 这是一个已经配置好Docker的命令行环境
- Oracle VM Virtualbox. 虚拟机

### Installing Docker for Mac

``` bash
homebrew cask install docker
```

### minikube

``` bash
homebrew cask install minikube
```