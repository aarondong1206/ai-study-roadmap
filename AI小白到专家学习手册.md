# 从零基础到人工智能专家学习手册

最后联网核对日期：2026-05-17  
适用对象：不会 Python、希望系统进入人工智能领域的人  
建议总时长：12-24 个月形成强实战能力；2-4 年持续深耕形成专家级判断力

---

## 0. 先说清楚：什么叫“人工智能专家”

很多人把“会调 ChatGPT、会跑几个模型”误认为 AI 专家。真正的 AI 专家至少具备这 6 种能力：

1. 能把现实问题转成数据问题或模型问题：知道什么时候该用规则、检索、传统机器学习、深度学习、LLM、RAG、Agent，什么时候不该用 AI。
2. 能写可靠代码：Python、数据处理、实验脚本、训练脚本、服务接口、测试、版本管理。
3. 能理解模型原理：线性模型、树模型、神经网络、反向传播、优化、泛化、Transformer、评估方法。
4. 能完成端到端项目：数据获取、清洗、建模、评估、部署、监控、迭代。
5. 能读论文并复现关键想法：不是只看摘要，而是能找出假设、实验设置、指标、失败点。
6. 能负责地使用 AI：理解偏见、隐私、安全、幻觉、版权、成本、风险管理。

本手册的路线是“先能做，再做对，再做深”。你不需要一开始就把数学吃透，但每个阶段都必须写代码、做项目、复盘错误。

---

## 1. 总路线图

### 1.1 四条主线

你要同时推进四条线，但每个阶段权重不同：

| 主线 | 你要获得的能力 | 初期权重 | 后期权重 |
|---|---|---:|---:|
| 编程与工程 | Python、Git、调试、测试、API、部署 | 高 | 高 |
| 数学与统计 | 线代、概率、微积分、优化、统计推断 | 中 | 高 |
| 机器学习与深度学习 | 模型、训练、评估、调参、误差分析 | 中 | 高 |
| 产品与研究判断 | 选型、论文、系统设计、风险、业务指标 | 低 | 高 |

### 1.2 时间表

如果你每周学习 10 小时：

| 时间 | 阶段 | 目标 |
|---|---|---|
| 第 1-6 周 | Python 入门 | 能独立写小程序、读报错、使用 Jupyter |
| 第 7-10 周 | 数据分析工具 | 会用 NumPy、pandas、matplotlib 做 EDA |
| 第 11-18 周 | 数学基础 | 掌握 AI 常用线代、概率、微积分、优化直觉 |
| 第 19-28 周 | 传统机器学习 | 会用 scikit-learn 完成分类、回归、聚类与评估 |
| 第 29-42 周 | 深度学习与 PyTorch | 能训练 CNN、MLP、简单 NLP 模型，理解反向传播 |
| 第 43-56 周 | LLM、RAG、Agent | 能做可评估的 RAG/Agent 原型，懂 Transformer 基础 |
| 第 57-72 周 | MLOps 与生产化 | 能把模型变成服务，做日志、监控、评估、迭代 |
| 第 73 周以后 | 专家方向 | 选择 NLP/LLM、CV、多模态、推荐、RL、AI Infra、AI Safety 等方向深挖 |

如果你每周学习 20 小时，可以把前 12 个月压缩到 7-9 个月，但不要压缩项目实践。

---

## 2. 每周学习方法

### 2.1 学习循环

每个知识点都按这个顺序走：

1. 看一节课或读一章。
2. 手写最小代码，不复制粘贴。
3. 改一个参数，看结果怎么变。
4. 记录一个“我原来误解了什么”。
5. 做一个小项目或练习题。
6. 用自己的话写 200-500 字总结。

### 2.2 一周模板

| 天 | 任务 |
|---|---|
| 周一 | 看视频或读教材，写概念笔记 |
| 周二 | 跟写代码，跑通示例 |
| 周三 | 不看答案重写一遍 |
| 周四 | 做练习或小项目 |
| 周五 | 调试、补缺口、整理 GitHub |
| 周六 | 做阶段项目的一部分 |
| 周日 | 复盘、写周报、安排下周 |

### 2.3 学习记录模板

每周写一次：

```markdown
## 本周主题

## 我完成了什么

## 我卡住了什么

## 我现在能解释的概念

## 我写过的代码链接

## 下周最重要的 3 件事
```

---

## 3. 阶段一：Python 零基础入门

建议时间：4-6 周  
阶段目标：能独立写 Python 小程序，能读懂基础脚本，能使用 Jupyter Notebook。

### 3.1 必学内容

- 变量、数字、字符串、布尔值
- 条件语句：`if / elif / else`
- 循环：`for`、`while`
- 列表、字典、集合、元组
- 函数、参数、返回值
- 文件读写
- 异常处理
- 模块与包
- 基础面向对象
- 调试：看懂报错、打印变量、拆小问题

### 3.2 主要资源

首选：

- [Harvard CS50P: Introduction to Programming with Python](https://cs50.harvard.edu/python/)  
  官方课程页面，有讲义、练习和最终项目。CS50P 官方说明中写明它面向“有或没有编程经验”的学习者，并且课程专注 Python。
- [CS50P YouTube 播放列表](https://www.youtube.com/playlist?list=PLhQjrBD2T3817j24-GogXmWqO5Q5vYy0V)

辅助：

- [Python.org: Python For Beginners](https://www.python.org/about/gettingstarted/)
- [Kaggle Learn Python](https://www.kaggle.com/learn/python)

### 3.3 学习任务

第 1 周：

- 安装 Python、VS Code、JupyterLab。
- 跑通 `print("hello ai")`。
- 学会在终端运行 `.py` 文件。
- 完成 CS50P Week 0。

第 2 周：

- 完成条件语句和循环。
- 写一个 BMI 计算器。
- 写一个猜数字游戏。

第 3 周：

- 学列表、字典、函数。
- 写一个联系人管理程序：增删改查联系人。

第 4 周：

- 学文件读写和异常。
- 写一个 CSV 成绩统计脚本：读取成绩文件，输出均值、最高分、最低分。

第 5-6 周：

- 学面向对象和第三方库。
- 完成一个 200-400 行的小项目。

### 3.4 阶段项目

项目 A：个人学习记账本  
功能：

- 输入学习日期、主题、时长、完成内容。
- 保存到 CSV。
- 统计每周学习时长。
- 输出最常学的主题。

项目 B：文件整理工具  
功能：

- 扫描一个文件夹。
- 按后缀把文件移动到不同子目录。
- 支持预览模式，不直接移动。

### 3.5 验收标准

你能做到下面这些，就可以进入下一阶段：

- 看到 Python 报错能定位到是哪一行。
- 能独立写函数。
- 能读写 CSV 或 TXT 文件。
- 能解释列表和字典的区别。
- 能把一个大任务拆成 3-5 个小函数。

---

## 4. 阶段二：数据分析与科学计算

建议时间：3-4 周  
阶段目标：能用 Python 处理表格数据、画图、做初步分析。

### 4.1 必学内容

- Jupyter Notebook / JupyterLab
- NumPy 数组、向量化计算、广播
- pandas `DataFrame`
- 缺失值、重复值、异常值
- 分组统计、透视表、合并表
- matplotlib / seaborn 可视化
- 数据分析报告结构

### 4.2 主要资源

- [pandas 官方 Getting Started Tutorials](https://pandas.pydata.org/docs/getting_started/intro_tutorials/index.html)
- [Kaggle Learn Pandas](https://www.kaggle.com/learn/pandas)
- [Kaggle Learn Data Visualization](https://www.kaggle.com/learn/data-visualization)

### 4.3 学习任务

第 1 周：

- 学 `Series`、`DataFrame`。
- 练习读取 CSV、查看前几行、查看列类型。
- 做 10 个筛选、排序、分组操作。

第 2 周：

- 学缺失值处理。
- 学 `groupby`、`merge`、`pivot_table`。
- 用真实数据做一次 EDA。

第 3 周：

- 学可视化。
- 输出一份 5-8 页的数据分析报告。

第 4 周：

- 学 SQL 基础，至少掌握 `SELECT`、`WHERE`、`GROUP BY`、`JOIN`。
- 用 pandas 复现 SQL 的几个查询结果。

### 4.4 阶段项目

项目：电商订单分析  
要求：

- 数据字段包括订单号、用户、商品、价格、数量、时间、城市。
- 输出总销售额、客单价、城市分布、热销商品、复购用户。
- 画出至少 5 张图。
- 写一份结论：业务上下一步应该做什么。

### 4.5 验收标准

- 能独立读入 CSV 并清洗。
- 能解释“缺失值”和“异常值”的处理选择。
- 能用图说明一个结论。
- 能写出一份别人能看懂的数据分析报告。

---

## 5. 阶段三：AI 必备数学

建议时间：8-10 周  
阶段目标：不追求数学竞赛式熟练，而是能理解模型公式、损失函数、梯度、概率和评估指标。

### 5.1 学习原则

数学不要孤立学。每学一个概念，就问：

- 它在模型中出现在哪里？
- 它对应什么代码？
- 它改变以后模型行为会怎样？

### 5.2 线性代数

必学：

- 向量、矩阵、张量
- 点积、矩阵乘法
- 线性变换
- 秩、基、维度
- 特征值、特征向量
- 奇异值分解 SVD
- 最小二乘

资源：

- [MIT 18.06 Linear Algebra 视频课](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/video_galleries/video-lectures/)
- [3Blue1Brown: Essence of Linear Algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr)

练习：

- 用 NumPy 写矩阵乘法、转置、逆矩阵、特征值分解。
- 用最小二乘拟合一条直线。
- 用 SVD 压缩一张灰度图片。

### 5.3 微积分与优化

必学：

- 函数、导数、偏导
- 链式法则
- 梯度
- 梯度下降
- 学习率
- 局部最优、鞍点

资源：

- [3Blue1Brown: Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)
- [StatQuest 视频索引](https://statquest.org/video_index.html)

练习：

- 手写一元函数的梯度下降。
- 手写线性回归的损失函数和梯度下降。
- 画出学习率过大、过小、合适时的 loss 曲线。

### 5.4 概率与统计

必学：

- 随机变量
- 条件概率、贝叶斯公式
- 常见分布：伯努利、二项、正态
- 均值、方差、标准差
- 置信区间、假设检验的直觉
- 最大似然估计
- 采样、偏差、方差

资源：

- [Khan Academy: Statistics and Probability](https://www.khanacademy.org/math/statistics-probability)
- [StatQuest 视频索引](https://statquest.org/video_index.html)

练习：

- 用 Python 模拟抛硬币、掷骰子、正态分布。
- 用模拟解释大数定律。
- 用朴素贝叶斯做一个简易文本分类器。

### 5.5 验收标准

- 能解释矩阵乘法为什么适合批量计算。
- 能说清楚梯度下降在优化什么。
- 能解释过拟合和欠拟合。
- 能解释训练集、验证集、测试集的区别。
- 能用代码实现一个最小线性回归。

---

## 6. 阶段四：传统机器学习

建议时间：8-10 周  
阶段目标：掌握常见机器学习任务、模型、评估与误差分析，能完成结构化数据项目。

### 6.1 必学内容

模型：

- 线性回归、逻辑回归
- KNN
- 决策树、随机森林、梯度提升树
- 朴素贝叶斯
- SVM 基础
- K-means、PCA

方法：

- 特征工程
- 标准化、归一化
- 训练/验证/测试划分
- 交叉验证
- 混淆矩阵、Precision、Recall、F1、ROC-AUC
- 数据泄漏
- 类别不平衡
- 超参数搜索
- 误差分析

### 6.2 主要资源

- [DeepLearning.AI Machine Learning Specialization](https://www.deeplearning.ai/specializations/machine-learning/)
- [Google Machine Learning Crash Course](https://developers.google.com/machine-learning/crash-course)
- [scikit-learn Getting Started](https://scikit-learn.org/stable/getting_started.html)
- [Kaggle Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning)
- [Kaggle Feature Engineering](https://www.kaggle.com/learn/feature-engineering)

进阶资源：

- [Stanford CS229 Summer 2019 课程页](https://cs229.stanford.edu/syllabus-summer2019.html)
- [Stanford CS229 Summer 2019 YouTube 播放列表](https://www.youtube.com/playlist?list=PLoROMvodv4rNH7qL6-efu_q2_bPuy0adh)

### 6.3 学习任务

第 1-2 周：

- 用 scikit-learn 跑通回归和分类。
- 学 `fit`、`predict`、`score`。
- 学 Pipeline，避免数据泄漏。

第 3-4 周：

- 学逻辑回归、树模型、随机森林。
- 对比模型效果，不只看准确率。

第 5-6 周：

- 学交叉验证、调参、特征工程。
- 写误差分析报告。

第 7-8 周：

- 学无监督学习：K-means、PCA。
- 完成一个 Kaggle 小比赛或公开数据项目。

第 9-10 周：

- 复盘传统 ML 项目。
- 把 notebook 整理成可复现项目。

### 6.4 阶段项目

项目 A：房价预测  
要求：

- 做 EDA。
- 建立 baseline。
- 对比线性回归、随机森林、梯度提升树。
- 做特征工程。
- 输出误差分析。

项目 B：用户流失预测  
要求：

- 处理类别不平衡。
- 用 Recall、Precision、F1、AUC 做评估。
- 给出业务策略：如何干预高风险用户。

### 6.5 验收标准

- 你能解释为什么不能只看 accuracy。
- 你能发现和避免数据泄漏。
- 你能用 Pipeline 组织预处理和模型。
- 你能写一份模型报告：数据、方法、指标、错误样本、下一步。

---

## 7. 阶段五：深度学习与 PyTorch

建议时间：10-12 周  
阶段目标：理解神经网络如何训练，能用 PyTorch 做 CV/NLP 基础项目。

### 7.1 必学内容

- 张量与自动求导
- 神经网络层：Linear、Conv、Embedding、Normalization
- 激活函数：ReLU、Sigmoid、Tanh、GELU
- 损失函数：MSE、Cross Entropy
- 优化器：SGD、Adam、AdamW
- Batch、Epoch、Learning Rate
- Dropout、BatchNorm、LayerNorm
- CNN、RNN 基础
- 训练循环、验证循环、保存模型
- GPU 与 mixed precision 基础

### 7.2 主要资源

- [PyTorch 60 Minute Blitz](https://docs.pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html)
- [Dive into Deep Learning 中文版](https://zh.d2l.ai/)
- [DeepLearning.AI Deep Learning Specialization](https://www.deeplearning.ai/specializations/deep-learning/)
- [fast.ai Practical Deep Learning for Coders](https://course.fast.ai/)
- [fast.ai YouTube 播放列表](https://www.youtube.com/playlist?list=PLfYUBJiXbdtSvpQjSnJJ_PmDQB_VyT5iU)
- [Andrej Karpathy: Neural Networks Zero to Hero](https://github.com/karpathy/nn-zero-to-hero)

中文辅助：

- [动手学深度学习中文版](https://zh.d2l.ai/)
- [李宏毅 2023 春机器学习课程 B 站授权版](https://www.bilibili.com/video/BV1TD4y137mP/)

### 7.3 学习任务

第 1-2 周：

- 学 PyTorch Tensor。
- 学 autograd。
- 写一个线性回归训练循环。

第 3-4 周：

- 写 MLP 做 MNIST 分类。
- 记录训练 loss、验证 accuracy。
- 试不同学习率。

第 5-6 周：

- 学 CNN。
- 做 CIFAR-10 或猫狗分类。
- 学数据增强。

第 7-8 周：

- 学 Embedding、RNN、文本分类。
- 做情感分析或垃圾短信分类。

第 9-10 周：

- 学训练技巧：早停、权重衰减、学习率调度。
- 用 TensorBoard 或 Weights & Biases 记录实验。

第 11-12 周：

- 复现一个小论文或 D2L 章节。
- 把训练代码整理成项目结构。

### 7.4 阶段项目

项目 A：图像分类器  
要求：

- 数据集至少 2 个类别，每类至少 100 张图。
- 使用迁移学习。
- 输出混淆矩阵。
- 做错误样本分析。
- 写部署方案。

项目 B：从零写一个小神经网络  
要求：

- 不使用 PyTorch autograd。
- 手写前向传播、反向传播、梯度更新。
- 在简单数据集上跑通。

### 7.5 验收标准

- 能解释反向传播的作用。
- 能写 PyTorch `Dataset` 和 `DataLoader`。
- 能独立写训练循环。
- 能判断 loss 不下降的常见原因。
- 能保存和加载模型。

---

## 8. 阶段六：现代 NLP、LLM、RAG 与 Agent

建议时间：10-14 周  
阶段目标：理解 Transformer 与 LLM 应用开发，能做可评估、可迭代的 RAG/Agent 系统。

### 8.1 必学内容

基础：

- Tokenization
- Embedding
- Attention
- Transformer Encoder/Decoder
- 预训练、微调、指令微调
- Prompt engineering
- RAG：检索、切分、向量库、重排、引用
- Agent：工具调用、状态、规划、失败恢复
- Evals：自动评估、人工评估、回归测试

工程：

- API 调用
- JSON 结构化输出
- Function calling / tool use
- 向量数据库
- 文档解析
- 安全与权限
- 成本与延迟优化

### 8.2 主要资源

- [Hugging Face LLM/NLP Course](https://huggingface.co/course)
- [Hugging Face Agents Course](https://huggingface.co/learn/agents-course)
- [Stanford CS224N: Natural Language Processing with Deep Learning](https://web.stanford.edu/class/cs224n/)
- [Stanford CS224N 2023 YouTube 播放列表](https://www.youtube.com/playlist?list=PLoROMvodv4rMFqRtEuo6SGjY4XbRIVRd4)
- [Stanford CS25: Transformers United](https://web.stanford.edu/class/cs25/)
- [Stanford CS336: Language Modeling from Scratch](https://cs336.stanford.edu/)
- [OpenAI API Quickstart](https://platform.openai.com/docs/quickstart)
- [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)
- [OpenAI Agents Guide](https://platform.openai.com/docs/guides/agents)
- [OpenAI Cookbook: evaluation flywheel](https://cookbook.openai.com/examples/evaluation/building_resilient_prompts_using_an_evaluation_flywheel)

### 8.3 学习任务

第 1-2 周：

- 学 Token、Embedding、Attention。
- 手写一个小型 self-attention。
- 用 3Blue1Brown 和 Hugging Face 建立直觉。

第 3-4 周：

- 用 Transformers 库做文本分类。
- 学 tokenizer、model、trainer。
- 对比 zero-shot、few-shot、fine-tuning。

第 5-6 周：

- 做第一个 RAG。
- 用 20-50 篇文档构建知识库。
- 输出答案时必须带来源。

第 7-8 周：

- 加入重排、查询改写、引用校验。
- 建立 30-100 条测试集。
- 做 RAG eval。

第 9-10 周：

- 做一个工具调用 Agent。
- 让模型能调用计算器、搜索、数据库或本地函数。
- 加入失败重试和日志。

第 11-14 周：

- 学 LLM 系统优化：缓存、并发、流式输出、成本控制。
- 读 3-5 篇 LLM 相关论文。
- 整理成可展示项目。

### 8.4 阶段项目

项目 A：个人知识库 RAG 助手  
要求：

- 支持 PDF/Markdown/TXT。
- 每个答案都给出处。
- 有“找不到答案”的能力。
- 有 50 条问题测试集。
- 记录准确率、引用正确率、拒答正确率。

项目 B：数据分析 Agent  
要求：

- 用户上传 CSV。
- Agent 能查看字段、生成分析计划、执行 pandas 代码、输出图表。
- 对危险代码做限制。
- 输出分析过程日志。

### 8.5 验收标准

- 能解释 Transformer 的输入输出。
- 能解释 RAG 为什么能减少但不能消灭幻觉。
- 能设计一个 eval 数据集。
- 能判断回答质量变差是检索问题、提示词问题、模型问题还是数据问题。
- 能做一个可演示的 LLM 应用。

---

## 9. 阶段七：选择专家方向

建议时间：8-16 周起步，然后长期深耕  
阶段目标：从“全都了解一点”进入“一个方向能做深”。

### 9.1 NLP / LLM 方向

适合：文本、问答、知识库、客服、办公自动化、代码助手、智能体。  
要学：

- Transformer 细节
- 预训练数据
- SFT、DPO、RLHF/RLAIF 基础
- RAG 评估
- 长上下文
- Tool use / Agents
- 推理优化

推荐资源：

- [Stanford CS224N](https://web.stanford.edu/class/cs224n/)
- [Stanford CS336](https://cs336.stanford.edu/)
- [Hugging Face LLM Course](https://huggingface.co/course)

项目：

- 训练一个小 GPT。
- 做领域 RAG。
- 做客服 Agent 并建立评估集。

### 9.2 计算机视觉方向

适合：图像识别、检测、分割、工业质检、医学影像、自动驾驶。  
要学：

- CNN、ViT
- Detection：Faster R-CNN、YOLO 系列思想
- Segmentation：U-Net、Mask R-CNN、SAM 思想
- 数据增强
- 标注质量
- 多模态视觉语言模型

推荐资源：

- [Stanford CS231n 官方课程页](https://cs231n.stanford.edu/)
- [Stanford CS231N 2025 YouTube 播放列表](https://www.youtube.com/playlist?list=PLoROMvodv4rOmsNzYBMe0gJY2XS8AQg16)

项目：

- 工业缺陷检测。
- 医学图像分割。
- 商品图片相似检索。

### 9.3 推荐系统方向

适合：电商、内容平台、广告、音乐视频推荐。  
要学：

- 协同过滤
- 矩阵分解
- 召回、排序、重排
- Embedding
- Wide & Deep、DeepFM、双塔模型
- 在线实验 A/B test

推荐资源：

- [Coursera Recommender Systems Specialization](https://www.coursera.org/specializations/recommender-systems)

项目：

- MovieLens 推荐系统。
- 新闻推荐。
- 商品召回和排序两阶段系统。

### 9.4 强化学习方向

适合：机器人、游戏、控制、自动决策、对齐研究。  
要学：

- MDP
- Value iteration、Policy iteration
- Q-learning
- Policy gradient
- Actor-Critic
- Offline RL
- RLHF 关联概念

推荐资源：

- [UC Berkeley CS285 Deep Reinforcement Learning](https://rail.eecs.berkeley.edu/deeprlcourse/)

项目：

- CartPole、LunarLander。
- 简单交易或资源调度环境。
- 用 RL 优化一个模拟控制问题。

### 9.5 AI 工程与 MLOps 方向

适合：把模型稳定落地、服务化、监控、成本优化。  
要学：

- FastAPI
- Docker
- CI/CD
- 数据版本管理
- 实验管理
- 模型注册
- 监控与告警
- A/B test
- 推理服务优化
- LLM eval 与灰度发布

推荐资源：

- [Full Stack Deep Learning 2022](https://fullstackdeeplearning.com/course/2022/)
- [Made With ML: MLOps Course](https://madewithml.com/courses/mlops/)

项目：

- 把一个 ML 模型部署为 API。
- 建一个模型监控面板。
- 建一个 LLM 应用的离线评估和线上日志系统。

### 9.6 AI 安全、治理与责任 AI

适合：高风险行业、企业 AI 管理、模型评估、安全红队。  
要学：

- 偏见与公平性
- 隐私与数据治理
- 幻觉与误导
- 安全评估
- 风险分类
- 合规与审计

推荐资源：

- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework)
- [Stanford HAI 2026 AI Index Report](https://hai.stanford.edu/ai-index/2026-ai-index-report)

项目：

- 为一个 RAG 系统写风险评估报告。
- 建立红队测试集。
- 为企业内部 AI 助手设计使用规范。

---

## 10. 阶段八：生产化与作品集

建议时间：8-12 周  
阶段目标：你不只是能训练模型，还能让别人使用、复现、评估你的系统。

### 10.1 必学内容

- Git 和 GitHub
- 项目结构
- 配置文件
- 日志
- 单元测试
- FastAPI
- Docker
- 数据版本管理
- 实验记录
- 模型评估报告
- 简单前端或 Gradio/Streamlit
- 云部署基础

### 10.2 一个合格 AI 项目的结构

```text
project-name/
  README.md
  requirements.txt 或 pyproject.toml
  data/
  notebooks/
  src/
    data/
    features/
    models/
    evaluate/
    app/
  tests/
  configs/
  reports/
  scripts/
```

### 10.3 README 必须包含

- 项目解决什么问题
- 数据来源
- 如何安装
- 如何运行训练
- 如何运行推理
- 主要指标
- 错误分析
- 已知限制
- 下一步计划

### 10.4 作品集最低配置

想证明你真的入门 AI，至少准备 6 个项目：

1. Python 自动化项目。
2. 数据分析报告。
3. 传统 ML 项目。
4. 深度学习项目。
5. RAG/LLM 应用。
6. 可部署的端到端 AI 服务。

想证明你接近专家水平，再加：

7. 论文复现项目。
8. 一个真实业务或开源项目贡献。
9. 一个系统性评估报告。

---

## 11. 论文阅读与研究训练

建议起点：完成阶段五以后开始  
目标：从“看热闹”变成“能判断论文价值和可复现性”。

### 11.1 论文阅读顺序

第一遍：只看标题、摘要、图表、结论。  
第二遍：看方法和实验设置。  
第三遍：看公式、消融实验、失败案例。  
第四遍：尝试复现核心实验或最小版本。

### 11.2 论文笔记模板

```markdown
# 论文标题

## 这篇论文解决什么问题

## 它的核心想法是什么

## 输入和输出是什么

## 方法的关键步骤

## 实验数据集和指标

## 比 baseline 好在哪里

## 我怀疑的地方

## 我能复现的最小版本

## 它对我的项目有什么启发
```

### 11.3 必读主题

不要一上来追最新论文。先按主题补：

- 反向传播
- CNN
- Word2Vec
- Seq2Seq + Attention
- Transformer
- BERT / GPT
- Vision Transformer
- Diffusion
- RAG
- RLHF / DPO
- Scaling laws
- Mixture of Experts
- Agent evals

### 11.4 验收标准

- 能讲清论文的假设。
- 能找出 baseline 是否公平。
- 能判断指标是否服务于真实目标。
- 能实现一个简化版。
- 能写出“这篇论文不适合我的场景”的理由。

---

## 12. 12 个月执行版

这是一个可以直接照做的压缩路线。

### 第 1 月：Python

资源：CS50P + Kaggle Python  
产出：学习记账本或文件整理工具  
验收：能独立写 200 行 Python

### 第 2 月：数据分析

资源：pandas 官方教程 + Kaggle Pandas  
产出：电商数据分析报告  
验收：能清洗数据、画图、写结论

### 第 3 月：数学基础

资源：MIT 18.06 + Khan Academy + 3Blue1Brown  
产出：线性回归从零实现、SVD 图片压缩  
验收：能解释矩阵、梯度、概率

### 第 4-5 月：传统机器学习

资源：DeepLearning.AI ML Specialization + Google MLCC + scikit-learn  
产出：房价预测、用户流失预测  
验收：能做特征工程、交叉验证、误差分析

### 第 6-8 月：深度学习

资源：PyTorch Blitz + D2L + fast.ai  
产出：图像分类、文本分类、手写小神经网络  
验收：能写训练循环，能解释 loss 曲线

### 第 9-10 月：LLM 应用

资源：Hugging Face Course + CS224N + OpenAI 文档  
产出：个人知识库 RAG、工具调用 Agent  
验收：有测试集、有引用、有拒答、有日志

### 第 11 月：MLOps

资源：Full Stack Deep Learning + Made With ML  
产出：一个可部署模型服务  
验收：有 API、Docker、测试、监控思路

### 第 12 月：作品集与面试/研究准备

产出：

- GitHub 整理 6 个项目。
- 写 2 篇技术博客。
- 复现 1 篇论文的最小版本。
- 做 1 次完整项目答辩录屏。

---

## 13. 每阶段自测题

### Python 自测

- 什么是可变对象？
- `list` 和 `dict` 的适用场景有什么不同？
- 什么时候应该写函数？
- 如何处理文件不存在？
- 如何安装第三方包？

### 数据分析自测

- 缺失值能不能直接删？为什么？
- `groupby` 的结果如何解释？
- 相关性是否意味着因果？
- 图表怎样避免误导？

### 数学自测

- 点积的几何意义是什么？
- 矩阵乘法为什么可以表示线性变换？
- 梯度指向什么方向？
- 最大似然估计在做什么？

### 机器学习自测

- 什么是过拟合？
- 为什么要分训练集、验证集、测试集？
- 什么是数据泄漏？
- Precision 和 Recall 如何取舍？
- 什么时候用树模型，什么时候用线性模型？

### 深度学习自测

- 反向传播解决什么问题？
- Batch size 变大会怎样？
- 学习率太大会发生什么？
- Dropout 为什么能缓解过拟合？
- CNN 为什么适合图像？

### LLM 自测

- Token 是什么？
- Attention 在解决什么问题？
- RAG 的检索失败会造成什么后果？
- Agent 和普通聊天机器人有什么区别？
- 如何评估一个 RAG 系统？

---

## 14. 常见误区

1. 只看视频不写代码。  
   视频只能给你熟悉感，项目才会暴露真实缺口。

2. 过早追大模型论文。  
   线性回归、树模型、过拟合、评估指标都没扎实，读大模型论文会很虚。

3. 以为调参就是机器学习。  
   真正重要的是数据、问题定义、评估、错误分析。

4. 只做 notebook，不做工程化。  
   notebook 适合探索，但作品集要能复现、能运行、能部署。

5. 不建立测试集。  
   没有测试集，就不知道模型是不是真的变好。

6. 把 AI 助手当答案机器。  
   AI 助手可以解释、出题、帮你 debug，但不能替你形成理解。

---

## 15. 如何使用 AI 助手辅助学习

好的用法：

- “请用生活例子解释梯度下降。”
- “这段报错是什么意思？请带我定位。”
- “请给我 10 道关于 pandas groupby 的练习，不要给答案。”
- “请审查我的模型评估方案有没有数据泄漏。”
- “请根据我的项目 README 模拟面试官提问。”

不好的用法：

- “直接帮我写完整作业。”
- “给我一个能跑就行的代码，不用解释。”
- “替我读论文并告诉我结论。”

学习期建议：核心代码先自己写，再让 AI 帮你 review。

---

## 16. 推荐资源总表

### 编程与数据

- [Python.org: Python For Beginners](https://www.python.org/about/gettingstarted/)
- [Harvard CS50P](https://cs50.harvard.edu/python/)
- [CS50P YouTube 播放列表](https://www.youtube.com/playlist?list=PLhQjrBD2T3817j24-GogXmWqO5Q5vYy0V)
- [Kaggle Learn Python](https://www.kaggle.com/learn/python)
- [pandas 官方教程](https://pandas.pydata.org/docs/getting_started/intro_tutorials/index.html)

### 数学

- [MIT 18.06 Linear Algebra 视频课](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/video_galleries/video-lectures/)
- [3Blue1Brown: Essence of Linear Algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr)
- [3Blue1Brown: Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)
- [Khan Academy: Statistics and Probability](https://www.khanacademy.org/math/statistics-probability)
- [StatQuest 视频索引](https://statquest.org/video_index.html)

### 机器学习

- [DeepLearning.AI Machine Learning Specialization](https://www.deeplearning.ai/specializations/machine-learning/)
- [Google Machine Learning Crash Course](https://developers.google.com/machine-learning/crash-course)
- [scikit-learn Getting Started](https://scikit-learn.org/stable/getting_started.html)
- [Kaggle Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning)
- [Stanford CS229 Summer 2019](https://cs229.stanford.edu/syllabus-summer2019.html)

### 深度学习

- [PyTorch 60 Minute Blitz](https://docs.pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html)
- [Dive into Deep Learning 中文版](https://zh.d2l.ai/)
- [DeepLearning.AI Deep Learning Specialization](https://www.deeplearning.ai/specializations/deep-learning/)
- [fast.ai Practical Deep Learning for Coders](https://course.fast.ai/)
- [fast.ai YouTube 播放列表](https://www.youtube.com/playlist?list=PLfYUBJiXbdtSvpQjSnJJ_PmDQB_VyT5iU)
- [Karpathy Neural Networks Zero to Hero](https://github.com/karpathy/nn-zero-to-hero)
- [李宏毅 2023 春机器学习课程 B 站授权版](https://www.bilibili.com/video/BV1TD4y137mP/)

### LLM 与 Agent

- [Hugging Face LLM/NLP Course](https://huggingface.co/course)
- [Hugging Face Agents Course](https://huggingface.co/learn/agents-course)
- [Stanford CS224N](https://web.stanford.edu/class/cs224n/)
- [Stanford CS25: Transformers United](https://web.stanford.edu/class/cs25/)
- [Stanford CS336: Language Modeling from Scratch](https://cs336.stanford.edu/)
- [OpenAI API Quickstart](https://platform.openai.com/docs/quickstart)
- [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)
- [OpenAI Agents Guide](https://platform.openai.com/docs/guides/agents)
- [OpenAI Cookbook: evaluation flywheel](https://cookbook.openai.com/examples/evaluation/building_resilient_prompts_using_an_evaluation_flywheel)

### 生产化、MLOps 与治理

- [Full Stack Deep Learning 2022](https://fullstackdeeplearning.com/course/2022/)
- [Made With ML: MLOps Course](https://madewithml.com/courses/mlops/)
- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework)
- [Stanford HAI 2026 AI Index Report](https://hai.stanford.edu/ai-index/2026-ai-index-report)

---

## 17. 你今天就可以开始的第一步

今天只做 3 件事：

1. 打开 [CS50P](https://cs50.harvard.edu/python/)，看 Week 0。
2. 新建一个文件夹 `ai-learning`，里面建 `week01.md`。
3. 写并运行第一个 Python 文件：

```python
name = input("你的名字是：")
print(f"{name}，欢迎开始人工智能学习之路。")
```

明天开始做 CS50P 的第一个 problem set。  
不要等“准备好了”再开始。准备是在做的过程中完成的。

