# py-xiaozhi-for-Unihiker
以下内容为main分支原文：</br>
The following is the original text of the main branch:</br>
***用python实现的小智客户端***,用于代码学习和在没有硬件条件下体验AI小智的语音功能</br>
***py-xiaozhi***, for code learning and experiencing AI Xiaozhi's voice functions without hardware.</br>
* 原项目作者地址[xiaozhi-esp32](https://github.com/78/xiaozhi-esp32)</br>
* URL of the original project author: [xiaozhi-esp32](https://github.com/78/xiaozhi-esp32)</br>
* [***bilibili演示视频***](https://b23.tv/GbXeLHX)</br>
* [***Watch the demo video on Bilibili***](https://b23.tv/GbXeLHX)</br>
* Not available on Youtube because author is in China. </br>
* **注意需要手动修改脚本中的全局变量MAC_ADDR**,以区分不同的客户端</br>
* **Note that you need to manually modify the global variable MAC_ADDR in the script**, to differentiate between different clients. </br>
* **按住空格键发起对话**</br>
* **Hold down the space bar to start a conversation**

**测试使用的python 版本为3.12(其它python3应该也可以,没做测试)**</br>
**The python version used for the test is 3.12 (other python3 should also work, no tests)**

## windows需要安装依赖
Windows requires installation dependencies</br>
* pip 安装依赖模块</br>
* Install dependency modules using PIP
```python
pip3  install -r requirements.txt
```
* 将opus.dll拷贝到至C:\Windows\System32目录中</br>
* Copy **opus.dll** to the C:\Windows\System32

## 启动命令
Start command (In Windows CMD or Linux/Mac Terminal)</br>
```python
python py-xiaozhi.py
```

（正片开始doge）</br>
Start here↓

## 更新了什么？
***What's new?*** </br>
* main分支可用于Linux。行空板自带Linux操作系统和python环境，理论上本项目可以用于行空板的Linux操作系统。</br>
* The main branch is available for Linux use. The Unihiker comes with Linux operating system and python environment, and theoretically this project can be used for the Linux operating system of the Unihiker.</br>
* 主要源代码来源于 DFRobot社区 云天 [**原帖**](https://mc.dfrobot.com.cn/thread-324368-1-1.html)</br>
* The main source code is from the DFRobot community. [**Original post**](https://mc.dfrobot.com.cn/thread-324368-1-1.html)</br>
* 源代码对行空板做了适配与GUI界面，激活对话方式有4种。本分支仅收录其中一种：按键，其余3种请移步至原帖。</br>
* The source code adapts the Unihiker and add a GUI, and there are 4 ways to activate the dialogue. This branch only includes one of them: buttons, and the other three types please move to the original post.</br>
* 文件中的**speaker.py**为没有扬声器的用户提供了使用[DFR0760 离线语音合成模块](https://www.dfrobot.com.cn/goods-3014.html)作为替代品的方案</br>
* The **speaker.py** in the file provides an alternative to using the [Gravity: Text to Speech Voice Synthesizer Module V2.0 for Arduino and ESP32](https://www.dfrobot.com/product-2234.html) for users who do not have speakers

## 如何使用
***How to use***</br>
* 按下A键开始讲话，按下B键结束。</br>
* Press the A button to start speaking and the B button to end.</br>
* 如果使用语音合成模块，参考接线图：</br>
* If using the speech synthesis module, refer to the wiring diagram:</br>
[![1.png](https://i.postimg.cc/FzR35XQN/1.png)](https://postimg.cc/gXCn85JT)
* 使用IO扩展板的接线：</br>
* Using the I/O expansion:</br>
[![image.png](https://i.postimg.cc/K88BX1dX/image.png)](https://postimg.cc/56D6L24p)
