EXAPUNKS-Manual-Localization-Chinese
====================================
steam编程类游戏EXAPUNKS的文档翻译，商店链接：[EXAPUNKS](https://store.steampowered.com/app/716490/ "EXAPUNKS")  
该文档在游戏内以杂志`TRASH WORLD NEWS`的形式出现，pdf见游戏根目录下/Content/manual，作者提供了三种格式以供直接阅读或打印成小册子。

杂志分为上下册，内容按顺序分别为  
* 游戏世界观介绍
* 教程
* 代码文档
* 每关对应的背景故事

目前已翻译完前三部分，后面的背景故事将会慢慢更新。  
本项目出于纯粹个人爱好，练练英语的同时熟悉一下markdown排版。一切更新随缘:kissing_closed_eyes:。
****
## 目录
* [上册](#上册)
	* [(02)TRASH WORLD MANIFESTO](#（02）TRASH&ensp;WORLD&ensp;MANIFESTO)
	* [(05)基于EXA的分布式网络编程](#（05）基于EXA的分布式网络编程)
	* [(06)主机，连接，文件以及硬件寄存器](#主机，连接，文件以及硬件寄存器)
		* [主机](#主机)
		* [连接](#连接)
		* [文件](#文件)
		* [硬件寄存器](#硬件寄存器)
	* [(08)教程](#教程)
		* [教程1：基础](#教程1：基础)
		* [教程2：文件读写](#教程2：文件读写)
		* [教程3：EXA间通信](#教程3：EXA间通信)
		* [教程4：条件与循环](#教程4：条件与循环)
	* [(12)RUNTIME ERRORS](#RUNTIME&ensp;ERRORS)
	* [(14)EXA语言参考文档](#EXA语言参考文档)
****
# 上册
## （02）TRASH&ensp;WORLD&ensp;MANIFESTO
&emsp;&emsp;欢迎阅读《TRASH WORLD NEWS》。你可能会好奇，为什么在这个数字时代我们还要发行一本纸质杂志呢？答案很简单：我们需要一块不受计算机干扰的净土，来分享有关于计算机系统和网络的重要敏感信息。  
&emsp;&emsp;你最近注意到了吗？无论何时何地，总有无数的计算机在幕后帮你做出决定。这些被当权者们设计并制造出来的电脑程序，正在背后估算着我们的价值，使我们可以为其所用，而这种行为似乎已经被大众接受并视作常态。  
&emsp;&emsp;电脑本身只是工具，应当为我们所用，这就是我们必须反抗的理由。我们要用知识和工具来武装自己，来反抗这股愈演愈烈的浪潮。下次再有计算机将我们视作棋子的时候，我们可以通过编写程序来破坏它们，让它们认识到人类才是这个世界的主宰。

**我们既是人类，也是黑客**

&emsp;&emsp;本杂志将会一步步地介绍渺小但是强大的EXA，这项技术在无人察觉的情况下已经统治了世界。从游戏控制台到大公司的服务器，几乎任何东西都已经离不开它了。  
&emsp;&emsp;我们会带你了解事情的来龙去脉，并让你很快上手编程，即便你以前从没接触过代码。
&emsp;&emsp;我们也会刊登来自全世界各个领域的黑客的研究成果，比如数据存储格式以及最新的网络研究进展等等。  
&emsp;&emsp;最后再提一句，本杂志刊登了某个生物学家最近关于“噬菌体”的研究报告，她在她的空闲时间进行了该项研究并分享给了我们。我敢保证这绝对是你在其他地方都找不到的绝密资料。
 
**黑客精神永存 Ghast留**


## （05）基于EXA的分布式网络编程
&emsp;&emsp;想要摆脱电脑的控制，第一步就是要学会如何去使用它们，这就需要学会用EXA编程。  
**EXA是什么？**  
&emsp;&emsp;EXA是可执行代理的缩写(EXecution Agent)。


