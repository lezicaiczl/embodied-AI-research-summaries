# BudVLN

**论文标题：** *Nipping the Drift in the Bud: Retrospective Rectification for Robust Vision-Language Navigation*

## 研究问题

在线导航中的小偏差可能逐步累积。论文指出，直接让智能体从偏离轨迹的状态学习恢复动作，可能产生与原始语言指令语义不一致的监督信号。

## 方法概览

- 从当前策略的在线轨迹中识别偏离情况。
- 回到最近的有效历史状态，重新锚定语言指令与导航状态。
- 通过反事实回溯和决策条件监督合成纠正轨迹。
- 按任务难度选择群组相对策略优化（GRPO）或监督微调（SFT）。

## 实验材料

附件列出 R2R-CE 与 RxR-CE 的 Val Unseen 结果，并展示了基线与 BudVLN 的路径对比。现有页面提到该方法改善偏离后的纠错表现。完整指标、训练细节和数值需对照论文原文补充。

> 以上是论文材料的概述，不代表本仓库完成了复现。

## 论文与代码

- 论文主页：[BudVLN 项目页](https://6zyyy.github.io/BudVLN/)
- 论文：[arXiv:2602.06356](https://arxiv.org/abs/2602.06356)
- 官方代码：项目页当前标注为 Coming Soon，尚未公开。
- 作者：Gang He、Zhenyang Liu、Kepeng Xu、Li Xu、Tong Qiao、Wenxin Yu、Chang Wu、Weiying Xie。
- 机构：西安电子科技大学；西南科技大学。
- 发表信息：项目页提供 arXiv 预印本信息，正式发表状态以作者后续更新为准。
