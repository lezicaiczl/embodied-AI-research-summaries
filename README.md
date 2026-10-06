# Embodied AI Research Showcase

具身智能研究与工程成果展示，围绕机器人多模态感知、视觉语言导航（VLN）和视觉语言动作（VLA），建设数据资源、算法方法与真实机器人验证能力。

<p align="center">
  <a href="multimodal-perception/README.md">多模态感知</a> &middot;
  <a href="vln/README.md">视觉语言导航</a> &middot;
  <a href="vla/README.md">视觉语言动作</a> &middot;
  <a href="datasets/README.md">数据集</a>
</p>

> **项目状态：** 成果展示与资料整理持续更新中。下表概述现有数据、算法和实验验证；数据规模与实验数字依据现有项目材料整理，具体条件见对应方向页面。

## 建设目标

1. 建立覆盖机器人感知、导航和操作的具身智能研究成果展示。
2. 整理仿真与真实环境中的多模态机器人数据，支持场景解析和算法评估。
3. 面向真实部署中的关键问题，提升机器人对复杂视觉、自然语言指令和受限通信条件的适应能力。
4. 通过仿真基准和机器人实验检验方法在连续环境中的执行表现。

## 已有成果

| 方向 | 已形成的能力 | 验证与资源 |
|---|---|---|
| **多模态感知与视频融合** | 建设仿真与真实多模态数据资源；研发几何引导场景解析，以及面向多种退化的红外-可见光视频融合方法。 | 覆盖 RGB、深度、点云、IMU 与分割标注；在场景解析和视频融合基准上评估。详见[感知与融合成果](multimodal-perception/README.md)。 |
| **视觉语言导航（VLN）** | 形成在线轨迹纠偏训练和局部运动可执行性优化方法，提升连续导航中的指令跟随与碰撞规避能力。 | 在 R2R-CE、RxR-CE 等基准及 Unitree Go2 室内任务上验证。详见[VLN 成果](vln/README.md)。 |
| **视觉语言动作（VLA）** | 形成面向低带宽远程机器人的压缩鲁棒视觉理解与动作生成方案。 | 在 LIBERO、CALVIN 及 AgileX 机械臂远程操作场景评估。详见[VLA 成果](vla/README.md)。 |

## 数据资源

| 数据资源 | 内容概览 | 数据集入口 |
|---|---|---|
| **Isaac Sim 仿真多模态数据集** | 基于 NVIDIA Isaac Sim 与 GRUtopia 场景资源，使用 Unitree G1 仿真平台采集 RGB-D、点云和分割标注，覆盖多类室内场景与约 15,000 个实例级对象。 | [XDU Embodied AI Lab 的 ModelScope 数据集列表](https://www.modelscope.cn/profile/XDUEaiLAB?tab=dataset) |
| **RC-MVSP** | Robot-Centric Multimodal Video Scene Parsing，包含 1,000 段视频、100,532 帧和 200 个类别，提供对齐的 RGB-D、点云与 IMU 数据。 | [XDU Embodied AI Lab 的 ModelScope 数据集列表](https://www.modelscope.cn/profile/XDUEaiLAB?tab=dataset) |

更多数据说明、传感器配置与数据卡信息见[数据集目录](datasets/README.md)。

## 研究与验证能力

| 能力领域 | 覆盖内容 |
|---|---|
| **机器人多模态感知** | RGB、深度、点云、IMU 的时序融合；几何先验编码；视频语义与全景场景解析。 |
| **连续视觉语言导航** | 自然语言指令跟随；在线策略训练；历史有效状态重锚定；严格接触条件下的局部轨迹选择。 |
| **远程视觉语言动作** | 压缩退化先验提取；视觉表征恢复；压缩先验注入动作模型；波动带宽下的闭环操作。 |
| **实验平台** | Isaac Sim 仿真；R2R-CE、RxR-CE、LIBERO、CALVIN 基准；Unitree Go2 和 AgileX 机械臂实机验证。 |

## 目录

```text
.
├── README.md
├── datasets/
│   └── README.md
├── multimodal-perception/
│   ├── README.md
│   ├── robot-video-scene-parsing.md
│   └── degraded-video-fusion.md
├── vla/
│   ├── README.md
│   └── bandwidth-robust-control.md
└── vln/
    ├── README.md
    ├── online-nav-training.md
    └── collision-aware-navigation.md
```

## 成果说明

- 本仓库用于展示实验室已有研究方向、数据资源、算法方法与验证结果。
- 实验数字反映现有项目材料所报告的结果；不同平台、基准和测试条件应结合对应页面理解。
- ModelScope 入口指向实验室数据集列表；具体数据集名称、许可、版本与下载说明以各数据卡为准。
- 公开数据资源不代表相关算法代码或全部实验资产均已开放。
