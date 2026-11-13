# Cauvera 教程课程库

DSH（Cauvera）教程栏的公开课程库。软件默认从这里读课程目录，用户在教程栏的「课程库」里点「下载」就能安装课程，不需要登录。

- 课程目录：https://github.com/leshenzhang/cauvera-tutorials/releases/latest/download/catalog.json
- 课程包：每次更新发一个 Release，`catalog.json` 和全部课程包（`<id>-<version>.tar.gz`）都作为 Release 附件上传。`catalog.json` 里的包名是相对地址，按目录地址解析，所以总是指向最新 Release。
- 格式：课程包是课程文件夹（`course.json`、`chapters/*.md`、章节引用的图片、上游许可原文 `LICENSE`）打成的 `.tar.gz`。`catalog.json` 给出每门课的 `sha256`，软件下载后先核对再安装。格式说明见 DSH 仓库 `docs/TUTORIAL.zh-CN.md` 的「课程库」一节。

## 课程

这里收开放许可的课程，以及经原作者授权公开分发、由课题组整理改编的计算化学笔记（`cc-notes-*`）。每门课按原许可改编成 DSH 课程格式，`course.json` 的 `source` 和包内 `LICENSE` 写明作者、许可和原始仓库；第三方版权图片没有收入，只保留原文链接。

| id | 课程 | 章 | 作者 | 许可 | 原始仓库 |
|---|---|---|---|---|---|
| `atomistic-cookbook` | Atomistic Cookbook | 45 | EPFL COSMO lab (cosmo software cookbook developers) | BSD-3-Clause | https://github.com/lab-cosmo/atomistic-cookbook |
| `epfl-iesm` | Introduction to Electronic Structure Methods (EPFL CH-353) | 37 | Ursula Roethlisberger and contributors (EPFL LCBC) | CC BY-SA 4.0 | https://github.com/lcbc-epfl/iesm-public |
| `epfl-mdmc` | Molecular Dynamics and Monte Carlo (EPFL) | 22 | Ursula Roethlisberger and contributors (EPFL LCBC) | Text CC BY-SA 4.0, code MIT | https://github.com/lcbc-epfl/mdmc-public |
| `fairchem-docs` | FAIR Chemistry (fairchem) Documentation | 63 | FAIR Chemistry & Collaborators (Meta) | MIT | https://github.com/facebookresearch/fairchem |
| `kitchin-dft-book` | Modeling Materials Using Density Functional Theory | 30 | John R. Kitchin | CC BY 4.0 (text and figures), MIT (code) | https://github.com/jkitchin/dft-book |
| `mace-tutorials` | MACE Tutorials | 5 | I. Batatia et al. | MIT | https://github.com/ACEsuit/mace-tutorials |
| `qcedu-introqm` | Introduction to Quantum Mechanics for Chemists (QC-Edu IntroQM) | 22 | Paul Ayers, Valerii Chuiko, Farnaz Heidar-Zadeh | CC0 1.0 | https://github.com/QC-Edu/IntroQM |
| `zenggs05-dft-common` | DFT 计算通用基础与脚本资源 | 9 | Gaoshan Zeng | MIT | https://github.com/zenggs05/DFT-Tutorials |
| `zenggs05-dft-cp2k` | CP2K 第一性原理计算教程 | 32 | Gaoshan Zeng | MIT | https://github.com/zenggs05/DFT-Tutorials |
| `zenggs05-dft-gaussian` | Gaussian 量子化学计算教程 | 52 | Gaoshan Zeng | MIT | https://github.com/zenggs05/DFT-Tutorials |
| `zenggs05-dft-openmx` | OpenMX 第一性原理计算教程 | 51 | Gaoshan Zeng | MIT | https://github.com/zenggs05/DFT-Tutorials |
| `zenggs05-dft-vasp` | VASP 第一性原理计算教程 | 69 | Gaoshan Zeng | MIT | https://github.com/zenggs05/DFT-Tutorials |
| `cc-notes-qc` | 量子化学计算笔记 | 240 | Cauvera 课题组整理 | 经原作者授权公开分发与改编 | — |
| `cc-notes-multiwfn` | Multiwfn 波函数分析笔记 | 226 | Cauvera 课题组整理 | 经原作者授权公开分发与改编 | — |
| `cc-notes-md` | 分子模拟笔记 | 42 | Cauvera 课题组整理 | 经原作者授权公开分发与改编 | — |
| `cc-notes-vmd` | VMD 可视化笔记 | 20 | Cauvera 课题组整理 | 经原作者授权公开分发与改编 | — |
| `cc-notes-cp2k` | CP2K笔记 | 6 | Cauvera 课题组整理 | 经原作者授权公开分发与改编 | — |
| `cc-notes-dft-pbc` | 第一性原理计算笔记 | 4 | Cauvera 课题组整理 | 经原作者授权公开分发与改编 | — |
| `cc-notes-orca` | ORCA笔记 | 1 | Cauvera 课题组整理 | 经原作者授权公开分发与改编 | — |

CC BY-SA 4.0 的课程（`epfl-iesm`、`epfl-mdmc` 文本）改编后仍按 CC BY-SA 4.0 发布。

## 更新

在维护者本机重新打包后发布新 Release（例如 `v2026.11.13`），上传 `catalog.json` 和全部课程包。已安装的课程版本与目录不同时，教程栏显示「更新」。
