# **survey**

tools：  
1\. Bitbead: [https\://www\.bitbead.app/en/generator](https://www.bitbead.app/en/generator) (web)  
2\. Beadmachine: [https\://pkg.go.dev/github.com/cornelk/beadmachine](https://pkg.go.dev/github.com/cornelk/beadmachine) (web)   
	[https\://github.com/cornelk/beadmachine/blob/2cba9d970c85/beadmachine.go](https://github.com/cornelk/beadmachine/blob/2cba9d970c85/beadmachine.go) (git)  
3.Beads: [https\://github.com/hiro-sys/iron-beads-designer](https://github.com/hiro-sys/iron-beads-designer) (git)  
4\. Pixelbead: [https\://www\.pixelbead.art/?utm\_source=devto\&utm\_medium=organic\_article\&utm\_campaign=launch\_jun\_2026](https://www.pixelbead.art/?utm_source=devto&utm_medium=organic_article&utm_campaign=launch_jun_2026) (web)  
5\. Perler Bead Pattern Maker [https\://madegooddesigns.com/tools/perler-bead-pattern-maker/](https://madegooddesigns.com/tools/perler-bead-pattern-maker/) (web)  
**6\. Perler Pattern [https\://clawhub.ai/tobewin/skills/perler-pattern](https://clawhub.ai/tobewin/skills/perler-pattern) (ai agent)**  
**7\. KP [https\://kandipad.com/fuse-bead-patterns?s=3d](https://kandipad.com/fuse-bead-patterns?s=3d) (web: 给了可以组装成3d物体的图纸)**  
**8.Beadify: [https\://beadify.app/how-to-iron-fuse-beads](https://beadify.app/how-to-iron-fuse-beads) (有关熨烫的指南）**

本文收录 38 项相关工作，每项按以下 7 个字段整理：名称、链接、年份、发表期刊或会议、输入（Input）、任务（Task）、参考价值与区别。各项按与本项目的相关程度排序，分为三级：

> * **S**：与本项目问题最接近，或可直接作为本项目某一模块的方法基础。  
> * **A**：方法或问题表述可供借鉴。  
> * **B**：领域背景或对比基线（baseline）。

## **总表 / Overview**

| \# | 名称 | 年份 | 期刊/会议 | 相关度 | 主要关联   |
| :---- | :---- | :---- | :---- | :---- | :---- |
| 1 | SD-πXL | 2024 | SIGGRAPH Asia | S | 限色低分辨率图像生成，含拼豆实例 |
| 2 | ALPS | 2026 | SIGGRAPH | S | 限色抽象与手工制作；stencil 连通性 |
| 3 | Diceplay | 2026 | SIGGRAPH | S | 极低分辨率离散网格的图像生成 |
| 4 | Legolization | 2015 | SIGGRAPH Asia (TOG) | S | 连通性与受力稳定性的结构优化 |
| 5 | Computational Thermoforming | 2016 | SIGGRAPH (TOG) | S | 热过程仿真、标定与逆向设计 |
| 6 | Fabricable 3D Wire Art | 2024 | SIGGRAPH | S | 语义损失与可制造性正则的联合优化 |
| 7 | Pixel Art Adaptation | 2022 | Pacific Graphics (CGF) | A | 珠子类手工 pixel art 的制作误差修正 |
| 8 | BrickGPT | 2025 | ICCV | A | 物理稳定性约束下的生成 |
| 9 | BrickWright | 2026 | arXiv | A | 以连通分量数作为可行性指标 |
| 10 | DreamWire | 2024 | CVPR | A | 连通性的可微软约束 |
| 11 | MechStyle | 2025 | ACM SCF | A | 生成式设计与结构仿真结合 |
| 12 | String Art | 2018 | Eurographics (CGF) | A | 媒介前向模型与二值离散优化 |
| 13 | Spider-Web String Art | 2019 | CAVW | A | 制造约束作为优化硬约束 |
| 14 | Fully Automated Bead Art Assembly | 2022 | J. Robotics & Mechatronics | B | 拼豆的机器人自动摆放 |
| 15 | Pixelated Image Abstraction | 2012 / 2013 | NPAR / Computers & Graphics | B | 基于优化的 pixel art 生成 |
| 16 | Content-Adaptive Image Downscaling | 2013 | SIGGRAPH Asia (TOG) | B | 内容自适应缩小，保持线条连通 |
| 17 | Perceptually Based Downscaling | 2015 | SIGGRAPH (TOG) | B | 基于 SSIM 的感知缩小，闭式解 |
| 18 | Depixelizing Pixel Art | 2011 | SIGGRAPH (TOG) | B | pixel art 矢量化放大；对角连通歧义处理 |
| 19 | Real-ESRGAN | 2021 | ICCV Workshops | B | 真实图像盲超分辨率，放大并去伪影 |
| 20 | CLIPasso | 2022 | SIGGRAPH (TOG) | A | 用最少笔画保持可识别性；CLIP 感知损失与显著性初始化 |
| 21 | Quantifying Visual Abstraction Quality for Stipple Drawings | 2017 | NPAR | A | 点数与感知抽象质量呈对数关系；成对比较用户实验 |
| 22 | Depth-First Search and Linear Graph Algorithms | 1972 | SIAM J. Computing | S | 线性时间求割点与双连通分量；连通性检查与单点失效分析的基础 |
| 23 | Maximal Flow Through a Network | 1956 | Canadian J. Mathematics | S | 最大流最小割定理；平面图最小割等于对偶图最短路 |
| 24 | Designing Structurally-Sound Ornamental Curve Networks | 2016 | SIGGRAPH (TOG) | A | 特征模态分析找最软变形；虚拟边指示最佳补强位置 |
| 25 | Worst-Case Structural Analysis | 2013 | SIGGRAPH (TOG) | S | 未知载荷下的最坏载荷与最大应力；模态分析加线性规划 |
| 26 | Synthesis of Filigrees for Digital Fabrication | 2016 | SIGGRAPH (TOG) | A | 稀疏连通花丝图案合成；由密到疏、保持连通、先补弱再加厚 |
| 27 | Modeling of Bond Formation Between Polymer Filaments in the FDM Process | 2004 | J. Manufacturing Processes | S | 传热加烧结模型预测相邻塑料丝的颈部生长；热台实验标定 |
| 28 | A Transient Updated Lagrangian FE Formulation for Bond Formation in FDM | 2021 | J. Mech. Phys. Solids | A | 有限元模拟多颗粒颈部生长；邻居排布与重力影响熔接 |
| 29 | Prediction of Interlayer Strength in Material Extrusion Additive Manufacturing | 2020 | Additive Manufacturing | S | 强度 \= 压力驱动接触 × 分子扩散；实验验证的连接强度模型 |
| 30 | Process-Structure-Property Effects on ABS Bond Strength in FFF | 2018 | Additive Manufacturing | A | 红外测温、截面测接触长度；归一化接触长度超过 0.6 后强度饱和 |
| 31 | An Inverse Procedural Modeling Pipeline for SVBRDF Maps | 2022 | ACM TOG | A | 材质贴图分解为子材质与掩码并程序化；少参数、可编辑的外观模型 |
| 32 | Practical Inverse Rendering of Textured and Translucent Appearance | 2025 | ACM TOG (SIGGRAPH) | B | Laplacian mipmapping；可微路径追踪次表面散射；从照片反推外观 |
| 33 | Optimization of FFF Process Parameters under Uncertainty | 2020 | Additive Manufacturing | S | KOH 贝叶斯校准模型偏差；稳健工艺参数优化 |
| 34 | Data-Driven Process Optimization of FFF based on In Situ Measurements | 2023 | IFAC-PapersOnLine | A | 原位粗糙度作为质量代理指标；约束贝叶斯优化 |
| 35 | Improving Geometric Accuracy of 3D Printed Parts Using 3D Metrology Feedback and Mesh Morphing | 2020 | J. Manuf. Mater. Process. | S | 多件扫描平均分离系统误差；反向预变形补偿 |
| 36 | On Iterative Pre-Compensation of 3D Laser-Printed Micro-Optical Components | 2024 | Adv. Funct. Mater. | A | 2.5D 高度图配准、过滤、逐像素迭代预补偿 |
| 37 | Two-Dimensional Digital Image Correlation: A Review | 2009 | Meas. Sci. Technol. | A | 2D DIC 测量面内位移与应变场 |
| 38 | Bayesian Calibration of Computer Models | 2001 | J. R. Stat. Soc. B | A | 含模型偏差项的贝叶斯校准框架（KOH） |

### ---

**1\. SD-πXL（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | SD-πXL: Generating Low-Resolution Quantized Imagery via Score Distillation（A. Binninger, O. Sorkine-Hornung；ETH Zurich） |
| 链接 | [Paper](https://arxiv.org/abs/2410.06236) · [Code](https://github.com/AlexandreBinninger/SD-piXL) · [Project](https://igl.ethz.ch/projects/sd-pixl/) |
| 年份 | 2024 |
| 期刊/会议 | SIGGRAPH Asia 2024 Conference Papers，DOI 10.1145/3680528.3687570 |
| Input | 文本提示（text prompt），可选条件图像；输出分辨率 H×W；n 色调色板 |
| Task | 生成颜色严格取自给定调色板的低分辨率图像。以 Gumbel-softmax 将离散颜色选择松弛为可微形式，以 SDXL 的 latent score distillation 及 ControlNet（Canny 边缘、深度图）保持语义，并加入基于 FFT 的平滑正则。实物示例包括十字绣、拼豆与积木。 |
| 参考价值与区别 | **参考价值**：提供了可微的离散调色板选择方法，以及在低分辨率下保持语义的生成先验，可作为拼豆图纸生成阶段的基线。 **区别**：仅优化排布时的图案，未建模熨烫引起的形变与熔合，不包含留空选项，也没有连通性或结构约束。 |

### **2\. Gradient Descent in the ALPS（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Gradient Descent in the ALPS: Abstracted Low-Poly Stylization and Fabrication（R. Wiersma, A. Binninger 等；ETH Zurich） |
| 链接 | [Paper](https://alexandrebinninger.com/ALPS/paper/alps.pdf) · [Code](https://github.com/rubenwiersma/alps) · [Project](https://alexandrebinninger.com/ALPS/) |
| 年份 | 2026 |
| 期刊/会议 | SIGGRAPH 2026 Conference Papers，DOI 10.1145/3799902.3811050 |
| Input | 目标图像与固定调色板 |
| Task | 将图像抽象为二维 low-poly 三角网格，要求网格为流形、无自相交且颜色限定于调色板。以深度条件的 score distillation 联合优化顶点位置与面颜色，并通过由细到粗的 edge collapse 改变网格拓扑。实物应用包括刺绣、彩色玻璃、木皮马赛克、钩针挂毯、拼布与 stencil。 |
| 参考价值与区别 | **参考价值**：通过网格简化处理离散拓扑变化的思路可用于留空优化；其 stencil 应用沿网格边保留材料以保证连通，与镂空拼豆的连通性问题同属一类。 **区别**：基本单元为自由多边形而非固定网格上的圆形豆子；其连通性由几何构造保证，而拼豆的连通性取决于熨烫这一物理过程；不预测制作后的外观变化。 |

### **3\. Diceplay（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Diceplay: A Modular Canvas for Physical Image Composition（M. Kodnongbua, …, A. Schulz；University of Washington 等） |
| 链接 | [Project](https://www.computationaldesign.group/publications/diceplay) · [Paper](https://dl.acm.org/doi/10.1145/3799902.3811206) |
| 年份 | 2026 |
| 期刊/会议 | SIGGRAPH 2026 Conference Papers，DOI 10.1145/3799902.3811206 |
| Input | 文本提示；5×5 骰子网格，每颗骰子六面印有几何图案，计入旋转共 15 种 tile |
| Task | 为每个格子选择骰子朝上的面与旋转方向，组成符合提示的图像。方法在 tile 边界上进行插值，以形状文法（shape grammar）约束相邻格子之间的依赖，并以 Stochastic Rewrite Descent 交替执行 score distillation 梯度更新与离散改写。 |
| 参考价值与区别 | **参考价值**：实验表明 Gumbel-softmax 松弛在极低分辨率下失效，提示拼豆尺度的生成需单独验证；邻域约束下的离散改写可用于在保持连通的前提下决定留空；其用户研究显示 CLIP 分数与人类偏好相关性很低（R² \= 0.013）。 **区别**：骰子之间不存在物理连接，制作过程不改变外观，不涉及结构问题。 |

### **4\. Legolization（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Legolization: Optimizing LEGO Designs（S.-J. Luo, Y. Yue, C.-K. Huang, Y.-H. Chung, S. Imai, T. Nishita, B.-Y. Chen） |
| 链接 | [Paper](https://dl.acm.org/doi/10.1145/2816795.2818091) |
| 年份 | 2015 |
| 期刊/会议 | ACM Transactions on Graphics 34(6), Article 222（SIGGRAPH Asia 2015） |
| Input | 带颜色的三维模型 |
| Task | 生成兼顾形状、颜色、砖块数量与物理稳定性的 LEGO 布局。第一阶段基于连通分量保证结构连通；第二阶段进行基于摩擦力与法向力的稳定性分析，并在最薄弱处局部重排砖块。 |
| 参考价值与区别 | **参考价值**：“先连通、再受力分析、于薄弱处局部修改”的流程可对应本项目的结构项 S；其指出图结构相同的布局可能具有不同的稳定性，说明仅凭图论规则不足以判断结构强度。对应 Stage 2 的 Q6 与 Q7：① 力分析模型——每块砖满足力与力矩平衡，摩擦力受最大摩擦载荷 T 约束，法向力只能受压，在所有满足平衡的力分布中求使最小剩余容量最大者，得到每个连接的受力、稳定性指标 C\_M 与最弱连接；将容量写入目标而非约束，使不稳定的设计之间也可比较。拼豆可改写为每个熔合连接传递轴力、剪力与弯矩的线性规划。② 悬挂场景的最大承载力可通过逐步增大挂钩载荷直至 C\_M 降为零得到（Q7）。③ 附录 A 以悬挂砝码测量最大摩擦载荷 T，可作为熨烫连接强度标定实验的模板。④ 悬臂桥实验表明图结构相同的布局稳定性可以不同，说明 Q3–Q5 的图论分析需由力学分析补充。 **区别**：研究对象为三维堆叠结构，连接方式为确定的卡扣，载荷为重力；拼豆为二维平面，连接依赖热熔且强度受工艺影响。 |

### **5\. Computational Thermoforming（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Computational Thermoforming（C. Schüller, D. Panozzo, A. Grundhöfer, H. Zimmer, E. Sorkine, O. Sorkine-Hornung；ETH Zurich, Disney Research） |
| 链接 | [Paper](https://la.disneyresearch.com/wp-content/uploads/Computational-Thermoforming-Paper.pdf) · [Project](https://studios.disneyresearch.com/2016/07/11/computational-thermoforming/) |
| 年份 | 2016 |
| 期刊/会议 | ACM Transactions on Graphics（SIGGRAPH 2016），DOI 10.1145/2897824.2925914 |
| Input | 带纹理的三维模型及对应模具 |
| Task | 仿真塑料片在加热与真空成型过程中的形变（Batty 2012 粘性薄片模型，加入塑性、粘附接触，分松弛、模具上升、抽真空三阶段），并逆向计算平面塑料片上应打印的预畸变图案，使成型后的颜色与几何对齐。标定只需一个金字塔标定物：印上多尺度 RGB 噪声纹理与色卡，成型后拍照三维重建，经 homography 对齐与光流求出稠密位移场；9 个仿真参数中只拟合 4 个（杨氏模量、蠕变、屈服应变、粘度），在材料表给出的范围内以 625 点网格搜索；在半球与猫模型上验证，误差 1.5 与 1.6 mm，接近标定误差 1.3 mm；作者指出误差分布不均可能来自加热不均匀。 |
| 参考价值与区别 | **参考价值**：提供了“热过程仿真、外观预测、逆向设计”的完整框架，以及仅拟合少量材料参数、使用专用标定件、网格搜索参数并在未见形状上验证误差的标定流程，可用于熔合模型 F 的标定。对应 Stage 3：S3-Q1（每种熨烫条件熨一块标准测试板，旁置色卡拍照、homography 对齐网格，测外径、孔洞、颈部与颜色，再拟合膨胀率、孔洞闭合率、颈部生长速率、晕染宽度等少量参数，并跨熨烫条件插值）；S3-Q3（简化模型实现快速预览）；S3-Q5（预先补偿，如预先加宽易断的细颈）；S3-Q6（留出验证与误差分布分析）。其加热不均匀的发现提示家用熨斗需用可控加热设备标定，或采用位置相关或概率化的连接模型。对应 S3-Q8：作为熔合模型的初始标定（标准测试板、少量有效参数、网格搜索、留出验证），之后由 KOH 式贝叶斯校准（33、38）持续更新。 **区别**：处理的是连续塑料片的大变形，目标是复制已有物体；拼豆为离散单元的局部熔合，目标是生成图像作品。 |

### **6\. Fabricable 3D Wire Art（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Fabricable 3D Wire Art（K. Tojo, A. Shamir, B. Bickel, N. Umetani） |
| 链接 | [Paper](https://www.dropbox.com/scl/fi/pvvjthg9uir0sg16rvq2n/wireart_sig24.pdf?rlkey=ynzvq9t7ro9btbw8ejwfzjgzy&dl=0) · [Code](https://github.com/kenji-tojo/fab3dwire) · [Project](https://kenji-tojo.github.io/publications/fab3dwire/) |
| 年份 | 2024 |
| 期刊/会议 | SIGGRAPH 2024 Conference Papers，DOI 10.1145/3641519.3657453 |
| Input | 三维模型、图像或文本 |
| Task | 优化一条可由铁丝弯折而成的三维 B-spline 曲线，使其多视角可微渲染结果在语义上接近目标；以曲率、扭转与间隙构成可制造性正则项；同时生成辅助弯折的可打印夹具。 |
| 参考价值与区别 | **参考价值**：目标函数由语义损失与可制造性正则组成，与本项目目标函数的结构一致；同时输出辅助制造工具，可类比为输出熨烫建议。 **区别**：铁丝为连续媒介，约束为几何约束；拼豆为离散媒介，约束来自热熔合的物理过程。 |

### **7\. Pixel Art Adaptation for Handicraft Fabrication（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Pixel Art Adaptation for Handicraft Fabrication（Y. Igarashi, T. Igarashi） |
| 链接 | [Paper](https://www.is.ocha.ac.jp/~yuki/papers/pixelArtAdaptation_PG2022.pdf) · [Project](https://www.is.ocha.ac.jp/~yuki/pixelArtAdaptation/index-e.html) |
| 年份 | 2022 |
| 期刊/会议 | Computer Graphics Forum 41(7)（Pacific Graphics 2022），pp. 489–494 |
| Input | pixel art 设计稿，以及制作过程中已完成（可能含错误）的部分 |
| Task | 在编织、十字绣与串珠（bead weaving）等手工制作中出现错位、重复或遗漏时，调整尚未制作的部分以减弱错误的可见性。行间采用贪心策略，行内采用动态规划，并向用户提供多个候选方案。 |
| 参考价值与区别 | **参考价值**：是少数直接处理珠子类手工 pixel art 的学术工作；其基于相邻像素对保持的代价函数简单且可解释，可用于处理摆放阶段的误差。 **区别**：处理的是人为制作误差而非材料的物理变化；串珠可在制作中修改，而拼豆熨烫后无法修改。 |

### **8\. BrickGPT（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Generating Physically Stable and Buildable Brick Structures from Text（A. Pun, K. Deng, R. Liu, D. Ramanan, C. Liu, J.-Y. Zhu；Carnegie Mellon University） |
| 链接 | [Paper](https://arxiv.org/abs/2505.05469) · [Code](https://github.com/AvaLovelace1/BrickGPT) · [Project](https://avalovelace1.github.io/BrickGPT/) |
| 年份 | 2025 |
| 期刊/会议 | ICCV 2025（Best Paper） |
| Input | 文本提示 |
| Task | 以微调的大语言模型在 20×20×20 网格上逐块自回归生成 LEGO 结构。生成过程中对每块砖进行有效性检查与拒绝采样，生成后进行受力稳定性分析，若不稳定则回退到首个不稳定砖块之前重新生成。 |
| 参考价值与区别 | **参考价值**：消融实验显示，去除拒绝采样与回退后稳定率由 98.8% 降至 12.8%，说明不考虑物理约束的生成结果难以制作；“违反约束即回退”的策略可用于留空决策。 **区别**：研究对象为三维结构，由文本生成，以卡扣连接；拼豆为二维，以图像为目标，依靠热熔连接。 |

### **9\. BrickWright（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | BrickWright: Agentic Creation of Physically Feasible Brick Builds（A. Pun, …, M. Agrawala, J.-Y. Zhu；Carnegie Mellon University, Stanford University） |
| 链接 | [Paper](https://arxiv.org/abs/2610.31651) · [Code](https://github.com/AvaLovelace1/brickwright) · [Project](https://avalovelace1.github.io/brickwright/) |
| 年份 | 2026 |
| 期刊/会议 | arXiv 预印本 2610.31651 |
| Input | 文本提示 |
| Task | 为通用编程智能体提供一个 LEGO 搭建函数库，由智能体编写代码完成搭建，并在“规划、执行、验证”的循环中检查碰撞、悬空零件与连通分量数。 |
| 参考价值与区别 | **参考价值**：将“连通分量数为 1”作为独立的可行性指标进行报告，可用于评估熨烫后成品的连通性。 **区别**：仅进行几何检查，不含受力分析；拼豆的连通性需在物理层面判断，即熨烫后是否实际粘连及其强度。 |

### **10\. Wired Perspectives（DreamWire）（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Wired Perspectives: Multi-View Wire Art Embraces Generative AI（Z. Qu, L. Yang, H. Zhang, T. Xiang, K. Pang, Y.-Z. Song） |
| 链接 | [Paper](https://arxiv.org/abs/2311.15421) · [Code](https://github.com/WinKawaks/DreamWire) · [Project](https://dreamwireart.github.io) |
| 年份 | 2024 |
| 期刊/会议 | CVPR 2024，pp. 6149–6158 |
| Input | 最多三个视角各自对应的文本提示或草图 |
| Task | 以 score distillation（草图输入时结合 ControlNet）优化三维 Bézier 曲线，经可微渲染生成从不同方向观看呈现不同物体的线材雕塑，并以最小生成树软约束使所有曲线连为一体。 |
| 参考价值与区别 | **参考价值**：提供了将连通性表述为可微损失的实例，可与以硬约束处理连通性的方法对比。 **区别**：优化对象为连续曲线参数，可直接求梯度；拼豆为离散网格选择，并需额外建模热熔合。 |

### **11\. MechStyle（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | MechStyle: Augmenting Generative AI with Mechanical Simulation to Create Stylized and Structurally Viable 3D Models（F. Faruqi, …, S. Mueller；MIT CSAIL 等） |
| 链接 | [Paper](https://arxiv.org/abs/2509.20571) · [Project](https://hcie.csail.mit.edu/research/mechstyle/mechstyle.html) |
| 年份 | 2025 |
| 期刊/会议 | ACM Symposium on Computational Fabrication（SCF 2025），DOI 10.1145/3745778.3766655 |
| Input | 可三维打印的模型与风格描述 |
| Task | 以 CLIP 引导的网格变形对模型进行风格化，同时通过有限元分析（FEA）模拟跌落测试，限制高应力区域的修改，以保证打印后的结构可用。 |
| 参考价值与区别 | **参考价值**：其前期研究表明无约束风格化结果中仅 25.55% 结构可用，这种先量化问题严重程度的实验设计可用于说明本项目的研究动机。 **区别**：研究对象为三维打印的连续实体，采用 FEA；拼豆为二维离散单元，熔合强度需通过实验标定。 |

### **12\. String Art: Towards Computational Fabrication of String Images（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | String Art: Towards Computational Fabrication of String Images（M. Birsak, F. Rist, P. Wonka, P. Musialski） |
| 链接 | [Paper](https://www.peterwonka.net/Publications/pdfs/2018.EG.Birsak.StringArt.pdf) · [Code](https://github.com/Exception1984/StringArt) · [Project](https://www.cg.tuwien.ac.at/research/publications/2018/Birsak2018-SA/) |
| 年份 | 2018 |
| 期刊/会议 | Computer Graphics Forum 37(2)（Eurographics 2018） |
| Input | 灰度图像与圆形框上的钉子位置 |
| Task | 将钉子间连线的选择表述为非线性二值最小二乘问题并以迭代贪心算法求解，再将所选线段排列为可一次绕完的路径，由工业机器人完成制作。 |
| 参考价值与区别 | **参考价值**：将线宽等媒介属性写入前向模型；指出将二值问题松弛后取阈值的效果不如直接求解二值问题，对拼豆的留空决策有参考意义。 **区别**：线的叠加近似线性，且制作完成后不再变化；拼豆熨烫为非线性过程，会改变孔径、轮廓与连接关系。 |

### **13\. A Computational Approach for Spider Web-Inspired Fabrication of String Art（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | A Computational Approach for Spider Web-Inspired Fabrication of String Art（S. Je, Y. Abileva, A. Bianchi, J.-C. Bazin；KAIST） |
| 链接 | [Paper](https://make.kaist.ac.kr/files/2019/Je_SpiderWeb_CAV19.pdf) · [Publisher](https://onlinelibrary.wiley.com/doi/abs/10.1002/cav.1904) |
| 年份 | 2019 |
| 期刊/会议 | Computer Animation and Virtual Worlds 30, e1904，DOI 10.1002/cav.1904 |
| Input | 目标图像与支撑边界上的钉子位置 |
| Task | 仅用一根连续的线绕出目标图像。以贪心策略逐步选择下一个钉子，代价为高斯模糊后的均方误差，并只允许机器可实现的连接；同时设计了低成本的自动绕线机。 |
| 参考价值与区别 | **参考价值**：将制造约束作为硬约束直接纳入优化；采用客观指标与小规模用户研究相结合的评估方式。 **区别**：其约束为路径连续性；拼豆的约束为网格上的区域连通性与熔合强度。 |

### **14\. Fully Automated Bead Art Assembly for Smart Manufacturing（B）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Fully Automated Bead Art Assembly for Smart Manufacturing Using Dynamic Compensation Approach（K. Murakami, S. Huang, M. Ishikawa, Y. Yamakawa；The University of Tokyo） |
| 链接 | [Paper](https://www.fujipress.jp/jrm/rb/robot003400050936) · [J-STAGE](https://www.jstage.jst.go.jp/article/jrobomech/34/5/34_936/_article/-char/ja) |
| 年份 | 2022 |
| 期刊/会议 | Journal of Robotics and Mechatronics 34(5), 936–945，DOI 10.20965/jrm.2022.p0936 |
| Input | 拼豆图纸与高速视觉的实时图像 |
| Task | 工业机器人从传送带上逐颗拾取直径 5 mm 的拼豆并插入拼豆板，通过动态补偿实时修正定位误差。按颜色拾取的成功率约 81%，插入成功率约 95%。 |
| 参考价值与区别 | **参考价值**：是以拼豆为对象的学术制造工作，其摆放误差数据可用于分析制作阶段的误差。 **区别**：只解决自动摆放问题，不涉及图案设计与熨烫。 |

### **15\. Pixelated Image Abstraction（B）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Pixelated Image Abstraction（扩展版：Pixelated Image Abstraction with Integrated User Constraints；T. Gerstner, D. DeCarlo, M. Alexa, A. Finkelstein, Y. Gingold, A. Nealen） |
| 链接 | [Paper](https://cragl.cs.gmu.edu/pixelate/pixelated_image_abstraction-journal.pdf) · [Project](https://cragl.cs.gmu.edu/pixelate/journal.html) |
| 年份 | 2012（会议版）；2013（期刊扩展版） |
| 期刊/会议 | NPAR 2012；Computers & Graphics 37(5), 333–347（2013） |
| Input | 图像、目标分辨率与颜色数 |
| Task | 以改进的 SLIC 超像素与 mass-constrained deterministic annealing 交替优化像素划分与调色板，生成限色 pixel art；扩展版支持用户约束。 |
| 参考价值与区别 | **参考价值**：经典的基于优化的 pixel art 生成方法，代码公开，可作为对比基线。扩展版允许用户以约束指定重要区域，可与 CLIPasso（20）的自动重要性图互补，用于 Stage 2 的 Q1；其在固定低分辨率网格上的抽象可作为 Q2 的离散基线。 **区别**：不包含语义先验，不考虑实物制作；调色板由算法自动求得，而非实际拼豆色卡。 |

### **16\. Content-Adaptive Image Downscaling（B）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Content-Adaptive Image Downscaling（J. Kopf, A. Shamir, P. Peers） |
| 链接 | [Paper (ACM)](https://doi.org/10.1145/2508363.2508370) |
| 年份 | 2013 |
| 期刊/会议 | ACM Transactions on Graphics 32(6), Article 173（SIGGRAPH Asia 2013） |
| Input | 高分辨率图像（自然图像、卡通或矢量图）与目标输出尺寸 |
| Task | 为每个输出像素构造由空间与颜色 Gaussian 组成的 bilateral kernel，以带约束的 EM 算法优化 kernel 的形状与位置，使其贴合局部图像特征；每轮迭代后施加空间、局部性与边缘方向约束。可结合 mean shift 或 k-means 后处理实现限色 pixel art。 |
| 参考价值与区别 | **参考价值**：可用于 Stage 1 中输入图像大于拼豆板时的缩小步骤，尤其适合卡通与线稿输入；其"缩小后线条保持连通"的特性与本项目的连通性目标可作类比。 **区别**：限色仅为后处理，不受实际拼豆色卡约束；不支持留空；不处理板子大于输入图像（放大）的情形；不考虑熨烫；迭代优化速度较慢。 |

### **17\. Perceptually Based Downscaling of Images（B）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Perceptually Based Downscaling of Images（A. C. Öztireli, M. Gross） |
| 链接 | [Paper (ACM)](https://doi.org/10.1145/2766891) |
| 年份 | 2015 |
| 期刊/会议 | ACM Transactions on Graphics 34(4), Article 77（SIGGRAPH 2015） |
| Input | 高分辨率图像与缩小倍数 |
| Task | 以感知图像质量指标 SSIM 衡量输入与输出的差异，将缩小表述为优化问题，并推导出闭式解；该解等价于一种自适应 unsharp masking 滤波，保持局部亮度与对比度并最大化结构相似性，运行速度接近线性滤波。 |
| 参考价值与区别 | **参考价值**：可作为 Stage 1 中照片类输入的快速缩小方法；以感知指标而非像素误差衡量结果的思路，可借鉴到本项目对熨烫后结果与输入图像的比较。 **区别**：输出为连续颜色，不进行限色；对规则高频图案仍会产生混叠；不支持留空与放大；不考虑熨烫。 |

### **18\. Depixelizing Pixel Art（B）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Depixelizing Pixel Art（J. Kopf, D. Lischinski） |
| 链接 | [Paper (ACM)](https://doi.org/10.1145/2010324.1964994) |
| 年份 | 2011 |
| 期刊/会议 | ACM Transactions on Graphics 30(4)（SIGGRAPH 2011） |
| Input | 手绘的小尺寸 pixel art 图像 |
| Task | 构建像素相似图，用三条感知启发式（曲线、稀疏像素、孤岛）消解对角连接的歧义，以广义 Voronoi 图重塑像素格子，再拟合并优化 B-spline 轮廓，输出可任意倍数放大的矢量图。 |
| 参考价值与区别 | **参考价值**：当输入为小尺寸 pixel art、而所选拼豆板大于输入时，可用于放大；其对角连通歧义的处理方式（含避免孤岛的规则）可借鉴到判断哪些对角相邻的豆子需要加固。 **区别**：不补充新细节，仅平滑轮廓；对抗锯齿或由照片缩小得到的输入效果差；输出为连续矢量图，不限色、不支持留空，不考虑熨烫。 |

### **19\. Real-ESRGAN（B）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Real-ESRGAN: Training Real-World Blind Super-Resolution with Pure Synthetic Data（X. Wang, L. Xie, C. Dong, Y. Shan） |
| 链接 | [Paper (arXiv)](https://arxiv.org/abs/2107.10833) · [Code](https://github.com/xinntao/Real-ESRGAN) |
| 年份 | 2021 |
| 期刊/会议 | ICCV Workshops 2021；arXiv 2107.10833 |
| Input | 存在未知退化（模糊、噪声、JPEG 压缩等）的低分辨率真实图像 |
| Task | 以二阶退化过程与 sinc 滤波器合成训练数据，训练基于 ESRGAN 生成器与带 spectral normalization 的 U-Net 判别器的超分辨率网络，实现 ×4 放大，同时去除伪影并恢复纹理。 |
| 参考价值与区别 | **参考价值**：当输入为低质量照片、而所选拼豆板大于输入时，可作为 Stage 1 的预处理，放大输入并去除噪声与压缩伪影，使后续色卡量化更干净。 **区别**：补出的纹理由 GAN 先验生成，不保证忠实于原图，且大部分会在缩小到板子分辨率并量化到色卡时丢失；训练数据为自然照片，不适合手绘 pixel art；不限色、不考虑熨烫。 |

### ---

**20\. CLIPasso（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | CLIPasso: Semantically-Aware Object Sketching（Y. Vinker, E. Pajouheshgar, J. Y. Bo, R. C. Bachmann, A. H. Bermano, D. Cohen-Or, A. Zamir, A. Shamir） |
| 链接 | [Paper (arXiv)](https://arxiv.org/abs/2202.05822) · [Project](https://clipasso.github.io/clipasso/) |
| 年份 | 2022 |
| 期刊/会议 | ACM Transactions on Graphics 41(4)（SIGGRAPH 2022）；arXiv 2202.05822 |
| Input | 单个物体的图像（有背景时先用 U2-Net 去背景）与笔画数 n |
| Task | 将草图表示为 n 条黑色 Bézier 曲线，经可微光栅化器（diffvg）渲染后，以 CLIP 感知损失（ResNet101 第 3、4 层特征的 L2 几何项，加 0.1 倍最终 embedding 的余弦语义项）直接优化控制点；笔画初始位置按 CLIP ViT 注意力 relevancy map 与 XDoG 边缘图的乘积采样；通过减少 n 控制抽象程度，并以用户实验（类别级与实例级识别）和 CLIP zero-shot 分类器评估可识别性。 |
| 参考价值与区别 | **参考价值**：与 Stage 2 的 Q1（哪些拼豆对识别最重要）和 Q2（如何在不影响识别的前提下减少拼豆）直接对应。① 注意力 relevancy map × 边缘图可下采样为每个 peg 的重要性图；② 实验表明 L2 与 LPIPS 不适合稀疏表示，CLIP 几何加语义损失可作为保真项；③ 笔画数对应拼豆预算，用户实验给出可识别性的断点（4 笔类别识别率 36%，8 笔 87%），可沿用此评估方式；④ 论文指出只删除、不重新放置的抽象方式（Muhammad et al. 2018）在高抽象程度下是次优的，提示拼豆的精简算法应允许交换或重新放置。 **区别**：笔画是连续、可微的曲线，拼豆是离散的 0/1 网格；不要求连通，也不考虑结构稳定性；以笔画数而非材料数量计预算；在 224×224 分辨率下渲染，远高于拼豆板；不考虑熨烫。 |

### ---

**21\. Quantifying Visual Abstraction Quality for Stipple Drawings（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Quantifying Visual Abstraction Quality for Stipple Drawings（M. Spicker, F. Hahn, T. Lindemeier, D. Saupe, O. Deussen） |
| 链接 | [Paper (ACM)](https://doi.org/10.1145/3092919.3092923) |
| 年份 | 2017 |
| 期刊/会议 | NPAR 2017（Proceedings of the Symposium on Non-Photorealistic Animation and Rendering） |
| Input | 灰度图像，以及用 Weighted Voronoi Stippling（Secord 2002）在不同点数下生成的点画 |
| Task | 提出与图像尺寸和内容无关的归一化指标 tonal percentage τ（点数占输入图像色调总和的比例）；通过众包成对比较实验（5 级 Likert 量表，245 名有效参与者，63000 条有效回答），用扩展的 Thurstone 模型重建绝对的感知抽象质量分数（MAS）；拟合得到对数模型 MAS(τ) \= α \+ β·ln(τ − γ)，R² 约 0.96，符合 Weber–Fechner 定律，并在新图像上验证（解释 94% 的方差）。 |
| 参考价值与区别 | **参考价值**：与 Stage 2 的 Q2（如何在不影响识别的前提下减少拼豆）直接对应。① 点画与拼豆同属离散点表示，其结论"质量随点数对数增长"为拼豆预算选择提供依据：τ 从 10% 增加到 20% 的质量提升是 40% 到 50% 的三倍以上，作者建议取色调总和的 20–40%；② tonal percentage 可借鉴为跨图像比较的归一化豆子预算；③ 成对比较加 Thurstone 重建的实验设计可直接用于拼豆的用户研究，并可用来校验 CLIP loss 等自动指标。 **区别**：对数模型单调递增，不存在最优点数，需按应用权衡；全图重要性均匀，不考虑语义（作者将人脸等重点区域列为未来工作），因此不直接回答 Q1；点的位置连续且互不相连，无连通与稳定性要求；只针对灰度，不考虑实物制作与熨烫。 |

### ---

**22\. Depth-First Search and Linear Graph Algorithms（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Depth-First Search and Linear Graph Algorithms（R. Tarjan） |
| 链接 | [Paper](https://epubs.siam.org/doi/epdf/10.1137/0201010) · [NetworkX 实现：articulation\_points](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.components.articulation_points.html) |
| 年份 | 1972 |
| 期刊/会议 | SIAM Journal on Computing 1(2), 146–160 |
| Input | 无向图（求割点与双连通分量）或有向图（求强连通分量） |
| Task | 证明对无向图做深度优先搜索（DFS）得到的有向图是 palm tree，即每条非树边都从某个顶点指向其祖先；据此定义 LOWPT(v)（沿树边向下、再经至多一条回边可到达的最小编号顶点），并给出割点判据：非根顶点 a 是割点，当且仅当它有子节点 v 满足 LOWPT(v) ≥ a；根是割点，当且仅当它有两个及以上子节点。一次 DFS 配合边栈即可求出全部割点与双连通分量，时间与空间均为 O(V+E)，在常数因子内最优。NetworkX 以非递归 DFS 实现该算法（文档引用 Hopcroft & Tarjan, CACM 16:372–378, 1973）。 |
| 参考价值与区别 | **参考价值**：直接对应 Stage 2 的 Q3 与 Q4。① Q3：在豆子邻接图（边由熨烫后是否粘合决定，4 邻接或 8 邻接）上，只删除非割点的豆子即可保证作品始终连通；每次删除后重新计算的代价在 100×100 板子上仅为毫秒级。② Q4：割点对应"某颗豆失效即导致分离"的位置，结合同类 DFS 算法求出的桥（bridge），可覆盖"某个连接断裂即导致分离"的情况，并按断开后脱落的豆子数排序，得到脆弱性地图。 **区别**：只诊断弱点，不负责修复，补强需要双连通增广（biconnectivity augmentation）或 Steiner 树；连接只分有无，不表达粘合强度；只考虑拓扑，不考虑受力（长悬臂根部即使不是割点也可能断裂）；NetworkX 约定两点一边的"二元组"也算一个双连通分量，因此只看割点会漏掉单一连接，必须同时求桥。 |

### ---

**23\. Maximal Flow Through a Network（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Maximal Flow Through a Network（L. R. Ford, Jr., D. R. Fulkerson） |
| 链接 | [Paper](https://www.cs.yale.edu/homes/lans/readings/routing/ford-max_flow-1956.pdf) · [NetworkX 实现：minimum\_cut](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.flow.minimum_cut.html) |
| 年份 | 1956 |
| 期刊/会议 | Canadian Journal of Mathematics 8, 399–404 |
| Input | 网络（图），每条边带有正的容量（capacity），并指定源点 a 与汇点 b |
| Task | ① 证明最大流最小割定理：从 a 到 b 的最大流值等于所有割（删去后使 a、b 不连通的极小边集）中容量之和的最小值；证明为非构造性的，利用流构成凸多面体，并说明在所有最大流中都饱和的边包含一个最小割。② 对 a、b 位于外边界的平面网络，证明最上方的路径与每个割恰好相交一次，由此给出逐条路径推流的手算方法。③ 指出平面网络的对偶关系：原图中 a 到 b 的最小割对应对偶图中的最短路径。④ 指出多对互不相通的源汇点时定理不成立。 |
| 参考价值与区别 | **参考价值**：直接对应 Stage 2 的 Q5（悬挂时最危险的断裂线）。① 以粘合强度作为容量、挂钩处的豆子作为源点，最小割即断开所需总强度最小的一组连接；② 4 邻接的拼豆网格是平面图，断裂线等价于对偶图（豆子间空隙）中按强度加权的最短路径，可直接画在作品上；③ 以每颗豆的重量连向超级汇点，可将"脱落重量与割强度之比最大"的断裂线化为一系列最小割问题（参数化最小割）；④ Q4 中的桥是容量全为 1 时割值为 1 的特例，两者可统一。 **区别**：容量模型只表达拉断，不表达弯矩，长悬臂根部的危险需要 Q6 的力学分析；8 邻接时对角边相互交叉，网格不再是平面图，对偶最短路方法不再适用，需改用一般最大流算法；直接以挂钩为源点、其余豆子为汇点的最小割会紧贴挂钩，必须结合脱落重量；容量需由熨烫后的拉伸实验标定。 |

### ---

**24\. Designing Structurally-Sound Ornamental Curve Networks（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Designing Structurally-Sound Ornamental Curve Networks（J. Zehnder, S. Coros, B. Thomaszewski） |
| 链接 | [Paper (ACM)](https://doi.org/10.1145/2897824.2925888) |
| 年份 | 2016 |
| 期刊/会议 | ACM Transactions on Graphics 35(4)（SIGGRAPH 2016） |
| Input | 三维曲面（Loop 细分曲面）与用户定义的二维样条曲线库 |
| Task | 将曲线建模为嵌入曲面的弹性曲线（discrete elastic rods），通过最小化弯曲、拉伸、防穿透与接触能量，交互式地放置、变形和连接曲线，生成可 3D 打印的装饰曲线网络；在结构分析中，由于手持与运输载荷无法预测，计算弹性能量 Hessian 的最小特征值模态（最容易发生的变形），并在空间上相近但未相连的点之间设置虚拟边，以其在低能量模态下的应变率指示最值得增加连接的位置，交由用户修正；修正后在 1000 个位置施加载荷，峰值变形降低约 2.24 倍。 |
| 参考价值与区别 | **参考价值**：对应 Stage 2 的 Q6（载荷未知时的变形分析）与 Q8（补强位置）。① 拼豆可建模为格子弹簧网络，以刚度矩阵的低阶特征模态找出最软的变形方式；② 指出变形最大处不一定是最佳补强处（两个半球仅以一条曲线相连的例子），虚拟边可直接用于判断在哪两颗隔空相邻的豆子之间补一颗桥接豆最有效。 **区别**：分析的是刚度与变形，不计算应力，不判断是否断裂；补强由用户手动完成；面向连续曲线与曲面，而非离散网格；假设线弹性、小变形。 |

### **25\. Worst-Case Structural Analysis（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Worst-Case Structural Analysis（Q. Zhou, J. Panetta, D. Zorin） |
| 链接 | [Paper (ACM)](https://dl.acm.org/doi/10.1145/2461912.2461967) |
| 年份 | 2013 |
| 期刊/会议 | ACM Transactions on Graphics 32(4), 137:1–137:12（SIGGRAPH 2013） |
| Input | 三维物体（四面体网格）与材料参数（可为各向异性），以及载荷族约束（只受正压力、压强上限 p\_max、总力 F\_tot、合力与合力矩为零） |
| Task | 在载荷未知时，求使最大主应力（或最大位移）最大的最坏载荷。该问题非凸，作者以近似方法求解：先做模态分析，取前 15 个模态中应力最高的 2.5% 区域作为弱区域；再以加权的应力迹替代最大主应力，使每个弱区域的问题成为线性规划，并通过一次线性求解消去位移变量。与暴力搜索结果一致，速度快 600–10000 倍；掉落测试与挤压测试中的断裂和变形位置与预测相符；并以三点弯曲测试测量三种打印材料的模量与临界应力。 |
| 参考价值与区别 | **参考价值**：对应 Stage 2 的 Q7（手持、运输等载荷未知场景下的最大承载力）与 Q6。① 线弹性下应力与载荷成正比，最大承载力为 F\_tot × 强度 / σ\_max；② 拼豆网络是离散的，每个连接的内力是载荷的线性函数，可对每个连接直接求两个小规模线性规划，无需应力迹近似，50×50 的板子可逐个连接遍历；③ 三点弯曲测试可借鉴为熨烫豆条的模量与断裂强度标定；④ 指出各向异性会改变最弱位置，提示需测量不同方向连接的强度。 **区别**：面向连续体有限元；只考虑压力，不考虑拉扯；以第一处达到强度视为失效，未考虑断裂后的力重新分配；模态弱区域假设未在离散网格上验证。 |

### **26\. Synthesis of Filigrees for Digital Fabrication（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Synthesis of Filigrees for Digital Fabrication（W. Chen, X. Zhang, S. Xin, Y. Xia, S. Lefebvre, W. Wang） |
| 链接 | [Paper (ACM)](https://doi.org/10.1145/2897824.2925911) |
| 年份 | 2016 |
| 期刊/会议 | ACM Transactions on Graphics 35(4), Article 98（SIGGRAPH 2016） |
| Input | 若干二维花丝基元（filigree element）与目标曲面，可附带控制方向与尺度的场 |
| Task | 以骨架图（medial axis）表示花丝；先用蓝噪声投点密集放置基元以保证覆盖与连通，再在连通硬约束下以随机搜索优化基元位置，用修正 Hausdorff 距离定义的图案匹配能量（PME）衡量重叠处的外观；以 boosting 记录并复用好的局部配置；以 topology cut 按长度与靠近末梢程度的重要性分数剪去冲突分支；最后以有限元分析找出薄弱区域，先在薄弱处加入基元，再整体加厚，直至无薄弱节点。 |
| 参考价值与区别 | **参考价值**：对应 Stage 2 的 Q2–Q4 与 Q8。① 骨架表示适合细线状的稀疏拼豆布局；② "由密到疏、全程保持连通"的策略与只删除非割点的精简方式一致；③ topology cut 的重要性分数可用于决定先删哪段分支；④ 修正 Hausdorff 距离可作为结构保真项；⑤ "先补弱、再加厚"的顺序可减少补强所需的豆子（作者实验发现先加厚无法消除薄弱区域，先补弱后只需少量加厚）；⑥ 合成与结构优化交替迭代、在薄弱处插入新元素后重新合成的流程，可作为 Q8 材料最少布局优化的主循环；⑦ boosting 允许暂时放松连通约束以跳出局部最优，并以独立集顺序更新互不相邻的元素，便于并行。 **区别**：目标是外观与强度，不显式最小化材料用量；外观由基元风格定义，而非输入图像；面向连续曲面与有限元应力，而非离散网格与熔合连接。 |

### ---

**27\. Modeling of Bond Formation Between Polymer Filaments in the Fused Deposition Modeling Process（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Modeling of Bond Formation Between Polymer Filaments in the Fused Deposition Modeling Process（C. Bellehumeur, L. Li, Q. Sun, P. Gu） |
| 链接 | [Paper](https://doi.org/10.1016/S1526-6125\(04\)70071-7) |
| 年份 | 2004 |
| 期刊/会议 | Journal of Manufacturing Processes 6(2), 170–178 |
| Input | FDM 工艺参数（挤出温度、环境温度、丝径、对流换热系数）与 ABS 材料参数 |
| Task | 将熔接分为表面接触、颈部生长、界面扩散、分子随机化四步，只模拟颈部生长（润湿）。以集总热容一维传热模型求丝的冷却温度历程，并定义临界烧结温度（ABS 为 200°C，低于此温度颈部几乎不再生长）；将温度历程代入 Pokluda 修正的 Frenkel 烧结模型，输出无量纲颈部半径 y/a。粘度由旋转流变仪测得；表面张力由热台加显微相机记录两颗颗粒的颈部生长，用恒温实验拟合、升温实验验证。以两水平全因子设计加方差分析比较各参数，发现挤出温度比环境温度重要得多，对流换热系数影响显著。 |
| 参考价值与区别 | **参考价值**：直接对应 Stage 3 的 S3-Q2（相邻拼豆能否连接），并服务 S3-Q1 与 S3-Q4。① "传热模型给出温度历程、烧结模型给出颈部大小"的两段式框架可直接迁移：给定熨斗档位与时间，估算豆子接触处的温度历程，再积分颈部生长，以颈部大小超过阈值判断是否连上；② 热台加相机的双颗粒实验与流变仪测粘度，是标定拼豆材料参数的现成流程；③ 临界烧结温度的概念可用于定义有效熨烫时间；④ 全因子设计加方差分析可用于 S3-Q1 筛选主要熨烫因素。 **区别**：不直接预测连接强度，只以颈部大小作为指示，需补充拉伸或悬挂实验建立强度与颈部的关系；只考虑两个颗粒且假设初始接触，不适用于原本有空隙的对角相邻豆子；FDM 为熔融后冷却，拼豆为从上方加热，且豆子尺寸大一个数量级，集总热容假设可能不成立；材料为 ABS，拼豆通常为聚乙烯。文中表面张力温度系数写作 −0.00345 N/m·K，Lou 2021 引用为 0.000345，后者更合理。 |

### **28\. A Transient Updated Lagrangian Finite Element Formulation for Bond Formation in Fused Deposition Modeling Process（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | A Transient Updated Lagrangian Finite Element Formulation for Bond Formation in Fused Deposition Modeling Process（R. Lou, H. Li, J. Zhong, C. Zhang, D. Fang） |
| 链接 | [Paper](https://doi.org/10.1016/j.jmps.2021.104450) |
| 年份 | 2021 |
| 期刊/会议 | Journal of the Mechanics and Physics of Solids 152, 104450 |
| Input | 颗粒的初始排布与边界条件，以及随温度变化的粘度与表面张力（沿用 Bellehumeur 2004 的 ABS 参数） |
| Task | 将熔融聚合物视为高粘度、近似不可压缩、由表面张力（Young–Laplace）驱动的可变形体，以隐式更新拉格朗日有限元（Newmark 积分，颈部网格扭曲时重新划分）模拟颈部生长，形状自由演化。用 Bellehumeur 的恒温与升温实验验证（初始 y/a 取 0.2 吻合最好，并复现升温曲线的拐点）。数值实验表明：一排颗粒受邻居约束，颈部生长明显慢于两颗粒情形，最终被拉平成矩形；两层四颗粒时颈部向中心移动并挤出空隙；重力促进水平颈部、抑制竖直颈部，颗粒越大影响越大，但塌陷也越严重。 |
| 参考价值与区别 | **参考价值**：对应 S3-Q2、S3-Q3 与 S3-Q4。① 说明连接与否取决于局部排布：处于实心块中的豆子受四周约束，颈部生长较慢，因此连接模型应以邻居配置为输入，可为实心块、细颈、对角等配置分别标定修正系数；② 整排拉平与空隙被挤出的现象，为预测熨烫后变平、孔洞与空隙闭合（S3-Q3）提供物理依据；③ 重力的方向效应可类比熨斗压力：压力促进豆子之间的水平连接，但加剧压扁变形，构成 S3-Q4 选择熨烫参数时的取舍。 **区别**：二维平面应变，只做恒温，未与传热耦合；假设接触后界面立即完全愈合；计算量大，只适合离线生成修正系数，不适合放入优化循环；同样不直接给出连接强度。 |

### ---

**29\. Prediction of Interlayer Strength in Material Extrusion Additive Manufacturing（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Prediction of Interlayer Strength in Material Extrusion Additive Manufacturing（T. J. Coogan, D. O. Kazmer） |
| 链接 | [Paper](https://doi.org/10.1016/j.addma.2020.101368) |
| 年份 | 2020 |
| 期刊/会议 | Additive Manufacturing 35, 101368 |
| Input | 打印参数（熔体温度、层高、丝宽、打印速度），在线测得的熔体压力与温度，流变数据（Cross-WLF 粘度、平台模量） |
| Task | 将层间强度建模为 σ \= σ∞ · (W\_bond/W) · (χ/χ∞)（χ/χ∞ 不超过 1）。接触比例由压力驱动的紧密接触模型给出：W\_bond \= W · R\_c · (P\_contact · t\_p / η)^(1/5)，其中接触压力由喷头内在线流变仪实测；由于冷却很快，表面张力驱动的润湿可忽略。扩散比例由 reptation 与愈合理论给出：χ/χ∞ \= (∫ dt/τ\_weld(T))^(1/4)，τ\_weld \= η₀/(G\_N⁰ · M\_corr)，温度历程由二维有限差分传热模型计算，M\_corr \= 18 由实测强度拟合。以 16 组 HIPS 打印条件验证，预测与实测强度 R² \= 0.858。发现多数强度损失来自接触不足，仅低温时扩散成为限制；短时高温比长时稍低温更有利于扩散；截面边缘冷却更快、愈合更差；并演示了基于在线传感的实时弱层检测。 |
| 参考价值与区别 | **参考价值**：对应 Stage 3 的 S3-Q2 与 S3-Q3，并服务 S3-Q4、S3-Q5。① "强度 \= 接触 × 扩散"是目前最完整且经实验验证的连接强度模型，可补足 Bellehumeur 2004 只预测颈部大小的不足；② 熨烫是在熨斗压力下加热，压力驱动接触公式比表面张力润湿模型更贴近熨斗压住豆子的阶段，两者可串联：先由压力建立接触，再由表面张力在余热中继续长颈；③ 边缘愈合较差提示熨烫结果应依赖位置；④ 短时高温优于长时低温，为 S3-Q4 指明方向；⑤ 实时弱层检测可借鉴到 S3-Q5。 **区别**：针对 FDM 层间连接，压力由喷头产生且作用约 5–10 ms，而熨烫的压力与加热时间均长得多；材料为非晶态 HIPS，作者明确指出 PE 等半结晶聚合物的扩散受结晶抑制、界面强度还受结晶度影响，并伴随收缩与翘曲；需要在线流变仪与旋转流变仪测参数，拼豆实验需简化。 |

### **30\. Process-Structure-Property Effects on ABS Bond Strength in Fused Filament Fabrication（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Process-Structure-Property Effects on ABS Bond Strength in Fused Filament Fabrication（A. C. Abbott, G. P. Tandon, R. L. Bradford, H. Koerner, J. W. Baur） |
| 链接 | [Paper](https://doi.org/10.1016/j.addma.2017.11.002) |
| 年份 | 2018 |
| 期刊/会议 | Additive Manufacturing 19, 29–38 |
| Input | ABS 打印参数（挤出温度、打印速度、层高）与打印方向（XY、ZX） |
| Task | 以两水平全因子实验设计研究"打印参数 → 温度历程 → 截面结构 → 拉伸强度"。用红外相机记录结合线温度，并以埋入热电偶的 ABS 块建立红外读数与温度的标定曲线，测出结合线高于 Tg 的时间；以截面光学显微照片测量相邻丝的接触长度，并按丝高归一化；以数字图像相关测应变做拉伸测试；以方差分析判断显著因素（打印速度最显著）。发现归一化接触长度超过约 0.6 后，两种打印方向的强度均稳定在约 22 MPa；速度越快接触越短、强度越低；层高的影响取决于打印方向。 |
| 参考价值与区别 | **参考价值**：对应 Stage 3 的 S3-Q3，并服务 S3-Q1 与 S3-Q2。① 指出对强度最关键的几何量是归一化接触长度，且存在饱和阈值，拼豆可据此以"颈部宽度 ÷ 豆子直径"作为 S3-Q3 的核心预测量，并标定自己的阈值，使 S3-Q2 简化为阈值判断；② 截面显微测量接触长度的方法可作为 S3-Q3 的真值测量手段，与俯视照片配合；③ 红外相机加埋入热电偶的标定方法，可用于测量熨烫时豆子的真实温度（S3-Q1）；④ 全因子设计加方差分析可用于筛选熨烫参数；⑤ 结构不必完全致密也能达到满强度，与本项目"少用豆子"的目标一致。 **区别**：只给出经验关系，没有预测接触长度或强度的物理模型；材料为 ABS，过程为挤出后冷却；不涉及孔洞闭合、外观与颜色。 |

### ---

**31\. An Inverse Procedural Modeling Pipeline for SVBRDF Maps（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | An Inverse Procedural Modeling Pipeline for SVBRDF Maps（Y. Hu, C. He, V. Deschaintre, J. Dorsey, H. Rushmeier） |
| 链接 | [Paper (ACM)](https://doi.org/10.1145/3502431) |
| 年份 | 2022 |
| 期刊/会议 | ACM Transactions on Graphics 41(2), Article 18 |
| Input | 一组 SVBRDF 贴图（albedo、normal、roughness），以及少量用户笔画 |
| Task | 将材质层次分解为子材质树：以加入局部噪声频谱特征的 KNN matting（用户笔画引导）或实例检测加聚类进行分割；每个子材质以多层随机相位噪声程序化；分割掩码以 PPTBF 拟合（45 万掩码库检索最近邻，再用 Powell 与贝叶斯优化分别处理连续与离散参数），实例分布以按频率随机采样表示；最后加入可优化滤波参数，以 Gram 矩阵风格损失加 SSIM 损失进行可微渲染重组。得到不依赖预设材质图、可编辑、可任意分辨率生成的程序化材质。 |
| 参考价值与区别 | **参考价值**：对应 Stage 3 的 S3-Q4，并服务 S3-Q3、S3-Q5。熨烫后的拼豆作品可视为由重复单元组成的材质：每颗豆为一个实例，顶面、孔洞、颈部、空隙与晕染带为子材质，其尺寸即熔合模型预测的量；外观被压缩为少量参数后，选择熨烫参数即成为低维优化（可用贝叶斯优化）；Gram 加 SSIM 损失可在不要求逐像素对齐的情况下比较预测与实拍。 **区别**：不涉及任何制造过程，外观参数与熨烫参数的映射需自行建立；对密集重叠元素、复杂轮廓与有语义的结构效果差。 |

### **32\. Practical Inverse Rendering of Textured and Translucent Appearance（B）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Practical Inverse Rendering of Textured and Translucent Appearance（P. Weier, J. Riviere, R. Guseinov, S. Garbin, P. Slusallek, B. Bickel, T. Beeler, D. Vicini） |
| 链接 | [Paper (ACM)](https://doi.org/10.1145/3730855) |
| 年份 | 2025 |
| 期刊/会议 | ACM Transactions on Graphics 44(4)（SIGGRAPH 2025） |
| Input | 已知几何与光照下的多视角、多光照照片 |
| Task | 提出 Laplacian mipmapping：优化纹理的拉普拉斯金字塔各层，并按光线微分读取 mipmap，作为几乎无需调参、与分辨率无关的预条件方法；提出带 2D 纹理参数的可微路径追踪次表面散射，以 path replay backpropagation 并将整条散射路径的梯度合并计算，提速 20%–60%；优化有效反照率以降低非线性，出射时使用漫射边界降低方差；应用于 13 相机、14 灯 OLAT 的人脸外观重建，使用实测 IES 灯具分布，分两阶段优化。 |
| 参考价值与区别 | **参考价值**：作为 Stage 3 的拓展，服务 S3-Q3、S3-Q4 与 S3-Q8。拼豆为塑料且常为半透明，熔合后的光泽与透光感需次表面散射与可微渲染才能真实预测；从少量光照下的测试板照片反推 albedo、roughness、normal，可作为熔合程度的测量与校准手段；Laplacian mipmapping 可用于同时含整体图案与单颗豆细节的外观优化。 **区别**：不涉及制造过程；需已知几何与标定灯光；计算成本高，不适合作为只有几个参数的熨烫参数选择的主方法。 |

### **33\. Optimization of Fused Filament Fabrication Process Parameters under Uncertainty to Maximize Part Geometry Accuracy（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Optimization of Fused Filament Fabrication Process Parameters under Uncertainty to Maximize Part Geometry Accuracy（P. Nath, J. D. Olson, S. Mahadevan, Y.-T. T. Lee） |
| 链接 | [Paper](https://doi.org/10.1016/j.addma.2020.101331) |
| 年份 | 2020 |
| 期刊/会议 | Additive Manufacturing 35, 101331 |
| Input | FDM 工艺参数（挤出温度、挤出速度、层厚）与少量实测零件厚度 |
| Task | 以热–力单向耦合有限元模型模拟打印（按线激活单元）；以拉丁超立方采样 25 组参数训练高斯过程代理模型（留一交叉验证误差小于 7%）；按 Kennedy–O'Hagan 框架将实测表示为模型预测加模型偏差加测量误差，仅用 3 组参数、每组 3 个零件，以 MCMC 校准偏差分布；以误差均值与标准差加权的稳健设计优化工艺参数，并给出误差与打印时间的 Pareto 前沿，均经实物验证。 |
| 参考价值与区别 | **参考价值**：对应 Stage 3 的 S3-Q8（持续更新熔合模型），并服务 S3-Q4、S3-Q5。① KOH 框架可将实测与预测之差分解为模型偏差与测量误差，上一轮后验作为下一轮先验持续更新；② 校准出的正常偏差分布可用于判定缺陷：只有超出该分布的偏差才视为缺陷；③ 稳健设计提示修改 layout 时应使连接在熨烫波动下仍大概率成立；④ 高斯过程代理加拉丁超立方采样可用少量测试板建立熨烫参数模型。 **区别**：优化对象为工艺参数而非设计；数据少，模型偏差取为与输入无关的常数，作者指出应发展为输入相关；零件形状简单，只关注厚度。 |

### **34\. Data-Driven Process Optimization of Fused Filament Fabrication based on In Situ Measurements（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Data-Driven Process Optimization of Fused Filament Fabrication based on In Situ Measurements（X. Guidetti, M. Kühne, Y. Nagel, E. C. Balta, A. Rupenyan, J. Lygeros） |
| 链接 | [Paper](https://doi.org/10.1016/j.ifacol.2023.10.1232) |
| 年份 | 2023 |
| 期刊/会议 | IFAC-PapersOnLine 56(2), 4713–4718 |
| Input | FDM 打印参数（打印速度、挤出倍率）与打印过程中的激光测距扫描 |
| Task | 在打印头上加装激光测距传感器，逐层扫描并计算 ISO 4287 粗糙度 Ra 作为质量代理指标；验证其可重复性（变异系数 0.13%）、单线代表整层、与数字显微镜误差 7.1%；证明粗糙度与杨氏模量和拉伸强度相关；以约束贝叶斯优化在粗糙度约束下最大化打印速度，用置信阈值在保守与激进采集策略间切换，31 次实验后得到 3 倍于专家设定的合格打印速度。 |
| 参考价值与区别 | **参考价值**：服务 Stage 3 的 S3-Q4、S3-Q5、S3-Q8。① 以易测的代理指标（拼豆中为照片测得的颈部宽度、孔洞闭合率、表面起伏）替代破坏性测试，但需先验证代理指标与真实强度的关联；② 测量可重复性与准确性的验证流程可直接借鉴；③ 约束贝叶斯优化适合"保证全部连通的前提下熨烫时间最短"一类问题，也可用于主动选择下一块测试板的实验条件。 **区别**：优化对象为工艺参数；代理指标为全局平均值，不定位缺陷；只有两个参数。 |

### **35\. Improving Geometric Accuracy of 3D Printed Parts Using 3D Metrology Feedback and Mesh Morphing（S）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Improving Geometric Accuracy of 3D Printed Parts Using 3D Metrology Feedback and Mesh Morphing（M. Jadayel, F. Khameneifar） |
| 链接 | [Paper](https://doi.org/10.3390/jmmp4040112) |
| 年份 | 2020 |
| 期刊/会议 | Journal of Manufacturing and Materials Processing 4(4), 112 |
| Input | 零件 CAD 网格，以及同一参数下打印的多个牺牲件的 3D 扫描 |
| Task | 打印 5 个牺牲件并以结构光扫描；以 ICP 与 CAD 配准，求每个顶点的偏差向量；对每件偏差场做 Laplacian 平滑（网格上的热扩散）去除高频噪声，再对 5 件取平均得到系统偏差场；以"原网格减平均偏差场"变形网格（底面固定，剔除超过 500 µm 的异常值）后重新打印。五件平均补偿使 99 分位误差降低 68% 并满足全部公差；仅用一件补偿只改善 31%，且把该件的随机缺陷反向引入了补偿件。 |
| 参考价值与区别 | **参考价值**：对应 Stage 3 的 S3-Q7（根据成品反向优化 layout），并服务 S3-Q8。① 偏差由系统误差与随机误差组成，只能补偿系统部分；手工熨烫随机性大，应对同一 layout 熨多份并取平均，只修改反复出现的缺陷；② 连续的反向预变形需转化为离散修改：反复断开处加桥接豆或加宽线条，反复晕染处换过渡色或留空，整体膨胀则在 Stage 1 预先缩小图案；③ 平均偏差可修正模型的系统误差，各件方差可量化熨烫随机性。 **区别**：补偿为连续几何变形，拼豆为离散单元；只处理几何精度，不涉及连接强度与外观。 |

### **36\. On Iterative Pre-Compensation of 3D Laser-Printed Micro-Optical Components Using Confocal-Optical Microscopy（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | On Iterative Pre-Compensation of 3D Laser-Printed Micro-Optical Components Using Confocal-Optical Microscopy（J. Weinacker, S. Kalt, P. Kiefer, P. Rietz, M. Wegener） |
| 链接 | [Paper](https://doi.org/10.1002/adfm.202309356) · [Code (Quandalf)](https://gitlab.kit.edu/kit/aph/AGW/quandalf.git) |
| 年份 | 2024 |
| 期刊/会议 | Advanced Functional Materials 34(12), 2309356 |
| Input | 2.5D 微光学元件的设计高度图与打印后的共聚焦显微高度测量 |
| Task | 以基底区域拟合平面校正倾斜；以高度直方图阈值分离结构与基底并求重心做粗定位；以互相关依次求旋转、横向缩放与平移完成精对齐；逐像素计算差值，只选用质量好的测量并取平均；对差值依次做异常（大梯度或大差值）标记、扩张、置空插值、边缘外推与高斯滤波；新设计 \= 上一版设计 − 过滤后差值。一次补偿即显著降低误差并消除拼接缝，第二次补偿提升有限，瓶颈在测量本身。 |
| 参考价值与区别 | **参考价值**：服务 Stage 3 的 S3-Q5 与 S3-Q7。熨烫后的拼豆作品同为 2.5D，其流程几乎可直接用于照片：以背景校正拍摄倾斜与光照，以阈值分离豆子与空格，以互相关配准到网格，且求得的缩放系数即整体膨胀率；逐像素差值可汇总到每颗豆；作品边缘受热不同，应单独处理；"一到两轮迭代即饱和"的经验说明拼豆补偿只需熨少数几轮。 **区别**：补偿为连续高度修改；针对微米级光学元件与共聚焦测量；不涉及连接强度。 |

### **37\. Two-Dimensional Digital Image Correlation for In-Plane Displacement and Strain Measurement: A Review（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Two-Dimensional Digital Image Correlation for In-Plane Displacement and Strain Measurement: A Review（B. Pan, K. Qian, H. Xie, A. Asundi） |
| 链接 | [Paper](https://iopscience.iop.org/article/10.1088/0957-0233/20/6/062001/pdf) |
| 年份 | 2009 |
| 期刊/会议 | Measurement Science and Technology 20(6), 062001，DOI 10.1088/0957-0233/20/6/062001 |
| Input | 平面试件变形前后的照片（表面带随机散斑） |
| Task | 综述 2D 数字图像相关（DIC）：以随机散斑作为标记，在变形前后图像中进行子区匹配（零均值归一化互相关等），配合形函数与 Newton–Raphson 类迭代达到亚像素精度，再以局部最小二乘拟合由位移场求应变场；讨论平面试件、相机垂直、离面运动与镜头畸变等前提与误差来源。（本条未读全文，基于该综述的标准内容整理；出处信息取自 Abbott 2018 的参考文献列表。） |
| 参考价值与区别 | **参考价值**：对应 Stage 3 的 S3-Q6（识别薄弱区域），并服务 S3-Q8 与 Stage 2 的力学模型验证。单张照片只能发现几何缺陷；对作品施加小载荷并拍摄前后照片，可由应变集中或相邻豆之间的相对位移识别薄弱连接，得到每个连接的刚度地图，用于验证 Stage 2 预测的最弱连接并校准"颈部宽度 → 连接强度"模型。豆子网格的周期性会使相关匹配错位，可喷涂可擦除的随机散斑，或直接追踪每颗豆的中心，得到豆子邻接图中各节点的位移。 **区别**：只测刚度与变形，不直接给出强度；2D DIC 无法处理离面弯曲，需立体 DIC。 |

### **38\. Bayesian Calibration of Computer Models（A）**

| 字段 | 内容   |
| :---- | :---- |
| 名称 | Bayesian Calibration of Computer Models（M. C. Kennedy, A. O'Hagan） |
| 链接 | [Paper](https://www.asc.ohio-state.edu/statistics/comp_exp/jour.club/kennedy01.pdf) |
| 年份 | 2001 |
| 期刊/会议 | Journal of the Royal Statistical Society: Series B 63(3), 425–464 |
| Input | 计算机模型与少量实测数据 |
| Task | 提出含模型偏差项的贝叶斯校准框架：实测 \= 模型预测（含待定参数）+ 模型偏差函数 \+ 观测误差，以高斯过程表示模型偏差，联合推断参数与偏差的后验分布并用于预测。（本条未读全文，出处信息取自 Nath 2020 的参考文献列表。） |
| 参考价值与区别 | **参考价值**：对应 Stage 3 的 S3-Q8，是持续更新熔合模型的理论框架原文，Nath 2020（33）为其在增材制造中的应用。模型偏差可写为熨烫条件与局部邻居配置的函数，提示模型在何处需要改进结构。 **区别**：为通用统计方法，不涉及具体制造过程。 |

## ---

**小结 / Summary**

现有工作可分为五类：限色或低分辨率图像生成、分辨率变换与视觉抽象（1、3、15–21），考虑可制造性约束的计算设计（2、4、6、8–13、24、26），制造过程建模与自动化（5、7、14、27–30），用于连通性检查、断裂与结构分析的算法（22、23、25），以及外观反推、制造反馈测量与模型校准（31–38）。其中，部分工作已处理离散媒介的连通性（2、4、8–10），但均通过几何构造或刚性连接实现；热过程建模（5）则针对连续材料；聚合物熔接与连接强度研究（27–30）针对 FDM 丝材的冷却过程，未涉及从上方加热的离散颗粒阵列及其外观。目前尚无工作对热熔合如何改变离散布局的外观与连通性进行建模，并据此优化设计。