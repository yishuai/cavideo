class: middle, center

### 大数据时代下人工智能技术的应用与创新

# 应用与创新（视觉）

陈一帅

[yschen@bjtu.edu.cn](mailto:yschen@bjtu.edu.cn)

北京交通大学电子信息工程学院

.footnote[呼局中青班]
---
# 内容
- .red[背景]
- 目标检测和识别
- 图像分割
- 应用
- 应注意的问题
---
# 基本研究问题

- 目标检测、分割、识别

- 困难：遮蔽、干扰、噪声

.center[.width-100[![](figures/rail/rail.png)]]

---
# 效果

.center[.width-100[![](../ai/figures/all/retinanet.gif)]]

???
https://towardsdatascience.com/review-retinanet-focal-loss-object-detection-38fba6afabe4
---
# 图像分割
- Object Segmentation
- 从图形中提取对象的轮廓

.center[.width-80[![](../ai/figures/all/dog_segment.jpg)]]
---
# 语义分割

- 同一类的多个物体可以分在一起
- 和另一类物体分开

<br>
.center[.width-100[![](../ai/figures/all/cls_4_2.jpg)]]

---
class: middle, center
# 效果（2017）
<!-- <video width="700" controls>
    <source src="./video/seg.mp4" type="video/mp4">
</video> -->
<div class="aspect-ratio">
  <iframe src="//player.bilibili.com/player.html?aid=54907833&cid=96023749&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
</div>

---
# 实例分割

- 同一类的多个物体，互相也要分开

<br>
.center[.width-100[![](../ai/figures/all/cls_4_3.jpg)]]

---
# 效果

<br>
.center[.width-100[![](../ai/figures/all/segmentationresults2.jpg)]]
---
# 效果

- Mask RCNN效果

.center[.width-100[![](../ai/figures/all/maskrcnn.gif)]]
---
# 内容
- 背景
- 目标检测和识别
- 图像分割
- .red[应用]
- 应注意的问题
---
class: center, middle

# 应用
---
# 工业机器人
.center[.width-100[![](../ai/figures/all/maskrcnn-video.gif)]]
---
# 3D建筑物
.center[.width-100[![](../ai/figures/all/maskrcnn-project_3dbuildings.png)]]
---
# 照片特效
.center[.width-100[![](../ai/figures/all/maskrcnn-project_shiny1.jpg)]]

???
https://github.com/matterport/Mask_RCNN
---
# 人脸检测
.center[.width-90[![](../ai/figures/all/face-challenge.png)]]
---
# 人脸识别
- 美国马里兰州枪击事件，人脸识别技术找出了嫌犯
- 流行歌星泰勒·斯威夫特，演唱会上过滤狂热粉丝和跟踪狂
- 收容所追踪收容所和避难所的使用情况
---
# 姿势检测与识别

.center[.width-100[![](../ai/figures/all/pose.jpg)]]
---
# 情感识别

.center[.width-100[![](../ai/figures/all/emotion.jpg)]]
---
class: middle, center
# 交通流量计数

<!-- <video width="700" controls>
    <source src="./video/traffic-count.mp4" type="video/mp4">
</video> -->
<div class="aspect-ratio">
  <iframe src="//player.bilibili.com/player.html?aid=54907357&cid=96026074&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
</div>
---
class: middle, center
# 交通流量计数

<!-- <video width="700" controls>
    <source src="./video/traffic-count2.mp4" type="video/mp4">
</video> -->
<div class="aspect-ratio">
  <iframe src="//player.bilibili.com/player.html?aid=54907492&cid=96024461&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
</div>
---
# 交通信号识别

.center[.width-90[![](../ai/figures/all/traffic-challenge.png)]]
---
class: middle, center
# 铁轨检测
<!-- <video width="700" controls>
    <source src="./video/railway.mp4" type="video/mp4">
</video> -->
<div class="aspect-ratio">
  <iframe src="//player.bilibili.com/player.html?aid=54907949&cid=96020491&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
</div>
---
class: middle, center
# 道口监控
<!-- <video width="700" controls>
    <source src="./video/crossing.mp4" type="video/mp4">
</video> -->
<div class="aspect-ratio">
  <iframe src="//player.bilibili.com/player.html?aid=54906667&bvid=BV1F4411T7FZ&cid=96023038&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
</div>

---
# 文本识别
.center[.width-100[![](../ai/figures/all/text-challenge.png)]]
---
# 清晰度增强
.center[.width-100[![](../ai/figures/all/vision_translation.jpg)]]
---
# 去噪

.center[.width-80[![](../ai/figures/all/denoising.jpg)]]
---
# 图像转换
- 图像还原、渲染、着色
- 地图提取、场景转换

<br>
.center[.width-100[![](../ai/figures/all/pix2pix.jpg)]]
---
# 图像理解

图像 - 问答 - 文本描述

.center[.width-100[![](../ai/figures/all/nlp_vision.jpg)]]
---
class: middle,center
# 实时图像理解（2015）
<!-- <video width="700" controls>
    <source src="./video/caption.mp4" type="video/mp4">
</video> -->
<div class="aspect-ratio">
  <iframe src="//player.bilibili.com/player.html?aid=54906321&cid=96021881&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
</div>
<!-- .center[.width-100[![](../ai/figures/all/caption1.jpg)]] -->
<!-- .center[.width-100[![](../ai/figures/all/captioning_model.jpg)]] -->

---
# 内容
- 背景
- 目标检测和识别
- 图像分割
- 应用
- .red[应注意的问题]
---
# 应注意的问题
- 准确率
- 隐私保护
- 公平
---
# 准确率问题
- 2018年7月，“美国公民自由联盟”测试了亚马逊的人脸识别系统
- 将535名国会议员面孔，对照25000张公开的警方嫌疑犯照片。有28个无辜的国会议员被认成了嫌疑犯
- 对于皮肤较黑的人和女性，人脸识别通常不太准确。所有国会议员的错误率是5.2%，非白人国会议员错误率达39%
---
# 识别错误付出生命代价
特斯拉自动驾驶系统未成功识别出白色货车

.center[.width-100[![](../ai/figures/all/crash.jpg)]]
---
# 识别错误付出生命代价
.center[.width-50[![](../ai/figures/all/crash2.jpg)]]
---
# 识别错误引起民愤
把人识别成大猩猩

.center[.width-80[![](../ai/figures/all/gorillas.jpg)]]
---
# 隐私保护
- 2019年5月14日，旧金山城市监督委员会以8票对1票通过法令，禁止城市工作人员购买和使用人脸识别技术
- “人脸识别技术危害公民权利和公民自由的倾向大大超过了其声称的好处，这项技术将加剧种族不平等，并威胁到我们不受政府长期监控的生活能力”
---
# 小结
- 困难
- 目标检测和识别
- 图像分割
- 应用
- 应注意的问题
  - 准确率、隐私保护、公平