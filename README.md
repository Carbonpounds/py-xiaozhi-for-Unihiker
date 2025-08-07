# py-xiaozhi-for-Unihiker
以下内容为原文：
***用python实现的小智客户端***,用于代码学习和在没有硬件条件下体验AI小智的语音功能</br>
* 原项目作者地址[xiaozhi-esp32](https://github.com/78/xiaozhi-esp32)</br>
* [***bilibili演示视频***](https://b23.tv/GbXeLHX)</br>
* **注意需要手动修改脚本中的全局变量MAC_ADDR**,以区分不同的客户端</br>
* **按住空格键发起对话**

**测试使用的python 版本为3.12(其它python3应该也可以,没做测试)**

## windows需要安装依赖
* pip 安装依赖模块
```python
pip3  install -r requirements.txt
```
* 将opus.dll拷贝到至C:\Windows\System32目录中

## 启动命令
```python
python py-xiaozhi.py
```

（正片开始doge）
## 更新了什么？
* main分支可用于跨平台使用（不知道啥意思的直接下载.py文件去用，这一段你没必要看）。行空板自带Linux操作系统和python环境，理论上本项目可以用于行空板的Linux操作系统。</br>
* 主要源代码来源于 DFRobot社区 云天 [**原帖**](https://mc.dfrobot.com.cn/thread-324368-1-1.html)</br>
* 源代码对行空板做了适配与GUI界面，激活对话方式有4种。本分支仅收录其中一种：按键，其余3种请移步至原帖。</br>
* 文件中的```speaker.py```为没有扬声器的用户提供了使用[DFR0760 离线语音合成模块](https://www.dfrobot.com.cn/goods-3014.html)作为替代品的方案</br>

## 如何使用
* 按下A键开始讲话，按下B键结束。</br>
* 如果使用语音合成模块，参考接线图：</br>
[![1.png](https://i.postimg.cc/FzR35XQN/1.png)](https://postimg.cc/gXCn85JT)
* 使用IO扩展板的接线：</br>
[![image.png](https://i.postimg.cc/SxM8Q619/image.png)](https://postimg.cc/K1m4JM2c)
