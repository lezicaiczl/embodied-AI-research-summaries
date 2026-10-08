# CR-VLA：压缩鲁棒远程操作

[返回 VLA](README.md) · [实验室主页](../README.md)

*CR-VLA: Compression-Robust Vision-Language-Action models for Remote Deployment*

| 模块 | 作用 |
| --- | --- |
| CPE 压缩先验提取 | 提取受损输入中的压缩退化特征 |
| CAM 压缩感知调制 | 使用压缩先验恢复视觉特征 |
| 重建辅助训练 | 对齐受损输入与目标表征 |
| 压缩先验动作锚定 | 将退化信息引入动作生成 |

## 算法框架

![CR-VLA 原始算法框架](../assets/research/crvla-framework.png)

## LIBERO

![不同传输带宽下 LIBERO 完整结果表](../assets/research/crvla-libero.png)

| 波动带宽 | Spatial | Object | Goal | Long |
| --- | ---: | ---: | ---: | ---: |
| CR-VLA 成功率 | 97.7% | 99.2% | 95.9% | 87.6% |

## CALVIN

![CALVIN 固定带宽结果表](../assets/research/crvla-calvin.png)

![CALVIN 波动带宽及消融实验原表](../assets/research/crvla-calvin-fluct.png)

| 波动带宽 | 1 步 | 2 步 | 3 步 | 4 步 | 5 步 | 平均长度 |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| CR-VLA | 92.2% | 84.4% | 76.0% | 66.3% | 56.9% | 3.758 |

## AgileX 实机结果

![实机任务、动作序列与压缩输入](../assets/research/crvla-real-results.png)

![实机带宽、延迟与成功率原表](../assets/research/crvla-real-table.png)

| 波动带宽 | 香蕉 | 叠盘 | 整理餐具 | 抽屉 | P95 延迟 |
| --- | ---: | ---: | ---: | ---: | ---: |
| Base-Fluct | 55% | 35% | 10% | 15% | 205 ms |
| CR-Fluct | 80% | 65% | 60% | 60% | 214 ms |

| 实机条件 | 配置 |
| --- | --- |
| 平台 | AgileX，6 自由度单臂与夹爪 |
| 视觉 | 主视角与腕部视角，640 × 480，10 Hz |
| 链路 | H.265 / RTP，机器人采集、远端 GPU 推理 |
| 波动带宽 | 链路容量 1.81–3.61 Mbps |
| 评估 | 每任务 20 次 |
