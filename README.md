# 数学建模体验课 · 上海交大 GC 科学营

> 一套面向零基础同学的**数学建模入门体验材料**：用一个真实美赛案例，带你走完「读题建模 → 编程作图 → 写作排版」的完整流程。

本仓库对应 2025 年 MCM/ICM 竞赛 **Problem C（奥运会奖牌数据）**，课堂目标是用约 45 分钟把一篇 O 奖论文的 **Model I** 完整复现出来，最终编译出一篇含模型、结果表和图片的论文初稿。

---

## 课程主线

```
读题建模  →  编程作图  →  写作编译
（AI 读题）   （Python）    （LaTeX + AI 助手）
```

- **读题建模**：用 AI 工具（DeepSeek / ChatGLM）通读赛题，梳理两个问题、建立模型、生成符号表与假设。
- **编程作图**：用 Python（Notebook）读取奥运数据，用 SVR 预测 2028 洛杉矶奖牌数，并画出结果图。
- **写作编译**：在 LaTeX 在线环境（latex.sjtu.edu.cn）中导入模板、粘贴正文、插入图片与结果表，编译出论文 PDF。

---

## 目录结构

```
10-24上海交大GC科学营数学建模体验课/
├── 1_数学建模体验课课前准备.docx      # 课前工具准备清单（4 种免费工具）
├── 2_数学建模体验课课堂操作指南.docx  # 课堂分步操作指南（读题→作图→写作）
├── 3_Latex_start.zip                 # LaTeX 入门模板（easymcm-course，课堂编辑起点）
├── 4_编程作图演示.ipynb              # Python 编程作图演示 Notebook（复现 O 奖 Model I）
├── 5_Latex_final.zip                 # 课堂最终 LaTeX 工程样例（in_progress）
├── fig1.png / fig2.png              # 课堂演示用结果图
└── 2025-C-部分O奖论文/               # 部分 2025 MCM Problem C 的 O 奖论文（PDF，仅供学习参考）
```

| 文件 | 说明 |
| --- | --- |
| `1_数学建模体验课课前准备.docx` | 课前需要安装 / 注册的 4 种免费工具说明 |
| `2_数学建模体验课课堂操作指南.docx` | 课堂完整操作流程与提示词（prompt） |
| `3_Latex_start.zip` | 比赛用 LaTeX 模板，含 `main.tex` 与 `sections/` 各章节骨架 |
| `4_编程作图演示.ipynb` | 从零读取奥运数据、SVR 预测、绘图的 Python 演示 |
| `5_Latex_final.zip` | 课堂产出的完整 LaTeX 工程（含 `main.pdf` 样例） |
| `2025-C-部分O奖论文/` | 数篇官方 O 奖论文 PDF，用于对照学习 |

---

## 课前准备（4 种免费工具）

详见 `1_数学建模体验课课前准备.docx`，要点如下：

| 类别 | 工具 | 用途 |
| --- | --- | --- |
| 必备 · 写作 | [latex.sjtu.edu.cn](https://latex.sjtu.edu.cn/)（jAccount 登录） | LaTeX 在线编译，无需本地安装 |
| 必备 · 写作 | [智谱清言 ChatGLM](https://chatglm.cn/) 等 AI 对话工具 | 读题、生成模型与正文 |
| 选做 · 编程 | [WorkBuddy](https://www.workbuddy.cn/) | 本地 AI Agent，辅助编程与论文完善 |
| 选做 · 编程 | [VS Code](https://code.visualstudio.com/) + Python + Jupyter | 运行 `.ipynb` 编程演示 |

---

## 快速开始

1. **读题**：打开 [COMAP 2025 赛题页](https://www.contest.comap.com/undergraduate/contests/mcm/contests/2025/problems/) 下载 Problem C 的 PDF 与 `Data.zip`，解压数据。
2. **建模**：用 DeepSeek 上传赛题，参考 `2_数学建模体验课课堂操作指南.docx` 中的提示词，生成模型与英文 LaTeX 正文。
3. **编译起点**：用 jAccount 登录 latex.sjtu.edu.cn，上传 `3_Latex_start.zip` 作为新项目，先编译模板；再把生成的正文粘贴进 `sections/` 对应章节。
4. **编程作图**：用 VS Code 打开含数据的文件夹，运行 `4_编程作图演示.ipynb`（逐格 `Shift+Enter`），得到结果图与数值。
5. **完善论文**：把 `5_Latex_final.zip` 作为参考，将图片存入 `figure/` 并在 `result.tex` 中引用，参考 O 奖论文样式补全各章节，重新编译。

> 提示：环境卡住时可直接使用仓库中附带的参考结果（PDF / 图片）继续后续步骤。

---

## 技术栈

- **建模 / 写作**：LaTeX（easymcm-course 模板）、AI 对话工具
- **编程 / 作图**：Python 3、`numpy` / `pandas` / `matplotlib` / `scikit-learn`（SVR）
- **辅助**：Jupyter Notebook、WorkBuddy AI Agent

---

## 说明与版权

- 本仓库为**教学与学习用途**的体验课材料，供同学课前预习与课堂实践使用。
- `2025-C-部分O奖论文/` 中的 PDF 为 MCM/ICM 官方发布的获奖论文，**版权归 COMAP 及相应参赛队伍所有**，仅限个人学习参考，请勿用于商业用途或二次发布。
- 赛题、数据等原始材料版权归 [COMAP](https://www.comap.com/) 所有，请遵守竞赛官方规定。

---

## 贡献

如有排版错误、链接失效或希望补充内容，欢迎提交 Issue 或 Pull Request。

作者 上海交通大学 张嘉乐 zhangjiale100@sjtu.edu.cn
