# 赛题一：遗失宠物的智能寻找

伴随着人们物质生活水平的提高，越来越多的家庭选择饲养小动物，它们不仅是家庭的宠物，很多人也将他们视作家庭成员之一，给予百般宠爱和呵护。然而即便如此，意外还是难免发生——宠物的意外走失给很多宠物家庭带来了困扰，满大街发传单、贴广告不仅浪费时间，成效也甚微。

如果可以通过人工智能的方式解决这一难题，相信将成为不少养宠家庭的福音——“狗脸识别”、智能追踪设备、“离家出走”路线预测……

请以“遗失宠物的智能寻找”为主题，利用人工智能技术完成一款产品（软件或硬件）的开发。

---

* 作品介绍：

  猫是人们最喜欢的宠物之一，很多人都拜倒在了它们的魅力之下，成为了一名光荣的铲屎官。那么，如果你的小主子不幸走失了，你一定会心机如焚的去寻找。本项目致力解决这一问题，希望可以快速的在图片和视频中框选出猫咪的位置，从而发现猫咪的运动轨迹，最终成功接小主子回家。另外，本项目还可以从图片中选出猫脸所在的区域，将该区域放入SVM分类器中进行训练，进而对猫脸进行识别，这样就可以通过监控路线自动的检测你的猫咪的所在位置，大大减少了人工的工作量。

  本项目使用imglab对猫脸图片进行标注

* 作品截图：

  猫脸检测效果图一：

  ![1](https://github.com/CCCGX/aws-hackathon-2020/blob/master/1%20%E9%81%97%E5%A4%B1%E5%AE%A0%E7%89%A9%E7%9A%84%E6%99%BA%E8%83%BD%E5%AF%BB%E6%89%BE/%E7%8C%AB%E8%84%B8%E6%A3%80%E6%B5%8B%E5%8F%8A%E8%AF%86%E5%88%AB%20-%20Rainbow/res1.png?raw=true)

  猫脸检测效果图二：

  ![2](https://github.com/CCCGX/aws-hackathon-2020/blob/master/1%20%E9%81%97%E5%A4%B1%E5%AE%A0%E7%89%A9%E7%9A%84%E6%99%BA%E8%83%BD%E5%AF%BB%E6%89%BE/%E7%8C%AB%E8%84%B8%E6%A3%80%E6%B5%8B%E5%8F%8A%E8%AF%86%E5%88%AB%20-%20Rainbow/res2.png?raw=true)

  猫脸检测效果图三：（可以很好的识别出猫和狗的区别，opencv自带的猫脸检测就不能很好的做到这一点）

  ![3](https://github.com/CCCGX/aws-hackathon-2020/blob/master/1%20%E9%81%97%E5%A4%B1%E5%AE%A0%E7%89%A9%E7%9A%84%E6%99%BA%E8%83%BD%E5%AF%BB%E6%89%BE/%E7%8C%AB%E8%84%B8%E6%A3%80%E6%B5%8B%E5%8F%8A%E8%AF%86%E5%88%AB%20-%20Rainbow/res3.png?raw=true)

  猫脸检测效果图四：

  ![4](https://github.com/CCCGX/aws-hackathon-2020/blob/master/1%20%E9%81%97%E5%A4%B1%E5%AE%A0%E7%89%A9%E7%9A%84%E6%99%BA%E8%83%BD%E5%AF%BB%E6%89%BE/%E7%8C%AB%E8%84%B8%E6%A3%80%E6%B5%8B%E5%8F%8A%E8%AF%86%E5%88%AB%20-%20Rainbow/res4.png?raw=true)

  猫脸识别效果图一：

  ![4](https://github.com/CCCGX/aws-hackathon-2020/blob/master/1%20%E9%81%97%E5%A4%B1%E5%AE%A0%E7%89%A9%E7%9A%84%E6%99%BA%E8%83%BD%E5%AF%BB%E6%89%BE/%E7%8C%AB%E8%84%B8%E6%A3%80%E6%B5%8B%E5%8F%8A%E8%AF%86%E5%88%AB%20-%20Rainbow/res5.png?raw=true)

* 安装、编译指南：

  1.安装代码运行所需要的环境：

  python3

  并使用以下命令安装dlib：
  
  ```python
  pip install dlib-19.17.99-cp37-cp37m-win_amd64.whl
  ```
  并安装其他依赖环境
  
   ```python
  pip install numpy
  pip install matplotlib
  pip install scikit-learn
  pip install opencv-python
   ```
  3.使用juputer note打开cat1.ipynb，依次运行每个单元格进行猫脸检测
  
  4.使用juputer note打开cat2.ipynb，依次运行每个单元格进行猫脸识别
  
* 团队介绍：

  团队名称：Rainbow

  团队成员：曹光旭

  联系方式：13953006634

* 使用到的 AWS 技术：

  使用SageMaker提供的GPU对模型进行训练。
