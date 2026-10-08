# 视觉语言动作 VLA

[返回主页](../README.md)

| 成果 | 平台 / 设置 | 内容 |
| --- | --- | --- |
| 开源 VLA 部署与任务微调 | OpenVLA、π0、SmolVLA 等 | 语言指令驱动抓放、抽屉操作、组合任务 |
| CR-VLA | 仿真与 AgileX 实机，受限带宽 | [框架、基准测试与实机结果](bandwidth-robust-control.md) |

## 机械臂任务演示

| 语言任务 | 动态演示 |
| --- | --- |
| 打开抽屉，将茄子放在抽屉上方第一层小平台 | ![抽屉操作 GIF](../assets/research/vla-drawer.gif) |
| 将杯子放入碗中，再将整体放在盘子上 | ![餐具组合操作 GIF](../assets/research/vla-tableware.gif) |
| 将香蕉放入白色盘子 | ![香蕉操作 GIF](../assets/research/vla-banana.gif) |

<sub>来源：展示 PPT 第 23 页。PPT 未逐段标注演示所用模型，这里不作额外归属。</sub>

## CR-VLA：压缩鲁棒远程部署

![CR-VLA 原始算法框架](../assets/research/crvla-framework.png)

| 测试设置 | 代表结果 |
| --- | --- |
| LIBERO 波动带宽 | Spatial 97.7%、Object 99.2%、Goal 95.9%、Long 87.6% |
| CALVIN 波动带宽 | 五步成功率 56.9%，平均完成长度 3.758 |
| AgileX 实机波动带宽 | 四任务成功率 80% / 65% / 60% / 60% |

![远程操作场景与压缩输入对比](../assets/research/crvla-real-results.png)

[完整 LIBERO、CALVIN、实机对比表 →](bandwidth-robust-control.md)

<sub>来源：展示 PPT 第 25–26 页及所提供 CR-VLA 论文。</sub>
