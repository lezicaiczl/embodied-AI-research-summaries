# 数据资源

围绕机器人多模态场景感知，整理仿真与真实环境中的传感器数据资源，为视频场景解析和具身算法验证提供数据基础。两套数据均包括视觉与几何信息，覆盖室内居家场景；真实数据还覆盖城市户外环境。

## Isaac Sim 仿真多模态数据集

基于 NVIDIA Isaac Sim 与 GRUtopia 场景资源构建，使用 Unitree G1 仿真平台采集多模态观测。PPT 中展示的代表性场景包括阅览室、幼儿园和居家环境。GRUtopia（桃源）提供交互式三维场景资源，PPT 介绍其包含 89 个场景和约 10 万个交互环境要素，可用于多场景数据生成并降低真实数据采集成本。

| 项目 | 内容 |
|---|---|
| 仿真平台 | NVIDIA Isaac Sim |
| 场景资源 | GRUtopia |
| 机器人 | Unitree G1（仿真） |
| 传感器 | RGB-D 相机、Ouster OS0 LiDAR |
| 数据模态 | RGB、深度、点云、分割标注 |
| 图像分辨率 | RGB 与深度为 1280×720 |
| 点云 | 每帧平均约 300,000 个三维空间点 |
| 场景与规模 | 阅览室、幼儿园、居家等室内场景；约 15,000 个实例级对象 |
| 数据集入口 | [ModelScope 仿真数据集](https://www.modelscope.cn/datasets/XDUEaiLAB/RoboMM-Syn) |

## RC-MVSP

**全称：** Robot-Centric Multimodal Video Scene Parsing

面向机器人中心的多模态视频场景解析，提供传感器对齐的时序观测与语义标注。采集场景覆盖室内家居，也包括街道、小区、学校、公园等城市户外环境。

| 项目 | 内容 |
|---|---|
| 数据规模 | 1,000 段视频、100,532 帧 |
| 类别数量 | 200 个语义类别 |
| 数据模态 | 对齐的 RGB-D、点云与 IMU |
| 标注 | 现有材料报告密集标注帧率为 20 FPS |
| 真实采集设备 | RealSense D435i、Leishen C16 LiDAR |
| 图像分辨率 | RGB 与深度为 1280×720 |
| 点云 | 每帧平均约 100,000 个三维空间点 |
| 数据集入口 | [ModelScope 真实多模态数据集](https://www.modelscope.cn/datasets/XDUEaiLAB/Robot_multimodal_perception_dataset) |

## 数据使用信息

以上链接分别指向仿真数据集与真实多模态数据集的数据卡。正式名称、版本、许可、下载方式、数据划分与引用格式以对应数据卡为准。
