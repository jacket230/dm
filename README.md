已迁移: https://github.com/damaiqiangpiao/damai

抢票说明（大麦、猫眼、纷玩岛），分几个流派。v53

**一.控制篇**  
**1.非root篇**  
**1)使用无障碍，autojs，升级版autoxjs**  
官方说明文档：  
http://doc.autoxjs.com/#/http  
http://doc.autoxjs.com/#/?id=%e7%bb%bc%e8%bf%b0

优势:无root，所有的安卓机型都可以用。  
劣势:某些app对于无障碍有监测，导致会存在一些出现类似于滑块的东西出现。以大麦为明显。  
<img src="https://github.com/jacket230/dm/blob/main/img/damai-huakuai.png" width = "300"  alt="" align=center />  

当然，在实现滑块操作上，有两种流派可以参考：  
A：python的ocr识别，以一些库为基础进行实现，本文作者已实现了本地识别。  
B：打码平台，通过截屏，发送数据包通过返回的数据包里面的坐标位置，进行滑动。某些打码平台可以支持到。  

学习参考：
飞云脚本学院：
[http://www.feiyunjs.com/autox](http://www.feiyunjs.com/autox)

视频：  

<video src="https://github.com/jacket230/dm/blob/main/img/2318_1698484421.mp4" autoplay="true" controls="controls" width="800" height="600">
</video>
<video controls="controls" name="media">
    <source src="https://www.w3school.com.cn/example/html5/mov_bbb.mp4" type="video/mp4">
</video>
**2）uiautomator2 控制**
官方文档：  
https://github.com/openatx/uiautomator2  
相关的项目：  
设备管理平台，设备多了就会用到 atxserver2
专门与adb进行交互的库 adbutils
atx-agent 运行在设备上的驻守程序，go开发，用于保活设备上相关的服务
weditor 类似于uiautomatorviewer，专门为本项目开发的辅助编辑器

weditor使用起来非常方便，可以很快的找打节点和相关的操作方法。可以说是自动化测试，控制的利器。


**2）root篇**  
A：Magisk 面具  
B：SuperSu  
刷ROM以及刷Root权限，不一一赘述，如果没有能力刷的，可以某宝或者某鱼，代刷。

在root完成之后，可以做到边缘计算的能力。结合termux，本地运行相关的python脚本，不依赖于中心服务器。  
本地运行脚本：
方法1，本地运行python，Android手机脱离电脑直接运行UIAutomator2 ： https://www.pimspeak.com/android-without-pc-run-uiautomator2.html  
方法2，创建本地apk，uiautomator2.0脱离PC运行，实现模拟点击 ：https://blog.csdn.net/jgw2008/article/details/102958295


**3）安卓篇：**
奋笔疾书中....

**4）IOS篇：**
奋笔疾书中....

**5）BP流派：**  
大麦bp链接生成方式：
https://blog.csdn.net/gs1we1/article/details/132124935


**二.逆向协议篇**  
**1)frida hook**   

/gw/mtop.trade.order.create  
/gw/mtop.trade.order.build  

效果：  
<img src="https://github.com/jacket230/dm/blob/main/img/damaiapp-hook.png" alt="" align=center />  

参考文档：
[Android逆向] 某麦网APK抢票接口加密参数分析
https://ycnote.com/?p=564  


大麦网回流票监控，sing参数分析
https://blog.csdn.net/q2919761440/article/details/133775618?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_baidulandingword~default-4-133775618-blog-132765825.235^v40^pc_relevant_anti_vip&spm=1001.2101.3001.4242.3&utm_relevant_index=7   

**2)xposed hook**  
淘宝系抓包hook模块：  
使用xposed模块hook淘宝的SPDY协议，使其能够被抓包  
https://blog.csdn.net/zhangmiaoping23/article/details/105827285  

**3)抓包协议**  


**三.余票监控：**  
参考：  
大麦、猫眼、纷玩岛，演唱会回流票监控：https://github.com/Raptor-wxw/TicketMonitoring  

票星球余票监控：https://github.com/caizhimin/Damai_ticket/blob/main/piaoxingqiu_ticket.py

研究不易，请多关照。

已迁移: https://github.com/damaiqiangpiao/damai  
入群不迷路。q群q：955767910  
<img src="https://github.com/jacket230/dm/blob/main/img/qqunqu-qrcode.jpg" width = "300"  alt="" align=center />  

<img src="https://github.com/jacket230/dm/blob/main/img/3qun.jpg" width = "300"  alt="" align=center />    
