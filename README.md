![标题图](docs/EMO-Dot.jpg)

# EMO Dot 1.28(小豆AI表情机器人)
## 项目简介

EMO Dot 1.28(小豆)，采用7块2的ESP32 C3 Supermini开发板，高颜值玻璃盖板屏幕，3D打印外壳，具有表情显示，AI语音对话，英文学习等功能，角色及音色均可在小智AI后台配置。

## 项目特色
* 总成本低于50元（C3版本）

* 高颜值玻璃盖板

* 在ESP32S3 N4R2的极低内存和Flash中，实现了语音唤醒及对话功能

* 卡扣设计，无螺丝，组装复刻均很简单

* 角色及音色均可在小智AI后台配置

* 声纹识别

![ESP32 supermini C3淘宝价格](docs/supermini_price.png)
## 项目硬件
![EMO Dot bom](docs/EMO-Dot_bom.jpg)

### C3版本
| 型号 | 描述 | 链接 |价格 |
| ---- | ---- | ---- | ---- |
| ESP32 supermini C3 | C3开发板 | [淘宝链接](https://item.taobao.com/item.htm?id=748324039194) | 7.2|
| 1.28LCD | 带玻璃盖板 | [淘宝链接](https://item.taobao.com/item.htm?&id=694336841904) | 20|
| 1.28 lcd&Audio扩展板 | 屏幕背板及音频PCB | [立创开源](https://item.taobao.com/item.htm?id=728806967199) | 17|
| 喇叭 | 2415 | [淘宝链接](https://item.taobao.com/item.htm?id=728806967199) | 2.1|
| 麦克风 | 4015 | [淘宝链接](https://item.taobao.com/item.htm?id=764128372417) | 0.28|
| mx1.25转杜邦线8pin | 两根 | [淘宝链接](https://www.example.com/project2) | 2|
| 合计 |-|-| 48.58 |

#### 备注
    目前带玻璃盖板屏幕缺货中，价格可能有浮动，但是颜值没的说。

    后续会尝试出一个没有玻璃盖板的方案，敬请期待。
    
### S3版本
| 型号 | 描述 | 链接 |价格 |
| ---- | ---- | ---- | ---- |
| ESP32 supermini S3 | S3开发板 | [淘宝链接](https://item.taobao.com/item.htm?id=777200828819) |20.4 |

### 版本区别
C3版本无语音唤醒，必须触摸小豆机器人头顶触摸区域才能唤醒交互。机器人唤醒开始聆听对话后，无需再次触摸交互。

#### 注意事项
    部分ESP32 supermini C3开发板天线设计有缺陷，必须在menuconfig配置降低WIFI发射功率。

### 结构外壳
本项目结构参考了国外网友及MoveCall的MOJI设计。

由本人花了一天多的时间从零学习solidworks设计完成，因长时间以错误姿势画图，还导致了严重的手肘关节疼痛，一周多时间才恢复。

外壳使用拓竹P1SC打印机打印，去年双十一3400购入，真香！

makerworld模型链接：[EMO Dot 小豆表情机器人MakerWorld](https://makerworld.com.cn/zh/models/1003119-emo-dot-xiao-dou-biao-qing-ji-qi-ren)

## 固件烧录与编译
### 固件烧录
项目基于xiaozhi-esp32, 新手建议先不要搭建开发环境，直接使用免开发环境烧录的固件。

| 文件名 | 下载链接 | 备注 |
| ------ | -------- | -------- |
| Supermini C3版固件 | [下载](bin/EMO-Dot-C3-1.28-1.4.1_20250305.bin) |屏幕背光低电平有效|
| Supermini S3版固件 | [下载](bin/EMO-Dot-C3-1.28-1.4.1_20250305.bin) |屏幕背光低电平有效|

### 固件编译
开源代码见我fork的[xiaozhi-esp32](https://github.com/M-D-777/xiaozhi-esp32)，如有需要可按照xiaozhi-esp32文档自行编译烧写。

后续我也会向xiaozhi-esp32官方仓库提交pull requeset，希望虾哥能审核通过。

## 后续规划
* 更多的表情

* 增加1.8寸屏及AMOLED等各种屏的适配支持

* 结构及PCB优化

* 扩展智能家居等功能

## 致谢
* 感谢虾哥开源的小智AI，让广大网友可以零门槛创造AI机器人

* 感谢热心网友 - 你要不要吃菠萝，设计的可爱表情包

* 感谢鱼鹰光电鱼总[淘宝链接](https://shop110742373.taobao.com/shop/view_shop.htm)及大众点屏社区广大网友支持

