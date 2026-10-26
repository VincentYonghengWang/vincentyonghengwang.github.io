企业 RSI 需要一个“不会很快耗尽”的优化空间，这种空间可能来自科学探索，也可能来自博弈(safety、trading)。很多人认为 RSI 应该涉及 Pretrain。有人认为 Harness 层也可能实现 RSI，只要其改进能够反过来增强下一轮的改进能力。谈论企业 RSI 之前，先讨论一下企业任务。**我把任务大致先分为2类，或者说一个 Spectrum 的两个端点。**

## 第 1 类：Mapped-Space Tasks

主要包括以下 5 类：

1. Customer Support
2. Legal & Compliance
3. HR & Recruiting
4. Business Operations
5. Financial Operations

这些任务具有2个共同特点：优化上限相对明确，变化主要来自一些局部的更新，比如发布新产品、法律发生变化、招聘流程调整，很多场景不需要 RSI，只需要 FDE 把 Workflow 写好。

2. 如果要做 Self-Improvement，要先搭建一个 Representative Benchmark，让它能够很好地 Represent 真实任务，包括：任务出现的频率、不同任务类型和难度、Failure Modes、Environment Coverage，包括 Permissions、Tool Availability、Context Limitations 和 Verification。

然后，Self-Evolving Harness 可以自己向着目标不断改进和提高。

## 第 2 类：Open Ended Problems

这类任务需要定义目标，提供工具、环境、Constraints、Eval Criteria、Search Space： What can the system change or discover? 比如提高训练效率时，需要明确 Search Space：是否可以修改 Learning Rate、Optimizer、Model Architecture、CUDA Kernel、Training Pipeline 等？

### 例子 1：提高模型训练效率

**Goal:** Reduce training cost while maintaining model quality.

**Tools:** Python, PyTorch, CUDA, profiling tools.

**Environment:** Training infrastructure and GPU clusters.

**Constraints:** GPU budget, memory, runtime.

**Evaluation:** Validation loss, throughput, training cost, reproducibility.

**Search Space:** Optimizers, model architectures, kernels, training algorithms.

### 例子 2：Scientific Discovery RSI

**Goal:** Identify and validate disease-relevant therapeutic targets.

**工具：** 生物信息学、文献检索、分子建模。

**Environment:** Public databases, computational and laboratory experiments.

**Constraints:** Biological plausibility, safety, experimental cost.

**Evaluation:** Experimental validation, reproducibility, causal evidence.

**Search Space:** Genes, proteins, pathways, mechanisms.

这个领域的特点是：Evaluation is expensive and time-consuming.

### 例子 3：GTM RSI

**Goal:** Maximize incremental downloads and revenue.

**Tools:** Social media, advertising platforms, analytics.

**Environment:** Real-world market.

**Constraints:** Budget, brand, platform policies.

**Evaluation:** Incremental conversion, CAC, retention, LTV.

**Search Space:** Content, channels, audiences, pricing, campaigns.

## 两种持续扩展 Frontier 的机制

真正有长期价值的 RSI，需要持续扩展的优化空间。

这种空间可能来自科学探索，也可能来自竞争性博弈。

### 机制一：Exploration-driven Frontier

通过探索不断发现新的可能性。

**1. Life Science**

人类可以持续探索新的疾病机制、药物靶点、治疗方案和生物学机制。

**2. Entertainment**

人类对娱乐体验的需求不断变化。

即使已经有大量游戏，仍然可能出现新的玩法、交互方式和娱乐形式。

### 机制二：Competition-driven Frontier

通过竞争不断提高能力要求。

**1. Finance**

一个交易策略今天有效，明天可能因为竞争对手采用类似策略而失效。

**2. Cybersecurity**

攻击者能力提高，防御系统就需要继续提高。

**3. GTM**

一个广告创意今天有效，但当竞争对手采用更有效的内容、平台算法改变、消费者兴趣变化时，原来的策略可能失效。

不同领域的信息衰减速度不同。

| 领域 | Information Decay | 持续优化的需求 |
| --- | --- | --- |
| Entertainment | 用户偏好不断变化 | 需要持续探索新体验 |
| Finance | 市场信息衰减很快 | 需要持续发现新策略 |
| Cybersecurity | 攻防能力持续变化 | 需要不断适应对手 |
| GTM | 广告效果、用户偏好、平台算法变化 | 需要持续优化投放策略 |

金融市场不仅具有竞争性，而且信息衰减速度快，因此特别适合自动研究和持续优化。

## 值得探索 RSI 的 5 个方向

1. Life Science
2. Entertainment
3. Finance
4. Cybersecurity
5. GTM

这些领域具有持续扩展的优化空间，主要来自两种机制：

- **Exploration-driven Frontier：** 通过探索不断发现新的可能性。
- **Competition-driven Frontier：** 通过竞争不断提高能力要求。

## 五、Robotics：RSI 进入传统物理产业的重要桥梁

为什么 RSI 的潜在方向似乎集中在少数数字化领域？传统制造业、农业、建筑业等行业似乎没有被充分覆盖。一个重要原因是，目前 AI 主要能够直接操作数字环境，而不能直接完成大量物理任务。Robotics 是 RSI 进入传统物理产业的重要桥梁。当前很多传统行业无法仅靠软件 Agent 完成完整的优化闭环。Robotics 可以让 RSI 从 Digital Space 进一步扩展到 Physical Space。

## 六、RSI 需要第三个条件：Economic Sustainability

持续提高能力是否能够创造足够的经济价值，从而支持下一轮优化？

即使技术上能够持续优化，如果优化成果不能创造足够的商业价值，也很难支持长期的算力投入。

因此，RSI 不仅需要持续扩展的优化空间和 Recursive Improvement，还需要考虑 Economic Sustainability。

**核心问题：持续提高能力是否能够创造足够的经济价值，从而支持下一轮优化？**

例如，Anthropic 的[“设计能够结合蝎子神经毒素的蛋白质”研究](https://www.anthropic.com/research/claude-scorpion-toxin-binder-design)，在我看来，应该不是一个能提供很多经济价值的研究。

**Note:** 这个 note 不追求每个观点都正确，只是先记录一下。
