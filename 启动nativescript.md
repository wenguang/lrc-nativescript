
#### 启动nativescript的系统要求

1、macOS 10.12以上（具备）

2、更新Node到最新稳定版本
//清除npm缓存
npm cache clean -f
//安装n模块
npm install -g n
//升级node.js到最新稳定版
n stable
更新前node的版本是7.5.0(/usr/local/Cellar/node/7.5.0/bin/node)，更新后在该目录下./node --version检测版本是10.15.x了，也就是说node在原先的目录里更新了程序（这确实让我看了有点混乱）

3、Latest Xcode && Command-line tools for Xcode (具备)

4、xcodeproj ruby gem
sudo gem install cocoapods

5、安装及setup cocoapods
sudo gem install cocoapods
pod setup

6、Install python six package
pip install six

##### 安装nativescript
$ npm install -g nativescript
安装成功后在/usr/local/Cellar/node/7.5.0/bin/目录下多了一个命令：tns，这个命令要么在该目录下 ./tns运行，要么用全路径/usr/local/Cellar/node/7.5.0/bin/tns运行，既然在~/.bash_profile设计了别名：alias tns='/usr/local/Cellar/node/7.5.0/bin/tns'，也不能用tns运行命令（这很奇怪）

参考：
https://docs.nativescript.org/start/ns-setup-os-x
https://nativescript-vue.org/en/docs/getting-started/installation/



##### 用Vue-CLI模板创建app

$ npm install -g @vue/cli @vue/cli-init
$ vue init nativescript-vue/vue-cli-template <project-name>
$ cd <project-name>
$ npm install
$ tns run android --bundle
$ # or
$ tns run ios --bundle

参考：
https://nativescript-vue.org/en/docs/getting-started/upgrade-guide/



