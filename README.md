    
    这是中文版本的介绍
# 价格追踪器
   这是PPT的地址: [ppt](https://github.com/AnonymousAudience/PriceTracker/blob/master/PriceTracker%E9%A1%B9%E7%9B%AE%E7%AE%80%E4%BB%8B.pptx)  
   
   这是演示视频的地址:[视频]()  
   
                                           
### 项目简介
#### 功能介绍
这是一款轻便、小巧的价格追踪器，它能够依照用户输入的商品网址来查询指定商品的历史价格信息并且自动生成并存储历史价格的图像。  

#### 主要面向人群
经常并且习惯在电商平台上购买商品的有着**了解商品以往价格来帮助决策的需求**的用户。  

#### 使用方法
1.首先下载打开我们软件的压缩包（名为PriceTracker2），进入到以下目录界面：（也可以先将整个文件进行解压再操作）  

（在此文件夹中同时包含了软件的源码，可以提供给有需求的用户修改软件XD）  

![使用方法](https://github.com/AnonymousAudience/PriceTracker/blob/master/Pics_Used/a.jpg)

2.在Publish文件夹中找到我们的目标：PriceTracker.exe  

PriceTracker.exe是可执行程序，无需安装，点开即可运行。
在运行之前我们可以在相同的目录下找到ReadmeBeforeUse.txt，里面有些使用该软件的注意事项，建议先进行阅读。  
![建议阅读](https://github.com/AnonymousAudience/PriceTracker/blob/master/Pics_Used/b.jpg)


> 另外我们给出编译源代码文件方法：    

 **打开压缩包中的aardio.7z，打开开发软件aardio.exe （无需安装，可直接打开）。在aardio中打开工程文件 default.aproj，按F5键即可运行。**
#### 界面初识
以下就是我们这款小型软件的主要界面，上面有相关的文字提示。  
点击不同的按钮即可弹出相应的文本介绍。  
**黄色区域为输入商品网址区域**，输入完成后，点击“Confirm”按钮软件即可正常工作。  
相关的使用示例在我们的演示视频中会有更详细的说明。
![界面初识](https://github.com/AnonymousAudience/PriceTracker/blob/master/Pics_Used/c.png)

#### 原理介绍
该项目使用的是一门目前比较简单的的语言 aardio  
（我们在此给出aardio的官网：[arrdio官网](http://www.aardio.com/)，方便您的进一步了解）

   >起初，我们的设计构想是利用python语言对各电商平台的价格数据进行实时爬取，但是由于各电商平台对自家的价格数据都进行了反爬取的保护措施（尤其是对于历史价格而言）。而且，淘宝天猫如今更是要求用户在浏览商品前进行登陆操作。尽管这个问题用python可以解决（需要使用到用户电脑上的cookies），但这多少也造成了不方便。  
  
   >所以，我们转变了思路，找到了一些原本就具有各电商平台商品历史价格数据的网站，又注意到这些网站上本身已经生成了图像，因此我们可以对这些网站直接进行截图处理，等到我们想要的结果完成目标。

   >在项目源代码中，我们主要调用了类似python中的webdriver的自动化测试脚本，用户输入网页并且在点击confirm按钮之后，软件会自动打开Chrome浏览器并打开相应的历史价格网站，并且在生成本地图片后自动关闭测试test窗口，留给用户最直接的使用体验。

### 基本内容介绍完毕，感谢您的阅读！

  
----------------------------------------------------------------------------------------

      
      
##### This is an introduction of the English version.

# Price Tracker

 This is the where the ppt is stored: [ppt](https://github.com/AnonymousAudience/PriceTracker/blob/master/PriceTracker%E9%A1%B9%E7%9B%AE%E7%AE%80%E4%BB%8B.pptx)  
                                           
### Project Description
#### Features
This is a lightweight, compact price tracker that queries historical price information for a given item based on the product URL entered by the user and automatically generates and stores an image of the historical price.

#### Main user crowd
Users who are often and accustomed to purchasing goods on an e-commerce platform have users who understand the past price of the product to help make decisions.

#### Instructions
1. First download and open the compression package of our software called  PriceTracker2, enter the following directory interface: (You can also decompress the entire file and then operate)

(In this folder, the source code of the software is also included, which can be provided to the user in need to modify the software XD)

![How to use](https://github.com/AnonymousAudience/PriceTracker/blob/master/Pics_Used/a.jpg)

2. Find our target in the Publish folder: PriceTracker.exe  

PriceTracker.exe is an executable program that you can run without having to install it.  
Before running, we can find ReadmeBeforeUse.txt in the same directory.  
There are some precautions for using the software. It is recommended to read it first.
![Recommended reading](https://github.com/AnonymousAudience/PriceTracker/blob/master/Pics_Used/b.jpg)


> In addition, we give the method of compiling the source code file:  

   **Open aardio.7z in the archive and open the development software aardio.exe (you can open it directly without installing it). Open the project file default.aproj in aardio and press F5 to run.**

#### Interface first met
The following is the main interface of our small software, with related text prompts.  
Click on a different button to bring up the corresponding text description.  
**The yellow area is the input product URL area**. After the input is completed, click the “Confirm” button software to work normally.
A related usage example will be explained in more detail in our demo video.    

![First look at the interface](https://github.com/AnonymousAudience/PriceTracker/blob/master/Pics_Used/c.png)

#### Principle introduction
The project uses a relatively simple language aardio  
(We are here to give aardio's official website:[arrdio offical website](http://www.aardio.com/), for your further understanding)  

   > At first, our design concept is to use the Python language to crawl the price data of each e-commerce platform in real time, but because the e-commerce platform has anti-crawl protection measures for their own price data (especially for historical prices) In terms of). Moreover, Taobao Tmall now requires users to log in before browsing the product. Although this problem can be solved with python (requires the use of cookies on the user's computer), this is somewhat inconvenient.  
  
   > So, we changed our mindset and found some websites that originally had historical price data for each e-commerce platform. We also noticed that the images on these websites have already been generated, so we can directly take screenshots of these websites and wait until we The desired result accomplishes the goal.  

   > In the project source code, we mainly call the automated test script similar to webdriver in python. After the user enters the webpage and clicks the confirm button, the software will automatically open the Chrome browser and open the corresponding historical price website, and the test window will automatically closed after generating the local picture, leaving the user with the most direct experience.  

### The basic content is introduced, thank you for your reading!
