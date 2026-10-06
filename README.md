# Embodied AI Research Showcase

具身智能方向的研究展示仓库，当前整理多模态感知、视觉语言导航（VLN）与视觉语言动作（VLA）相关数据集和论文。内容依据已有介绍材料编写，后续可继续补充论文、实验、代码和演示视频。

> **当前版本：展示初稿。** 部分论文和数据集条目仍待补充。论文中的实验结果如有引用，会明确标注为原论文结果；本仓库暂不声称完成了代码复现。

## 研究方向

| 方向 | 当前收录 | 简介 |
|---|---|---|
| [多模态感知](multimodal-perception/README.md) | 2 个数据集、2 篇论文（1 篇待补充） | 面向机器人场景解析，整理仿真与真实环境中的 RGB、深度、点云及 IMU 数据，并关注时序几何建模。 |
| [VLA](vla/README.md) | 2 篇论文（1 篇待补充） | 关注视觉、语言与动作的联合建模，以及受限带宽下的远程机器人操作。 |
| [VLN](vln/README.md) | 2 篇论文 | 关注机器人如何依据自然语言指令在连续环境中导航，以及在线纠错、分布偏移与物理可执行性问题。 |

## 数据集

### 仿真多模态数据集

基于 NVIDIA Isaac Sim 与上海人工智能实验室的 GRUtopia 场景资源构建。介绍材料提到室内等代表性场景、约 15,000 个实例级对象，以及 RGB、深度、点云和分割标注；仿真采集平台为 Unitree G1，配置 RGB-D 相机与 Ouster OS0 LiDAR。具体数据集名称、统计口径和下载条目待与 ModelScope 页面核对。

### RC-MVSP

Robot-Centric Multimodal Video Scene Parsing 数据集。论文材料报告包含 1,000 段视频、100,532 帧、200 个类别，提供对齐的 RGB-D、点云与 IMU 数据，标注帧率为 20 FPS。真实数据采集说明使用 RealSense D435i 与 Leishen C16 LiDAR，RGB/深度分辨率为 1280×720。

> 仓库中数据集介绍依据现有材料整理。数据规模、传感器配置、许可和下载方式以数据集官方页面为准。

## 论文

- **GDAFormer**：几何引导可变形注意力，用于机器人中心的多模态视频全景分割，并介绍 RC-MVSP 数据集。见 [论文介绍](multimodal-perception/gdaformer.md)。
- **VLN / BudVLN**：通过回溯校正缓解语言指令与偏离状态之间的监督错位。见 [论文介绍](vln/budvln.md)。
- **VLN / VeSTA**：揭示仿真接触语义掩盖的物理可执行性差距，并通过轨迹分布对齐与风险感知候选选择降低碰撞。见 [论文介绍](vln/vesta.md)。
- **VLA / CR-VLA**：在压缩视觉输入下恢复特征并提升远程操作鲁棒性。见 [论文介绍](vla/cr-vla.md)。
- 其余两篇论文：先保留展示位置，待补充标题和材料。

## 数据集主页

[XDU Embodied AI Lab 在 ModelScope 的数据集主页](https://www.modelscope.cn/profile/XDUEaiLAB?tab=dataset)

## 内容说明

- 这是论文与数据集的学习、整理和展示页面，不代表所有项目代码均已公开。
- 论文作者、发表状态、代码地址和正式数据集卡片等信息待核对后补入。
- 论文图片、数据样例和第三方材料应遵循各自的版权与使用许可；本仓库初稿不复制原论文配图或数据文件。

## 目录

```text
.
├── README.md
├── datasets/
│   └── README.md
├── multimodal-perception/
│   ├── README.md
│   ├── gdaformer.md
│   └── paper-2-TODO.md
├── vla/
│   ├── README.md
│   ├── cr-vla.md
│   └── paper-2-TODO.md
└── vln/
    ├── README.md
    ├── budvln.md
    └── vesta.md
```
