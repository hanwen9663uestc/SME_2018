## 【嵌入式 · 进阶题：计步器】  
利用MPU6050实现一个计步器（满分120分）  

---

### 【基础要求】
- 读取MPU6050传感器读取得到当前的3个方向角加速度，以及三个角度轴的加速度，并且在显示屏上显示出来，或利用按键数码管切换显示（20分）  
- 当检测到物体自由落体时（下落时的方向随机，总的加速度大于7米每平方秒即可以认定自由落体），机器会发出报警（10分）  
<br />
  
### 【拓展要求】
- 可以通过WiFi或者蓝牙将获得的加速度信息传给手机或者电脑（20分）
- （70分）在已知加速度下利用卡尔曼滤波等手段可以计算出累计行进路程，当我拿着你的传感器向前走2m时，观察出你计算出的累计路程是多少，精度越高得分越高。测试分为四步：  
  - 1）慢速直线行走2m  
  - 2）快速直线行走2m  
  - 3）直线行走1m后沿随机方向再行走1m  
  - 4）曲线行走2m  
<br />
  
### 【注意事项】
- 只有完成基础任务，才能完成拓展任务。仅完成拓展任务不得分。  
<br />
  
### 【参考资料】
#### 1. 《STM32库开发实战指南》：
<p align="center">
 <img src="https://github.com/CXCYGZF-UESTC/SME_2018/raw/master/%E5%B5%8C%E5%85%A5%E5%BC%8F%20%C2%B7%20%E8%BF%9B%E9%98%B6%E9%A2%98/picture/%E5%9B%BE%E4%B8%80.jpg">
</p>  
  
#### 2. 《电子设计从零开始》：
<p align="center">
 <img src="https://github.com/CXCYGZF-UESTC/SME_2018/raw/master/%E5%B5%8C%E5%85%A5%E5%BC%8F%20%C2%B7%20%E8%BF%9B%E9%98%B6%E9%A2%98/picture/%E5%9B%BE%E4%BA%8C.jpg">
</p>  
  
#### 3. 涉及模块：数码管，按键，EEPROM
#### 4. STM32开发板（学习用的板子上面很多模块都有）  
https://item.taobao.com/item.htm?id=20428448343  
#### 5. 卡尔曼滤波理解（仅作参考，可以使用其他滤波，反正最后是比谁精度高，那个效果好用哪个）  
https://www.zhihu.com/question/23971601
#### 6. 视频教程  <br />
- 腾讯课堂下载链接：https://ke.qq.com/course/279762?tuin=1730a331  
- 腾讯课堂在线观看链接：https://ke.qq.com/course/278479  
- 百度网盘下载链接：  
  - A盘独立压缩包: http://pan.baidu.com/s/1c2zdIJQ 程序源码，手册，软件等除视频外的所有其他资料  
  - B盘独立压缩包: http://pan.baidu.com/s/1i5GwEqT 视频盘,《手把手教你学STM32-M3》视频  
  - C盘独立压缩包：http://pan.baidu.com/s/1miPJYeW 视频盘,《手把手教你学STM32-M3》视频  
  - D盘独立压缩包：http://pan.baidu.com/s/1i4UZ4Lf 视频盘,《手把手教你学STM32-M3》视频  
