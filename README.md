# README
This repository is built for ShenQichuan's graduation project ———— Implementation of interventional application of children’s autism spectrum disorder based on Hololens.
## Tips
若您在阅读本文时，Github无法加载图片或图片不显示，可使用hosts加速的方式：
* 若是Windows，则用记事本打开`C:\Windows\System32\drivers\etc\hosts`,在最下面将以下代码复制进去即可。
* 在Mac终端输入
```python
sudo vi /etc/hosts
```
* 输入密码后，点击`i`键，进入Insert模式，将下面内容拷贝进去。
```python
# GitHub Start
192.30.253.112    github.com
192.30.253.119    gist.github.com
199.232.28.133    assets-cdn.github.com
199.232.28.133    raw.githubusercontent.com
199.232.28.133    gist.githubusercontent.com
199.232.28.133    cloud.githubusercontent.com
199.232.28.133    camo.githubusercontent.com
199.232.28.133    avatars0.githubusercontent.com
199.232.28.133    avatars1.githubusercontent.com
199.232.28.133    avatars2.githubusercontent.com
199.232.28.133    avatars3.githubusercontent.com
199.232.28.133    avatars4.githubusercontent.com
199.232.28.133    avatars5.githubusercontent.com
199.232.28.133    avatars6.githubusercontent.com
199.232.28.133    avatars7.githubusercontent.com
199.232.28.133    avatars8.githubusercontent.com
 # GitHub End
```
* 点击`esc`键，然后输入`:wq`保存退出即可。
* 刷新Github，图片即可正常加载。
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


* 将Hololens头盔与电脑连接，可以在电脑端操作设备，包括拍照、录像等操作。


![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/4.png)


* 完成无USB连接的情况下，从VS2017部署应用程序至Hololens头盔（在同一局域网下）
* 解决了部署时VS2017报错DEP0100的问题。
### 2020/02/19
* 完成 Mixed Reality Toolkit (MRTK) 插件在Unity的部署
* 进行MR项目创作实践，调用模型以实现MR效果。
  * 第一视角
  <div align="center"><img width="500" height="auto" src="https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/5.jpg"/></div>

  <div align="center"><img width="500" height="auto" src="https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/7.jpg"/></div>

  <div align="center"><img width="500" height="auto" src="https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/8.jpg"/></div>

  * 第三视角(有点现代化办公的感觉=v=)
  <div align="center"><img width="500" height="auto" src="https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/9.jpg"/></div>

* 初步掌握了使用MRTK插件的开发方式。
### 2020/02/24
* 整理毕业设计所需参考的相关论文，再次明确开发目的，初拟论文大纲。
### 2020/03/03
* 近段时间在尝试空中绘画功能的开发，找教程以及尝试自己解决各种报错和版本不匹配问题。
* 粗翻了一篇英文文献《HoloLearn：Learning through Mixed Reality for People with Cognitive Disability》，主要讲的是一款Hololens应用“HoloLearn”，针对的用户群体是认知障碍（CD）患者，目的是通过MR教他们一些日常自主生活的能力。其中孤独谱系障碍是认知障碍的一种，并且论文是“2018 IEEE International Conference on Artificial Intelligence and Virtual Reality (AIVR)”会议刊物上的，这篇论文讲的应用程序“HoloLearn"对我的毕设参考价值较大。开发团队指出Hololens对于这类患者的治疗辅助应用程序非常少，所以这也是一个可以深入的点，鼓励更多的开发者去尝试，这么说我的毕设也有挺大的价值。
* 文献翻译已上传至translation文件夹
### 2020/03/08
* 本周开发工作复杂，工程量巨大，成果较多。
  * 三分之一的时间在翻译论文（成果在上面已经提及）
  * 三分之一的时间在寻找空中绘画的开发方式、与版本报错作斗争
  * 三分之一的时间应用已掌握的技能和开发方式，自主开发了一个初具成效的Hololens应用《PlantTrees》（本毕设第一个应用功能）
* （空中绘画功能开发的）主要问题来源于
  * 版本的无限不匹配，微软在2018年将HTK插件全面升级为了MRKT插件，导致大量之前的模型以及功能无法使用，且缺失文件
  * 开发工具与VS2017版本不匹配，而VS2019在MR上会报错导致无法更换版本
  * HTK插件资料和教程、源码都已被微软删除，找不到匹配的开发源
  * MRTK的教程过于复杂，看了几天仍然有报错问题出现
  * 缺少MRTK的绘画开发教程，自己摸索巨困难，只有HTK的模型和教程，但HTK已经用不了了被淘汰了
  * 总之仍在找方法，调错误的过程中
* 关于这周做出来的Hololens应用《PlantTrees》
  * 灵感来源于翻译的论文，应用的目的是激发自闭症孩子的兴趣以及好奇心，适当增强自闭症孩子的动手能力
  * 规则：将左边的树模型拖动至画面的任意位置，任意地放大、缩小、旋转它，直到你觉得合理为止！
  * Unity场景概览：公路、桥梁、楼房、树模型、动漫女孩（之后尝试给她添加动作，针对自闭症孩子的应用应该有一些可爱的引导人物，可以增加亲切感）
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/PT1.png)  
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/PT2.png) 
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/PT7.jpg) 


  * 将树的模型打上边框，在凝视（gaze）时变化颜色，并在敲击（Airtap）并拖拽（drag）时变化边框颜色
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/PT5.png) 


  * 随意地移动、缩放、旋转
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/PT6.png) 


  * 我戴着Hololens实地操作，拍摄了一个视频，沉浸感比较强，体验也是较好的，尤其是在MR环境下，下面截几张图
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/PT8.jpg)  
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/PT9.jpg)
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/PT10.jpg)
  * 后面的画和花是我家的实景，可以看到，MR的虚拟、现实的融合效果还是不错的，即“混合现实”。
![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/PT11.jpg)

 * 另外就是，我本来想把这个视频传到github上，但github是不允许100M以上文件的，除非LFS，详见问题解决【2020/03/08】。
 * 再另外，更新了windows如果看不到图片的解决方法，详见本文开头的Tips。
 ### 2020/03/16
 * 本周完成了一直以来存在问题的空中绘画功能。
   * 最后用调整版本的方式解决，下了2017年版本的MRTK插件，并且重新下了一个旧版本的Unity，将Unity与插件的版本完全匹配。
     * [MRTK历代版本存档](https://github.com/microsoft/MixedRealityToolkit-Unity/releases?after=2017.4.0.0-rc2)
     * [Unity历代版本存档](https://unity3d.com/get-unity/download/archive)
   * 因为一代Hololens不存在如二代Hololens较为丰富的手势，最终开发选用了凝视、单击、拖动三个Hololens动作
   * 将Hololens视点聚焦于颜色球上，运用单击并拖拽的动作，将颜色球移动，从而在真实环境下渲染出虚拟的线条，进而实现空中绘画的功能
 * 下面是功能演示（GIF图）
 * 环境平面扫描
   
   
 ![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/draw1s.GIF)
   * MR绘画
   
   
 ![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/draw2s.GIF)
 
 
 ![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/draw3s.GIF)
   * MR绘画（与真实物体的接触，达到混合现实的效果）
   
   
 ![avatar](https://github.com/hnsqc98/sqc_graduate/blob/master/Picture/draw5s.GIF)
 
 
* 现存问题
  * 绘画功能用2017.2.1.4插件版本开发，但该插件版本与MRTK不兼容。
  * 换言之，无法整合，将开发完成的应用打包导入新版本Unity后，无法运行。
  * Microsoft官方文档关于2017.2.1.4版本的插件中有写`This release is specifically targeted for Unity Editor-2017.2.1p2`
  * 即运行要求为：低版本插件配低版本Unity，或高版本插件配高版本Unity，且二者不兼容，无法打包导入
  * Microsoft官方文档关于两代插件（HoloToolkit与MRTK）的升级描述：`由于重建了框架，因此没有从HoloToolkit到Mixed Reality Toolkit v2的直接升级路径。`
  
  
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
* [Microsoft文档：构建和部署MRTK](https://microsoft.github.io/MixedRealityToolkit-Unity/Documentation/BuildAndDeploy.html)
* [Microsoft文档：MRTK入门](https://microsoft.github.io/MixedRealityToolkit-Unity/Documentation/GettingStartedWithTheMRTK.html)
* [MRTK的应用部署方式](https://blog.csdn.net/JiangCoolguy/article/details/94549643)
* [Unity-Chan动漫人物模型](https://unity-chan.com/)

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
  
* 【2020/02/19】**使用Unity-MRTK插件时Build报错**
  * 不在Build Settings中进行Build，而是在上方菜单栏中选择MRTK的子选项进行Build。
  * [解决参考：三（2）中有描述](https://blog.csdn.net/JiangCoolguy/article/details/94549643)
  
* 【2020/03/08】**在github上面push100M以上大小文件时报错**
  * github上除非用LFS不然时不允许上传100M以上文件的（以前还真不知道，第一次踩这个坑，可麻烦死我了）
  * 比较MMP的是，在上传失败后必须将git回调至上传前的最后一个正确版本（记得存档），即使你已经装了LFS，也要先回调，再push，否则git的记录里有100M以上文件的git信息，之后的git就无法成功。我在多方尝试之后用了这个解决方法：[git回调解决参考](https://blog.csdn.net/weixin_42762089/article/details/94320794)，以及[git-LFS下载链接](https://git-lfs.github.com/)
  * 另外一个办法是用BFG的Java命令直接把git里面的超过100M的文件提交记录给删光，但需要装java sdk，方法贴在这里[BFG解决参考](https://www.jianshu.com/p/4919056b33a9)，[BFG下载链接](https://rtyley.github.io/bfg-repo-cleaner/#download)
  * 总之大文件能别传就别传了

* 【2020/03/09】**git push文件太慢，甚至因为速度太慢报错停止push**
  * 修改HOSTS文件
  * [解决参考](https://blog.csdn.net/feixiangzaitianye/article/details/99646077?depth_1-utm_source=distribute.pc_relevant.none-task&utm_source=distribute.pc_relevant.none-task)
## 主要参考文献
* [1] G. Tian-Han, T. Qiao-Yu and Z. Shuo, "The Virtual Museum Based on HoloLens and Vuforia," 2018 4th Annual International Conference on Network and Information Systems for Computers (ICNISC), Wuhan, China, 2018, pp. 382-386.
* [2] S. Sirilak and P. Muneesawang, "A New Procedure for Advancing Telemedicine Using the HoloLens," in IEEE Access, vol. 6, pp. 60224-60233, 2018.
* [3] F. Garzotto, E. Torelli, F. Vona and B. Aruanno, "HoloLearn: Learning through Mixed Reality for People with Cognitive Disability,"  2018 IEEE International Conference on Artificial Intelligence and Virtual Reality (AIVR), Taichung, Taiwan, 2018, pp. 189-190.
* [4] A. Adjorlu, E. R. Høeg, L. Mangano and S. Serafin, "Daily Living Skills Training in Virtual Reality to Help Children with Autism Spectrum Disorder in a Real Shopping Scenario," 2017 IEEE International Symposium on Mixed and Augmented Reality (ISMAR-Adjunct), Nantes, 2017, pp. 294-302.
* [5] B. Munsinger, G. White and J. Quarles, "The Usability of the Microsoft HoloLens for an Augmented Reality Game to Teach Elementary School Children," 2019 11th International Conference on Virtual Worlds and Games for Serious Applications (VS-Games), Vienna, Austria, 2019, pp. 1-4


