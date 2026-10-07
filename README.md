# Sink-Physics · 汇物理

**《The Sink Is a Flattening: Charge, Antigravity, and the Photon in Flowing Space》**
**《汇即抹平：流动空间中的电荷、反引力与光子》**

> 站在山顶，你看不到山。
> —— 弗兰克·赫伯特《沙丘》

## 这是什么

本文是 flowing-space 框架（`logos-42/Hibs-Physics`）的第二篇论文，两条线合并成一篇：

1. **电荷 = 流散度，汇即抹平**：正电荷是源（正散度），负电荷是汇（负散度）；加速电荷
   ⟹ 反引力场 ⟹ 光子的条件推导链（CR1–CR5）；向心收缩以平方因子抹平起伏
   `Q_A → (1−λ)²Q_A`（CR9–CR10）——负电荷是反引力场的天然载体。
2. **半相位几何**：包络反射不动点 `ln(√e) = ½` 定位自旋 ½；半角相位 `exp(iθ/2)`
   是费米型闭包见证（CS2–CS5）。

结尾接双流环装置应用：环流电子自抹平把到达工作窗口 μ=0.999 从 132 步缩短到 85 步，
外部 RMF 减半仍可达。

## 动机（论文自己的思想史）

始于黎曼猜想（临界线 Re s = ½ 是反射不动集）→ 隐数空间尝试（失败：一张叶装不下费米/玻色
两种统计）→ 统一光子/费米子/玻色子 + 胶球质量（格点谱给质量不给来源）→ 顿悟：空间是
介质，质量=锚定，电荷=散度，汇=收敛流，完全收缩=抹平=光子。

## 文件

| 文件 | 说明 |
|---|---|
| `projection-sink-photon.tex` / `.pdf` | 英文版（16 页，tectonic 编译） |
| `projection-sink-photon-zh.tex` / `.pdf` | 中文版（9 页，tectonic 编译） |
| `projection-physics.bib` | 参考文献（26 条，含 Riemann 1859 动机起点） |
| `excellent-paper-patterns.md` | 优秀论文模式笔记（改写依据：13 篇经典论文） |

## 诚实边界

- 链条是条件性的：**若**发生抹平，任意锚定物质都变成光子；不证明加速电荷自动抹平
- λ（汇收缩率）与 δ, ε（汇能量尺度）是输入参数，不是推导值
- 连续 3D 散度到起伏泛函的对应未形式化（离散格点定理是代数种子）
- 自旋 ½ 被定位而非推导（自旋-统计定理另一半未做——半条定理）
- 无新可检验预言；数值复现已知物理

全部论断在 Lean 4 中零 `sorry` 形式化（4348 jobs 全绿），详见主仓
`logos-42/Hibs-Physics`。

## 编译

```bash
tectonic projection-sink-photon.tex      # 英文版
tectonic projection-sink-photon-zh.tex   # 中文版
```

## 关系

- 主仓：`logos-42/Hibs-Physics`（Lean 形式化 + 数值验证 + 第一篇论文 paper/）
- 本仓是第二篇论文的独立发布（原 Hibs-Physics 的 paper2/ 目录）
