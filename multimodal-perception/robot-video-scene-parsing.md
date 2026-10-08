# GDAFormer：几何引导视频场景解析

[返回多模态感知](README.md) · [实验室主页](../README.md)

| 输入 | 关键模块 | 输出 |
| --- | --- | --- |
| RGB 视频、深度、相机位姿 | 时序几何编码、G2-DAB 几何引导可变形注意力 | 视频语义 / 全景分割 |
| 多尺度视觉特征 | 动态采样与跨帧特征聚合 | 时序场景解析结果 |

## 算法框架

![GDAFormer 原始框架图](../assets/research/gdaformer-framework.png)

## 数据与实验对比

![RC-MVSP 场景示例](../assets/research/rc-mvsp-examples.png)

![数据集统计对比](../assets/research/dataset-comparison.png)

![GDAFormer 原始实验结果表](../assets/research/gdaformer-results.png)

## 动态结果

| 室内场景 | 室外场景 |
| --- | --- |
| ![室内动态分割](../assets/research/indoor-parsing.gif) | ![室外动态分割](../assets/research/outdoor-parsing.gif) |
