# 数据资源

围绕机器人多模态场景感知，整理仿真与真实环境中的传感器数据资源，为场景解析和具身算法验证提供数据基础。

## Isaac Sim 仿真多模态数据集

基于 NVIDIA Isaac Sim 与 GRUtopia 场景资源构建，使用 Unitree G1 仿真平台采集多模态观测。

| 项目 | 内容 |
|---|---|
| 仿真平台 | NVIDIA Isaac Sim |
| 场景资源 | GRUtopia |
| 机器人 | Unitree G1（仿真） |
| 传感器 | RGB-D 相机、Ouster OS0 LiDAR |
| 数据模态 | RGB、深度、点云、分割标注 |
| 场景与规模 | 阅览室、幼儿园、居家等室内场景；现有材料约 15,000 个实例级对象 |
| 数据集入口 | [XDU Embodied AI Lab 在 ModelScope 的数据集列表](https://www.modelscope.cn/profile/XDUEaiLAB?tab=dataset) |

## RC-MVSP

**全称：** Robot-Centric Multimodal Video Scene Parsing

面向机器人中心的多模态视频场景解析，提供传感器对齐的时序观测与语义标注。

| 项目 | 内容 |
|---|---|
| 数据规模 | 1,000 段视频、100,532 帧 |
| 类别数量 | 200 个语义类别 |
| 数据模态 | 对齐的 RGB-D、点云与 IMU |
| 标注 | 现有材料报告密集标注帧率为 20 FPS |
| 真实采集设备 | RealSense D435i、Leishen C16 LiDAR |
| 图像分辨率 | RGB 与深度为 1280×720 |
| 数据集入口 | [XDU Embodied AI Lab 在 ModelScope 的数据集列表](https://www.modelscope.cn/profile/XDUEaiLAB?tab=dataset) |

## 数据使用信息

ModelScope 链接当前指向实验室数据集列表。正式名称、版本、许可、下载方式、数据划分与引用格式以具体数据卡为准；补充数据前请核对对应数据卡内容。
