# 多模态感知

[返回主页](../README.md) · [开放数据集](../datasets/README.md)

| 成果 | 输入 / 任务 | 图表详情 |
| --- | --- | --- |
| RoboMM-Syn / RC-MVSP | 仿真与真实 RGB-D、点云、场景标注 | [数据样例与统计](../datasets/README.md) |
| GDAFormer | RGB、深度、相机位姿；视频场景解析 | [框架、结果表与动画](robot-video-scene-parsing.md) |
| MDV-Fusion | 退化红外与可见光视频；视频融合 | [框架与融合结果](degraded-video-fusion.md) |

## 数据集

![多模态视频数据样例](../assets/research/rc-mvsp-examples.png)

| 数据集 | 规模 | 下载 |
| --- | --- | --- |
| RoboMM-Syn | 约 15,000 个实例级对象 | [ModelScope](https://www.modelscope.cn/datasets/XDUEaiLAB/RoboMM-Syn) |
| 真实机器人多模态感知数据集 | 1,000 视频 / 100,532 帧 / 200 类 | [ModelScope](https://www.modelscope.cn/datasets/XDUEaiLAB/Robot_multimodal_perception_dataset) |

## GDAFormer：几何引导视频场景解析

![GDAFormer 原始算法框架](../assets/research/gdaformer-framework.png)

| 室内动态结果 | 室外动态结果 |
| --- | --- |
| ![室内分割 GIF](../assets/research/indoor-parsing.gif) | ![室外分割 GIF](../assets/research/outdoor-parsing.gif) |

[完整实验对比 →](robot-video-scene-parsing.md)

## MDV-Fusion：多退化视频融合

![MDV-Fusion 论文框架图](../assets/research/mdv-framework.png)

![MDV-Fusion 多退化场景融合结果](../assets/research/mdv-comparison.png)

[完整指标表与实验设置 →](degraded-video-fusion.md)
