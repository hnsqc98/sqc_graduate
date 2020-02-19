# README
## 进度记录
### 2020/01/29 
* 创建仓库，学习markdown语法。（[markdown基础语法](https://www.cnblogs.com/nickchen121/p/10821946.html "markdown基础语法")）
### 2020/02/04
* 下载/更新相关软件：
  * Visual Studio 2017（包括相关工作负载）
  * HoloLens Emulator（第一代）
  * Windows 10 SDK
    * HoloLens第一代开发应用程序，使用 Visual Studio 2017 安装的 Windows SDK
  * Unity（包括.NET相关安装包）
    * 本人使用版本为 Unity 2018.4.16，这是下文的 MRTK v2 所需的 LTS 版本。下载一个Unity Hub控制版本会更方便。
  * 混合现实工具包 (MRTK)
    * 适用于 Unity 的混合现实工具包 (MRTK) v2 是一款面向混合现实应用程序的开源跨平台开发套件。
    * 下载混合现实工具包 - 一系列脚本和组件，用于加速混合现实应用程序的开发。
    * 下载混合现实工具包-Unity - 使用基本工具包中的代码，使其更易于在 Unity 中使用。
    * 下载混合现实组件工具包 - 代码位和组件可能无法直接在 HoloLens 或沉浸式 (VR) 头戴显示设备上运行，但可通过与它们配对生成面向 Windows Mixed Reality 的体验。
### 2020/02/09
* 解决了HoloLens Emulator（第一代）无法安装的问题
* 解决了Unity Build Settings报错的相关问题
### 2020/02/11
* 完成 Unity -> VS2017 -> HoloLens Emulator 的项目部署，将练手的项目部署到HoloLens Emulator模拟器上并成功运行。
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/1.png)
### 2020/02/17
* 完成 Unity -> VS2017 -> HoloLens头盔的部署，将练手的项目导入Hololens头盔，并能独立启动。
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/2.jpg)


* 将Hololens头盔与电脑连接，可以在电脑端操作设备。
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/4.png)


* 完成无USB连接的情况下，从VS2017部署应用程序至Hololens头盔（在同一局域网下）
* 解决了部署时VS2017报错DEP0100的问题。

## 相关资料
* [markdown书写的基础语法](https://www.cnblogs.com/nickchen121/p/10821946.html)
* [B站-github使用启蒙](https://www.bilibili.com/video/av33238577?from=search&seid=7374412873796033945)
* [通过git提交文件到github仓库](https://www.cnblogs.com/alex-415/p/6912294.html)
  * git init //初始化仓库
  * git add .(文件name) //添加文件到本地仓库
  * git commit -m "first commit" //添加文件描述信息
  * git pull origin master // 把本地仓库的变化连接到远程仓库主分支
  * git push -u origin master //把本地仓库的文件推送到远程仓库
* [Microsoft官方文档：Hololens使用指南](https://docs.microsoft.com/zh-cn/windows/mixed-reality/development)
* [Hololens模拟器应用部署：Unity->VS2017->HoloLens Emulator模拟器](https://blog.csdn.net/Zheye666/article/details/82384085)
* [Hololens头盔应用部署](https://zhuanlan.zhihu.com/p/23672200?refer=kidscoding)
* [Microsoft文档：Hololens应用部署问题解决](https://docs.microsoft.com/zh-cn/hololens/hololens-known-issues)
* [Hololens与电脑连接：远程操控Hololens](https://www.cnblogs.com/mantgh/p/5448503.html)

## 问题与解决
* 【2020/02/09】**HoloLens Emulator（第一代）安装报错/无法安装** 
    
    Microsoft官方网站中给出的VS2019安装方法不成功，VS2019稳定性较差，经本人尝试，改用***VS2017***即可成功安装。同时需要系统满足以下条件，否则安装时会报错：
  * 系统上已启用“Hyper-V”功能（在控制面板启用)
  * 在 BIOS 中，必须支持且启用以下功能：硬件协助的虚拟化、二级地址转换 (SLAT)、基于硬件的数据执行保护 (DEP)
  * VS2017中已安装UWP与C++的工作负载

* 【2020/02/09】**Unity Build Settings Platform转为UWP时报错**
  * 在UnityHub中下载对应版本的Unity的.NET模块
  * File -> Build Settings -> Player Settings -> 将Allow 'unsafe' code打上勾
  * [解决参考](https://blog.csdn.net/weixin_43884551/article/details/102996320)
  
* 【2020/02/17】**在从VS至Hololens设备上部署应用时，开发者模式已打开，却报错DEP0100：请确保目标设备已启用开发人员模式。由于错误80004005，无法在某IP上获取开发人员许可证**
  * 我了解到这是很多开发者都会遇到的问题，在一番尝试后，找到根本原因为：在原本的Hololens上曾经用过VS2015或早期的VS2017部署应用，而现在较新版本的Visual Studio部署了组件的新版本，但是较旧版本中的文件会保留在设备上，从而导致更新版本失败。 
  * 解决方式较复杂，Microsoft官网给出了详细解决方式，实测解决成功
  * 详情：[解决参考](https://docs.microsoft.com/zh-cn/hololens/hololens-known-issues)
