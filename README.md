# 飞桨常规赛：遥感影像地块分割 4月第8名方案

## 项目描述
赛题简介
赛题任务 本赛题旨在对遥感影像进行像素级内容解析，并对遥感影像中感兴趣的类别进行提取和分类，以衡量遥感影像地块分割模型在多个类别（如建筑、道路、林地等）上的效果。

数据说明 本赛题提供了多个地区已脱敏的遥感影像数据，各参赛选手可以基于这些数据构建自己的地块分割模型。

训练数据集文件名称：train_and_label.zip 包含2个子文件，分别为：训练数据集（原始图片）文件、训练数据集（标注图片）文件，详细介绍如下：

训练数据集（原始图片）文件名称：img_train 包含66,653张分辨率为2m/pixel，尺寸为256 * 256的JPG图片，每张图片的名称形如T000123.jpg。

训练数据集（标注图片）文件名称：lab_train 包含66,653张分辨率为2m/pixel，尺寸为256 * 256的PNG图片，每张图片的名称形如T000123.png。 备注： 全部PNG图片共包括4种分类，像素值分别为0、1、2、3。此外，像素值255为未标注区域，表示对应区域的所属类别并不确定，在评测中也不会考虑这部分区域。

测试数据集 测试数据集文件名称：img_test.zip，详细介绍如下： 包含4,609张分辨率为2m/pixel，尺寸为256 * 256的JPG图片，文件名称形如123.jpg。

## 本项目基于PaddleSeg进行训练与推理

## 项目结构
```
-|data
-|work
-README.MD
-1742381.ipynb
```
## 使用方式
A：在AI Studio上[运行本项目](https://aistudio.baidu.com/aistudio/projectdetail/1742381)
