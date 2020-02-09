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

## 相关资料
* [hololens官方文档————Microsoft官方](https://docs.microsoft.com/zh-cn/windows/mixed-reality/development "hololens官方文档")
* [markdown书写的基础语法](https://www.cnblogs.com/nickchen121/p/10821946.html "markdown基础语法")
* [2020/02/09 hololen模拟器初步尝试案例](https://blog.csdn.net/Zheye666/article/details/82384085 "hololen模拟器初步尝试")

## 问题与解决
* 2020/02/09 HoloLens Emulator（第一代）安装报错/无法安装 
    
    Microsoft官方网站中给出的VS2019安装方法不成功，VS2019稳定性较差，经本人尝试，改用***VS2017***即可成功安装。
    
    同时需要系统满足以下条件，否则安装时会报错：
  * 系统上已启用“Hyper-V”功能（在控制面板启用)
  * 在 BIOS 中，必须支持且启用以下功能：硬件协助的虚拟化、二级地址转换 (SLAT)、基于硬件的数据执行保护 (DEP)
  * VS2017中已安装UWP与C++的工作负载

* 2020/02/09 Unity Build Settings Platform 转为 UWP 时报错
  * 在UnityHub中下载对应版本的Unity的.NET模块
  * File -> Build Settings -> Player Settings -> 将Allow 'unsafe' code打上勾
  * [解决参考](https://blog.csdn.net/weixin_43884551/article/details/102996320)
