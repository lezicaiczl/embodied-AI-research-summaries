# GDAFormer

**论文标题：** *GDAFormer: Geometry-Guided Deformable Attention for Robot-Centric Multimodal Video Panoptic Segmentation*

## 研究问题

机器人平台可同时采集 RGB、深度、点云和位姿等信息，但现有视频场景解析方法常以 RGB 为主；多模态融合方法则较少同时处理时序与几何信息。论文研究如何利用几何先验改善机器人场景中的跨帧多模态解析。

## 方法概览

1. **Temporal Geometry Encoder**：将深度与相机位姿等几何先验编码为紧凑表征。
2. **Geometry-Guided Deformable Attention Block（G2-DAB）**：根据几何特征动态选择时空采样位置，聚合关键区域信息。
3. **视频分割头**：使用融合后的时序多模态特征完成视频全景/语义分割任务。

## 数据集

论文介绍了 **RC-MVSP**，提供 RGB-D、点云和 IMU 对齐数据。材料列出的统计为 1,000 段视频、100,532 帧、200 个类别，密集标注帧率为 20 FPS。

## 实验结果

现有材料中的结果表覆盖 VIPSeg、VSPW 与 RC-MVSP。表格报告 GDAFormer 在几何与多模态设置下取得有竞争力的分割结果；FPS 的测试说明为单张 RTX 4090 上在线网络推理速度，不含离线深度/位姿估计。具体数值建议后续从论文原文表格校对后再录入。

> 以上为对现有介绍材料的整理，不代表本仓库完成了复现。

## 论文与代码

- 论文 PDF / DOI / arXiv：待补充
- 官方代码：待补充
- 项目主页：待补充
- 作者与发表信息：待核对（当前附件中的论文截图显示匿名稿）
