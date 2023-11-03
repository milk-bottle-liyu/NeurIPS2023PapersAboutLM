# Papers about Language Modeling in NeurIPS 2023
## Token-Scaled Logit Distillation for Ternary Weight Generative Language Models<sup>poster<sup>

Authors: Minsoo Kim, Sihwa Lee, Janghwan Lee, Sukjin Hong, Du-Seong Chang, Wonyong Sung, Jungwook Choi

Link: [https://neurips.cc/virtual/2023/poster/72260](https://neurips.cc/virtual/2023/poster/72260)

Abstract:

 Generative Language Models (GLMs) have shown impressive performance in tasks such as text generation, understanding, and reasoning. However, the large model size poses challenges for practical deployment. To solve this problem, Quantization-Aware Training (QAT) has become increasingly popular. However, current QAT methods for generative models have resulted in a noticeable loss of accuracy. To counteract this issue, we propose a novel knowledge distillation method specifically designed for GLMs. Our method, called token-scaled logit distillation, prevents overfitting and provides superior learning from the teacher model and ground truth. This research marks the first evaluation of ternary weight quantization-aware training of large-scale GLMs with less than 1.0 degradation in perplexity and achieves enhanced accuracy in tasks like common-sense QA and arithmetic reasoning  as well as natural language understanding. Our code is available at https://github.com/aiha-lab/TSLD.

摘要:

生成语言模型（GLM）在文本生成、理解和推理等任务中表现出了令人印象深刻的性能。然而，较大的模型尺寸给实际部署带来了挑战。为了解决这个问题，量化感知训练（QAT）变得越来越流行。然而，当前生成模型的 QAT 方法导致了准确性的明显损失。为了解决这个问题，我们提出了一种专门为 GLM 设计的新颖的知识蒸馏方法。我们的方法称为令牌规模 Logit 蒸馏，可以防止过度拟合，并提供从教师模型和基本事实中进行的卓越学习。这项研究标志着首次对大规模 GLM 的三元权重量化感知训练进行了评估，其困惑度下降小于 1.0，并在常识 QA、算术推理以及自然语言理解等任务中实现了更高的准确性。我们的代码可在 https://github.com/aiha-lab/TSLD 获取。

## Interactive Multi-fidelity Learning for Cost-effective Adaptation of Language Model with Sparse Human Supervision<sup>poster<sup>

Authors: Jiaxin Zhang, Zhuohang Li, Kamalika Das, Sricharan Kumar

Link: [https://neurips.cc/virtual/2023/poster/71465](https://neurips.cc/virtual/2023/poster/71465)

Abstract:

 Large language models (LLMs) have demonstrated remarkable capabilities in various tasks. However, their suitability for domain-specific tasks, is limited due to their immense scale at deployment, susceptibility to misinformation, and more importantly, high data annotation costs. We propose a novel Interactive Multi-Fidelity Learning (IMFL) framework for cost-effective development of small domain-specific LMs under limited annotation budgets. Our approach formulates the domain-specific fine-tuning process as a multi-fidelity learning problem, focusing on identifying the optimal acquisition strategy that balances between low-fidelity automatic LLM annotations and high-fidelity human annotations to maximize model performance. We further propose an exploration-exploitation query strategy that enhances annotation diversity and informativeness, incorporating two innovative designs: 1) prompt retrieval that selects in-context examples from human-annotated samples to improve LLM annotation, and 2) variable batch size that controls the order for choosing each fidelity to facilitate knowledge distillation, ultimately enhancing annotation quality. Extensive experiments on financial and medical tasks demonstrate that IMFL achieves superior performance compared with single fidelity annotations. Given a limited budget of human annotation, IMFL significantly outperforms the $\bf 3\times$ human annotation baselines in all four tasks and achieves very close performance as $\bf 5\times$ human annotation on two of the tasks. These promising results suggest that the high human annotation costs in domain-specific tasks can be significantly reduced by employing IMFL, which utilizes fewer human annotations, supplemented with cheaper and faster LLM (e.g., GPT-3.5) annotations to achieve comparable performance.

摘要:

大型语言模型（LLM）在各种任务中表现出了卓越的能力。然而，由于其部署规模巨大、容易受到错误信息的影响，更重要的是，数据注释成本高昂，它们对特定领域任务的适用性受到限制。我们提出了一种新颖的交互式多保真学习（IMFL）框架，用于在有限的注释预算下经济有效地开发小型特定领域的 LM。我们的方法将特定领域的微调过程制定为多保真度学习问题，重点是确定在低保真度自动 LLM 注释和高保真度人工注释之间取得平衡的最佳获取策略，以最大限度地提高模型性能。我们进一步提出了一种增强注释多样性和信息量的探索-利用查询策略，结合了两种创新设计：1）提示检索，从人工注释的样本中选择上下文中的示例以改进LLM注释，2）可变批量大小控制选择每个保真度的顺序以促进知识蒸馏，最终提高注释质量。针对金融和医疗任务的大量实验表明，与单一保真度注释相比，IMFL 具有卓越的性能。鉴于人工注释的预算有限，IMFL 在所有四项任务中都显着优于 $\bf 3\times$ 人工注释基线，并且在其中两项任务上实现了与 $\bf 5\times$ 人工注释非常接近的性能。这些有希望的结果表明，通过采用 IMFL 可以显着降低特定领域任务中的高人工注释成本，IMFL 使用较少的人工注释，并辅以更便宜和更快的 LLM（例如 GPT-3.5）注释来实现可比较的性能。

## LayoutGPT: Compositional Visual Planning and Generation with Large Language Models<sup>poster<sup>

Authors: Weixi Feng, Wanrong Zhu, Tsu-Jui Fu, Varun Jampani, Arjun Akula, Xuehai He, S Basu, Xin Eric Wang, William Yang Wang

Link: [https://neurips.cc/virtual/2023/poster/71328](https://neurips.cc/virtual/2023/poster/71328)

Abstract:

 Attaining a high degree of user controllability in visual generation often requires intricate, fine-grained inputs like layouts. However, such inputs impose a substantial burden on users when compared to simple text inputs. To address the issue, we study how Large Language Models (LLMs) can serve as visual planners by generating layouts from text conditions, and thus collaborate with visual generative models. We propose LayoutGPT, a method to compose in-context visual demonstrations in style sheet language to enhance visual planning skills of LLMs. We show that LayoutGPT can generate plausible layouts in multiple domains, ranging from 2D images to 3D indoor scenes. LayoutGPT also shows superior performance in converting challenging language concepts like numerical and spatial relations to layout arrangements for faithful text-to-image generation. When combined with a downstream image generation model, LayoutGPT outperforms text-to-image models/systems by 20-40\% and achieves comparable performance as human users in designing visual layouts for numerical and spatial correctness. Lastly, LayoutGPT achieves comparable performance to supervised methods in 3D indoor scene synthesis, demonstrating its effectiveness and potential in multiple visual domains.

摘要:

在视觉生成中获得高度的用户可控性通常需要复杂、细粒度的输入，例如布局。然而，与简单的文本输入相比，这样的输入给用户带来了很大的负担。为了解决这个问题，我们研究了大型语言模型（LLM）如何通过根据文本条件生成布局来充当视觉规划器，从而与视觉生成模型协作。我们提出了 LayoutGPT，一种用样式表语言编写上下文视觉演示的方法，以增强法学硕士的视觉规划技能。我们证明 LayoutGPT 可以在多个领域生成合理的布局，范围从 2D 图像到 3D 室内场景。 LayoutGPT 在将数字和空间关系等具有挑战性的语言概念转换为布局安排以实现忠实的文本到图像生成方面也表现出了卓越的性能。当与下游图像生成模型结合使用时，LayoutGPT 的性能比文本到图像模型/系统高出 20-40%，并且在设计视觉布局的数值和空间正确性方面实现了与人类用户相当的性能。最后，LayoutGPT 在 3D 室内场景合成中实现了与监督方法相当的性能，展示了其在多个视觉领域的有效性和潜力。

## Parts of Speech–Grounded Subspaces in Vision-Language Models<sup>poster<sup>

Authors: James Oldfield, Christos Tzelepis, Yannis Panagakis, Mihalis Nicolaou, Ioannis Patras

Link: [https://neurips.cc/virtual/2023/poster/70789](https://neurips.cc/virtual/2023/poster/70789)

Abstract:

 Latent image representations arising from vision-language models have proved immensely useful for a variety of downstream tasks. However, their utility is limited by their entanglement with respect to different visual attributes. For instance, recent work has shown that CLIP image representations are often biased toward specific visual properties (such as objects or actions) in an unpredictable manner. In this paper, we propose to separate representations of the different visual modalities in CLIP’s joint vision-language space by leveraging the association between parts of speech and specific visual modes of variation (e.g. nouns relate to objects, adjectives describe appearance). This is achieved by formulating an appropriate component analysis model that learns subspaces capturing variability corresponding to a specific part of speech, while jointly minimising variability to the rest. Such a subspace yields disentangled representations of the different visual properties of an image or text in closed form while respecting the underlying geometry of the manifold on which the representations lie. What’s more, we show the proposed model additionally facilitates learning subspaces corresponding to specific visual appearances (e.g. artists’ painting styles), which enables the selective removal of entire visual themes from CLIP-based text-to-image synthesis. We validate the model both qualitatively, by visualising the subspace projections with a text-to-image model and by preventing the imitation of artists’ styles, and quantitatively, through class invariance metrics and improvements to baseline zero-shot classification.

摘要:

事实证明，视觉语言模型产生的潜在图像表示对于各种下游任务非常有用。然而，它们的实用性因其与不同视觉属性的纠缠而受到限制。例如，最近的工作表明 CLIP 图像表示通常以不可预测的方式偏向于特定的视觉属性（例如对象或动作）。在本文中，我们建议通过利用词性和特定视觉变化模式之间的关联（例如，名词与物体相关，形容词描述外观），来分离CLIP联合视觉语言空间中不同视觉模态的表示。这是通过制定适当的成分分析模型来实现的，该模型学习捕获与特定词性相对应的变异性的子空间，同时共同最小化其余部分的变异性。这样的子空间以封闭形式产生图像或文本的不同视觉属性的解开表示，同时尊重表示所在的流形的基础几何形状。更重要的是，我们表明所提出的模型还有助于学习与特定视觉外观（例如艺术家的绘画风格）相对应的子空间，这使得能够从基于 CLIP 的文本到图像合成中选择性地删除整个视觉主题。我们通过使用文本到图像模型可视化子空间投影并防止模仿艺术家风格来定性地验证模型，并通过类不变性指标和对基线零样本分类的改进来定量地验证模型。

## Augmenting Language Models with Long-Term Memory<sup>poster<sup>

Authors: Weizhi Wang, Li Dong, Hao Cheng, Xiaodong Liu, Xifeng Yan, Jianfeng Gao, Furu Wei

Link: [https://neurips.cc/virtual/2023/poster/72461](https://neurips.cc/virtual/2023/poster/72461)

Abstract:

 Existing large language models (LLMs) can only afford fix-sized inputs due to the input length limit, preventing them from utilizing rich long-context information from past inputs. To address this, we propose a framework, Language Models Augmented with Long-Term Memory (LongMem), which enables LLMs to memorize long history. We design a novel decoupled network architecture with the original backbone LLM frozen as a memory encoder and an adaptive residual side-network as a memory retriever and reader. Such a decoupled memory design can easily cache and update long-term past contexts for memory retrieval without suffering from memory staleness. Enhanced with memory-augmented adaptation training, LongMem can thus memorize long past context and use long-term memory for language modeling. The proposed memory retrieval module can handle unlimited-length context in its memory bank to benefit various downstream tasks. Typically, LongMem can enlarge the long-form memory to 65k tokens and thus cache many-shot extra demonstration examples as long-form memory for in-context learning. Experiments show that our method outperforms strong long-context models on ChapterBreak, a challenging long-context modeling benchmark, and achieves remarkable improvements on memory-augmented in-context learning over LLMs. The results demonstrate that the proposed method is effective in helping language models to memorize and utilize long-form contents.

摘要:

由于输入长度限制，现有的大型语言模型（LLM）只能提供固定大小的输入，从而阻止它们利用过去输入中丰富的长上下文信息。为了解决这个问题，我们提出了一个框架，即增强长期记忆的语言模型（LongMem），它使法学硕士能够记住悠久的历史。我们设计了一种新颖的解耦网络架构，将原始骨干LLM冻结为内存编码器，将自适应残差侧网络作为内存检索器和读取器。这种解耦的内存设计可以轻松缓存和更新长期过去的上下文以进行内存检索，而不会遭受内存陈旧的影响。通过记忆增强适应训练的增强，LongMem 可以记住很久以前的上下文，并使用长期记忆进行语言建模。所提出的内存检索模块可以处理其内存库中无限长度的上下文，以有利于各种下游任务。通常，LongMem 可以将长格式内存扩大到 65k 个标记，从而将多镜头额外演示示例缓存为长格式内存，用于上下文学习。实验表明，我们的方法在 ChapterBreak（一个具有挑战性的长上下文建模基准）上优于强大的长上下文模型，并且在记忆增强上下文学习方面比法学硕士取得了显着的改进。结果表明，该方法可以有效帮助语言模型记忆和利用长格式内容。

## Statistical Knowledge Assessment for Large Language Models<sup>poster<sup>

Authors: Qingxiu Dong, Jingjing Xu, Lingpeng Kong, Zhifang Sui, Lei Li

Link: [https://neurips.cc/virtual/2023/poster/70415](https://neurips.cc/virtual/2023/poster/70415)

Abstract:

 Given varying prompts regarding a factoid question, can a large language model (LLM) reliably generate factually correct answers? Existing LLMs may generate distinct responses for different prompts. In this paper, we study the problem of quantifying knowledge contained in an LLM regarding a given set of facts. We propose KaRR, a statistical approach to assess factual knowledge for LLMs. The main idea is to estimate the ratio of LLM generating text corresponding to the answer entity given diverse prompts of the subject and the querying relation, versus it generating by random chances. Our assessment suite contains a comprehensive set of 994,123 entities and 600 relations, with 1,395,905 text aliases. We use our method to evaluate 20 LLMs of various sizes, including LLaMA, Alpaca, OPT, etc. Experiments show that our results have a strong correlation (0.43 Kendall's $\tau$) with the results of human assessment on LLMs. Our results reveal that the knowledge in LLMs with the same backbone architecture adheres to the scaling law, while tuning on instruction-following data sometimes compromises the model's capability to generate factually correct text reliably.

摘要:

给定有关事实问题的不同提示，大型语言模型 (LLM) 能否可靠地生成事实上正确的答案？现有的法学硕士可能会对不同的提示产生不同的反应。在本文中，我们研究了量化法学硕士中包含的有关给定事实集的知识的问题。我们提出 KaRR，一种评估法学硕士事实知识的统计方法。主要思想是估计LLM在给定主题和查询关系的不同提示的情况下生成与答案实体相对应的文本与随机生成的文本的比率。我们的评估套件包含一整套 994,123 个实体和 600 个关系，以及 1,395,905 个文本别名。我们使用我们的方法评估了 20 个不同规模的 LLM，包括 LLaMA、Alpaca、OPT 等。实验表明，我们的结果与人类对 LLM 的评估结果具有很强的相关性（0.43 Kendall's $\tau$）。我们的结果表明，具有相同主干架构的法学硕士中的知识遵循缩放法则，而对指令跟踪数据的调整有时会损害模型可靠地生成事实上正确的文本的能力。

## Meta-in-context learning in large language models<sup>poster<sup>

Authors: Julian Coda-Forno, Marcel Binz, Zeynep Akata, Matt Botvinick, Jane Wang, Eric Schulz

Link: [https://neurips.cc/virtual/2023/poster/70239](https://neurips.cc/virtual/2023/poster/70239)

Abstract:

 Large language models have shown tremendous performance in a variety of tasks.  In-context learning  -- the ability to improve at a task after being provided with a number of demonstrations -- is seen as one of the main contributors to their success. In the present paper, we demonstrate that the in-context learning abilities of large language models can be recursively improved via in-context learning itself. We coin this phenomenon meta-in-context learning. Looking at two idealized domains, a one-dimensional regression task and a two-armed bandit task, we show that meta-in-context learning adaptively reshapes a large language model's priors over expected tasks. Furthermore, we find that meta-in-context learning modifies the in-context learning strategies of such models. Finally, we broaden the scope of our investigation to encompass two diverse benchmarks: one focusing on real-world regression problems and the other encompassing multiple NLP tasks. In both cases, we observe competitive performance comparable to that of traditional learning algorithms. Taken together, our work improves our understanding of in-context learning and paves the way toward adapting large language models to the environment they are applied purely through meta-in-context learning rather than traditional finetuning.

摘要:

大型语言模型在各种任务中表现出了巨大的性能。情境学习——在提供多次演示后改进任务的能力——被视为他们成功的主要因素之一。在本文中，我们证明了大型语言模型的上下文学习能力可以通过上下文学习本身来递归地提高。我们将这种现象称为元情境学习。着眼于两个理想化的领域，一个一维回归任务和一个双臂老虎机任务，我们表明元上下文学习自适应地重塑了大型语言模型相对于预期任务的先验。此外，我们发现元上下文学习修改了此类模型的上下文学习策略。最后，我们扩大了调查范围，涵盖两个不同的基准：一个专注于现实世界的回归问题，另一个涵盖多个 NLP 任务。在这两种情况下，我们都观察到与传统学习算法相当的竞争性能。总而言之，我们的工作提高了我们对上下文学习的理解，并为纯粹通过元上下文学习而不是传统的微调使大型语言模型适应它们所应用的环境铺平了道路。

## Language Models can Solve Computer Tasks<sup>poster<sup>

Authors: Geunwoo Kim, Pierre Baldi, Stephen McAleer

Link: [https://neurips.cc/virtual/2023/poster/71929](https://neurips.cc/virtual/2023/poster/71929)

Abstract:

 Agents capable of carrying out general tasks on a computer can improve efficiency and productivity by automating repetitive tasks and assisting in complex problem-solving. Ideally, such agents should be able to solve new computer tasks presented to them through natural language commands. However, previous approaches to this problem require large amounts of expert demonstrations and task-specific reward functions, both of which are impractical for new tasks. In this work, we show that a pre-trained large language model (LLM) agent can execute computer tasks guided by natural language using a simple prompting scheme where the agent \textbf{R}ecursively \textbf{C}riticizes and \textbf{I}mproves its output (RCI). The RCI approach significantly outperforms existing LLM methods for automating computer tasks and surpasses supervised learning (SL) and reinforcement learning (RL) approaches on the MiniWoB++ benchmark. We compare multiple LLMs and find that RCI with the InstructGPT-3+RLHF LLM is state-of-the-art on MiniWoB++, using only a handful of demonstrations per task rather than tens of thousands, and without a task-specific reward function. Furthermore, we demonstrate RCI prompting's effectiveness in enhancing LLMs' reasoning abilities on a suite of natural language reasoning tasks, outperforming chain of thought (CoT) prompting with external feedback. We find that RCI combined with CoT performs better than either separately. Our code can be found here: https://github.com/posgnu/rci-agent.

摘要:

能够在计算机上执行一般任务的代理可以通过自动执行重复任务并协助解决复杂问题来提高效率和生产力。理想情况下，此类代理应该能够解决通过自然语言命令呈现给他们的新计算机任务。然而，以前解决这个问题的方法需要大量的专家演示和特定于任务的奖励函数，这对于新任务来说都是不切实际的。在这项工作中，我们展示了预训练的大语言模型（LLM）代理可以使用简单的提示方案执行由自然语言引导的计算机任务，其中代理 \textbf{R} 递归地 \textbf{C} 批评和 \textbf{ I}提高了其输出（RCI）。 RCI 方法在自动化计算机任务方面显着优于现有的 LLM 方法，并且在 MiniWoB++ 基准上超越了监督学习 (SL) 和强化学习 (RL) 方法。我们比较了多个 LLM，发现使用 InstructGPT-3+RLHF LLM 的 RCI 在 MiniWoB++ 上是最先进的，每个任务仅使用少量演示，而不是数万次，并且没有特定于任务的奖励函数。此外，我们还证明了 RCI 提示在增强法学硕士在一系列自然语言推理任务中的推理能力方面的有效性，其表现优于带有外部反馈的思想链 (CoT) 提示。我们发现 RCI 与 CoT 结合使用比单独使用两者效果更好。我们的代码可以在这里找到：https://github.com/posgnu/rci-agent。

## VisIT-Bench: A Dynamic Benchmark for Evaluating Instruction-Following Vision-and-Language Models<sup>poster<sup>

Authors: Yonatan Bitton, Hritik Bansal, Jack Hessel, Rulin Shao, Wanrong Zhu, Anas Awadalla, Josh Gardner, Rohan Taori, Ludwig Schmidt

Link: [https://neurips.cc/virtual/2023/poster/73556](https://neurips.cc/virtual/2023/poster/73556)

Abstract:

 We introduce VisIT-Bench (Visual InsTruction Benchmark), a benchmark for evaluating instruction-following vision-language models for real-world use. Our starting point is curating 70 "instruction families" that we envision instruction tuned vision-language models should be able to address. Extending beyond evaluations like VQAv2 and COCO, tasks range from basic recognition to game playing and creative generation. Following curation, our dataset comprises 592 test queries, each with a human-authored instruction-conditioned caption. These descriptions surface instruction-specific factors, e.g., for an instruction asking about the accessibility of a storefront for wheelchair users, the instruction-conditioned caption describes ramps/potential obstacles. These descriptions enable 1) collecting human-verified reference outputs for each instance; and 2) automatic evaluation of candidate multimodal generations using a text-only LLM, aligning with human judgment. We quantify quality gaps between models and references using both human and automatic evaluations; e.g., the top-performing instruction-following model wins against the GPT-4 reference in just 27% of the comparison. VisIT-Bench is dynamic to participate, practitioners simply submit their model's response on the project website; Data, code and leaderboard is available at https://visit-bench.github.io/.

摘要:

我们介绍 VisIT-Bench（视觉指令基准），这是一个用于评估实际使用的指令跟踪视觉语言模型的基准。我们的出发点是策划 70 个“指令族”，我们设想指令调整的视觉语言模型应该能够解决这些问题。除了 VQAv2 和 COCO 等评估之外，任务范围还包括从基本识别到游戏和创意生成。经过整理后，我们的数据集包含 592 个测试查询，每个查询都有一个人工编写的指令条件标题。这些描述表面了特定于指令的因素，例如，对于询问轮椅使用者店面的可访问性的指令，以指令为条件的标题描述了坡道/潜在的障碍物。这些描述使得 1) 收集每个实例的经人工验证的参考输出； 2）使用纯文本法学硕士自动评估候选多模式生成，与人类判断保持一致。我们使用人工和自动评估来量化模型和参考之间的质量差距；例如，性能最佳的指令跟踪模型仅在 27% 的比较中胜过 GPT-4 参考模型。 VisIT-Bench是动态参与的，从业者只需在项目网站上提交他们的模型响应即可；数据、代码和排行榜可在 https://visit-bench.github.io/ 获取。

## Test-Time Distribution Normalization for Contrastively Learned Visual-language Models<sup>poster<sup>

Authors: Yifei Zhou, Juntao Ren, Fengyu Li, Ramin Zabih, Ser Nam Lim

Link: [https://neurips.cc/virtual/2023/poster/71464](https://neurips.cc/virtual/2023/poster/71464)

Abstract:

 Advances in the field of visual-language contrastive learning have made it possible for many downstream applications to be carried out efficiently and accurately by simply taking the dot product between image and text representations.  One of the most representative approaches proposed recently known as CLIP has quickly garnered widespread adoption due to its effectiveness. CLIP is trained with an InfoNCE loss that takes into account both positive and negative samples to help learn a much more robust representation space. This paper however reveals that the common downstream practice of taking a dot product is only a zeroth-order approximation of the optimization goal, resulting in a loss of information during test-time. Intuitively, since the model has been optimized based on the InfoNCE loss, test-time procedures should ideally also be in alignment. The question lies in how one can retrieve any semblance of negative samples information during inference in a computationally efficient way. We propose Distribution Normalization (DN), where we approximate the mean representation of a batch of test samples and use such a mean to represent what would be analogous to negative samples in the InfoNCE loss. DN requires no retraining or fine-tuning and can be effortlessly applied during inference. Extensive experiments on a wide variety of downstream tasks exhibit a clear advantage of DN over the dot product on top of other existing test-time augmentation methods.

摘要:

视觉语言对比学习领域的进步使得许多下游应用程序可以通过简单地获取图像和文本表示之间的点积来高效、准确地进行。最近提出的最具代表性的方法之一称为 CLIP，由于其有效性而迅速获得了广泛采用。 CLIP 使用 InfoNCE 损失进行训练，该损失同时考虑正样本和负样本，以帮助学习更稳健的表示空间。然而，本文揭示了采用点积的常见下游实践只是优化目标的零阶近似，导致测试期间信息丢失。直观上，由于模型是根据 InfoNCE 损失进行优化的，因此理想情况下测试时间程序也应该保持一致。问题在于如何在推理过程中以一种计算有效的方式检索任何类似的负样本信息。我们提出分布归一化（DN），我们近似一批测试样本的均值表示，并使用这样的均值来表示与 InfoNCE 损失中的负样本类似的内容。 DN 不需要重新训练或微调，并且可以在推理过程中轻松应用。对各种下游任务的大量实验表明，在其他现有的测试时间增强方法之上，DN 相对于点积具有明显的优势。

## CLadder: A Benchmark to Assess Causal Reasoning Capabilities of Language Models<sup>poster<sup>

Authors: Zhijing Jin, Yuen Chen, Felix Leeb, Luigi Gresele, Ojasv Kamal, Zhiheng LYU, Kevin Blin, Fernando Gonzalez Adauto, Max Kleiman-Weiner, Mrinmaya Sachan, Bernhard Schölkopf

Link: [https://neurips.cc/virtual/2023/poster/70983](https://neurips.cc/virtual/2023/poster/70983)

Abstract:

 The ability to perform causal reasoning is widely considered a core feature of intelligence. In this work, we investigate whether large language models (LLMs) can coherently reason about causality. Much of the existing work in natural language processing (NLP) focuses on evaluating commonsense causal reasoning in LLMs, thus failing to assess whether a model can perform causal inference in accordance with a set of well-defined formal rules. To address this, we propose a new NLP task, causal inference in natural language, inspired by the “causal inference engine” postulated by Judea Pearl et al. We compose a large dataset, CLadder, with 10K samples: based on a collection of causal graphs and queries (associational, interventional, and counterfactual), we obtain symbolic questions and ground-truth answers, through an oracle causal inference engine. These are then translated into natural language. We evaluate multiple LLMs on our dataset, and we introduce and evaluate a bespoke chain-of-thought prompting strategy, CausalCoT. We show that our task is highly challenging for LLMs, and we conduct an in-depth analysis to gain deeper insight into the causal reasoning abilities of LLMs

摘要:

执行因果推理的能力被广泛认为是智力的核心特征。在这项工作中，我们研究大型语言模型 (LLM) 是否能够连贯地推理因果关系。自然语言处理（NLP）领域的大部分现有工作都侧重于评估法学硕士中的常识因果推理，因此无法评估模型是否可以根据一组明确定义的形式规则执行因果推理。为了解决这个问题，我们提出了一个新的 NLP 任务，即自然语言中的因果推理，受到 Judea Pearl 等人提出的“因果推理引擎”的启发。我们构建了一个包含 10K 样本的大型数据集 CLadder：基于因果图和查询（关联、干预和反事实）的集合，我们通过预言机因果推理引擎获得符号问题和真实答案。然后将它们翻译成自然语言。我们在数据集上评估了多个法学硕士，并引入并评估了定制的思维链提示策略 CausalCoT。我们表明，我们的任务对于法学硕士来说非常具有挑战性，我们进行了深入的分析，以更深入地了解法学硕士的因果推理能力

## DoReMi: Optimizing Data Mixtures Speeds Up Language Model Pretraining<sup>poster<sup>

Authors: Sang Michael Xie, Hieu Pham, Xuanyi Dong, Nan Du, Hanxiao Liu, Yifeng Lu, Percy Liang, Quoc V Le, Tengyu Ma, Adams Wei Yu

Link: [https://neurips.cc/virtual/2023/poster/70588](https://neurips.cc/virtual/2023/poster/70588)

Abstract:

 The mixture proportions of pretraining data domains (e.g., Wikipedia, books, web text) greatly affect language model (LM) performance. In this paper, we propose Domain Reweighting with Minimax Optimization (DoReMi), which first trains a small proxy model using group distributionally robust optimization (Group DRO) over domains to produce domain weights (mixture proportions) without knowledge of downstream tasks. We then resample a dataset with these domain weights and train a larger, full-sized model. In our experiments, we use DoReMi on a 280M-parameter proxy model to find domain weights for training an 8B-parameter model (30x larger) more efficiently. On The Pile, DoReMi improves perplexity across all domains, even when it downweights a domain. DoReMi improves average few-shot downstream accuracy by 6.5% points over a baseline model trained using The Pile's default domain weights and reaches the baseline accuracy with 2.6x fewer training steps. On the GLaM dataset, DoReMi, which has no knowledge of downstream tasks, even matches the performance of using domain weights tuned on downstream tasks.

摘要:

预训练数据域（例如维基百科、书籍、网络文本）的混合比例极大地影响语言模型（LM）的性能。在本文中，我们提出了采用最小最大优化的域重新加权（DoReMi），它首先使用域上的组分布鲁棒优化（Group DRO）来训练一个小型代理模型，以在不了解下游任务的情况下产生域权重（混合比例）。然后，我们使用这些域权重对数据集进行重新采样，并训练一个更大的全尺寸模型。在我们的实验中，我们在 280M 参数代理模型上使用 DoReMi 来查找域权重，以更有效地训练 8B 参数模型（大 30 倍）。在 The Pile 上，DoReMi 改善了所有领域的复杂性，即使它降低了某个领域的权重。与使用 The Pile 默认域权重训练的基线模型相比，DoReMi 将平均少样本下游准确度提高了 6.5%，并以减少 2.6 倍的训练步骤达到基线准确度。在 GLaM 数据集上，不了解下游任务的 DoReMi 甚至可以与使用针对下游任务调整的域权重的性能相匹配。

## Counterfactual Memorization in Neural Language Models<sup>poster<sup>

Authors: Chiyuan Zhang, Daphne Ippolito, Katherine Lee, Matthew Jagielski, Florian Tramer, Nicholas Carlini

Link: [https://neurips.cc/virtual/2023/poster/72772](https://neurips.cc/virtual/2023/poster/72772)

Abstract:

 Modern neural language models that are widely used in various NLP tasks risk memorizing sensitive information from their training data.Understanding this memorization is important in real world applications and also from a learning-theoretical perspective. An open question in previous studies of language model memorization is how to filter out ``common'' memorization. In fact, most memorization criteria strongly correlate with the number of occurrences in the training set, capturing memorized familiar phrases, public knowledge, templated texts, or other repeated data.We formulate a notion of counterfactual memorization which characterizes how a model's predictions change if a particular document is omitted during training.We identify and study counterfactually-memorized training examples in standard text datasets.We estimate the influence of each memorized training example on the validation set and on generated texts, showing how this can provide direct evidence of the source of memorization at test time.

摘要:

广泛应用于各种 NLP 任务的现代神经语言模型存在记忆训练数据中敏感信息的风险。理解这种记忆对于现实世界的应用以及从学习理论的角度来看都很重要。先前语言模型记忆研究中的一个悬而未决的问题是如何过滤掉“常见”记忆。事实上，大多数记忆标准与训练集中出现的次数密切相关，捕获记忆的熟悉短语、公共知识、模板文本或其他重复数据。我们提出了反事实记忆的概念，它描述了模型的预测如何改变，如果在训练期间省略特定文档。我们识别并研究标准文本数据集中反事实记忆的训练示例。我们估计每个记忆的训练示例对验证集和生成文本的影响，展示这如何提供直接证据来源考试时的记忆。

## Cheap and Quick: Efficient Vision-Language Instruction Tuning for Large Language Models<sup>poster<sup>

Authors: Gen Luo, Yiyi Zhou, Tianhe Ren, Shengxin Chen, Xiaoshuai Sun, Rongrong Ji

Link: [https://neurips.cc/virtual/2023/poster/70226](https://neurips.cc/virtual/2023/poster/70226)

Abstract:

 Recently,  growing interest has been aroused in extending the multimodal capability of large language models (LLMs), e.g., vision-language (VL) learning, which is regarded as the next milestone of artificial general intelligence. However, existing solutions are prohibitively expensive, which not only need to optimize excessive parameters, but also require another large-scale pre-training before VL instruction tuning. In this paper, we propose a novel and  affordable  solution for the effective VL adaption of LLMs, called  Mixture-of-Modality Adaptation (MMA).  Instead of using large neural networks to connect the image encoder and LLM, MMA adopts lightweight modules, i.e., adapters, to  bridge the gap between LLMs and VL tasks, which also enables the joint optimization of the image and language models. Meanwhile, MMA is also equipped with a routing algorithm to help LLMs achieve an  automatic  shift between single- and multi-modal instructions without compromising their ability of natural language understanding.  To validate MMA, we apply it to a recent LLM called LLaMA and term this formed large vision-language instructed model as LaVIN.  To validate MMA and LaVIN, we conduct extensive experiments  under two setups, namely  multimodal science question answering and multimodal dialogue. The experimental results not only demonstrate the competitive performance and the superior training efficiency  of LaVIN  than existing multimodal LLMs, but also confirm  its  great potential   as a general-purpose chatbot. More importantly, the actual expenditure of LaVIN is extremely cheap, e.g., only 1.4 training hours with 3.8M trainable parameters, greatly confirming the effectiveness of MMA.   Our  code is anonymously released at:  https://anonymous.4open.science/r/LaVIN--1067.

摘要:

最近，人们对扩展大型语言模型（LLM）的多模态能力越来越感兴趣，例如视觉语言（VL）学习，这被认为是通用人工智能的下一个里程碑。然而，现有的解决方案成本高昂，不仅需要优化过多的参数，而且在VL指令调优之前还需要再次进行大规模的预训练。在本文中，我们提出了一种新颖且经济实惠的解决方案，用于 LLM 的有效 VL 适应，称为混合模态适应（MMA）。 MMA没有使用大型神经网络来连接图像编码器和LLM，而是采用轻量级模块（即适配器）来弥合LLM和VL任务之间的差距，这也使得图像和语言模型的联合优化成为可能。同时，MMA还配备了路由算法，帮助法学硕士实现单模态和多模态指令之间的自动切换，而不影响其自然语言理解能力。为了验证 MMA，我们将其应用于最近的一个名为 LLaMA 的法学硕士，并将这种形成的大型视觉语言指导模型称为 LaVIN。为了验证 MMA 和 LaVIN，我们在两种设置下进行了广泛的实验，即多模态科学问答和多模态对话。实验结果不仅证明了 LaVIN 比现有多模态 LLM 的竞争性能和优越的训练效率，而且证实了其作为通用聊天机器人的巨大潜力。更重要的是，LaVIN的实际花费极其低廉，仅需要1.4个小时的训练时间和380万个可训练参数，极大地证实了MMA的有效性。我们的代码匿名发布于：https://anonymous.4open.science/r/LaVIN--1067。

## Fine-Tuning Language Models with Just Forward Passes<sup>oral<sup>

Authors: Sadhika Malladi, Tianyu Gao, Eshaan Nichani, Alex Damian, Jason Lee, Danqi Chen, Sanjeev Arora

Link: [https://neurips.cc/virtual/2023/poster/71437](https://neurips.cc/virtual/2023/poster/71437)

Abstract:

 Fine-tuning language models (LMs) has yielded success on diverse downstream tasks, but as LMs grow in size, backpropagation requires a prohibitively large amount of memory. Zeroth-order (ZO) methods can in principle estimate gradients using only two forward passes but are theorized to be catastrophically slow for optimizing large models. In this work, we propose a memory-efficient zerothorder optimizer (MeZO), adapting the classical ZO-SGD method to operate in-place, thereby fine-tuning LMs with the same memory footprint as inference. For example, with a single A100 80GB GPU, MeZO can train a 30-billion parameter model, whereas fine-tuning with backpropagation can train only a 2.7B LM with the same budget. We conduct comprehensive experiments across model types (masked and autoregressive LMs), model scales (up to 66B), and downstream tasks (classification, multiple-choice, and generation). Our results demonstrate that (1) MeZO significantly outperforms in-context learning and linear probing; (2) MeZO achieves comparable performance to fine-tuning with backpropagation across multiple tasks, with up to 12× memory reduction and up to 2× GPU-hour reduction in our implementation; (3) MeZO is compatible with both full-parameter and parameter-efficient tuning techniques such as LoRA and prefix tuning; (4) MeZO can effectively optimize non-differentiable objectives (e.g., maximizing accuracy or F1). We support our empirical findings with theoretical insights, highlighting how adequate pre-training and task prompts enable MeZO to fine-tune huge models, despite classical ZO analyses suggesting otherwise.

摘要:

微调语言模型 (LM) 已在各种下游任务上取得了成功，但随着 LM 规模的增大，反向传播需要大量的内存。零阶 (ZO) 方法原则上可以仅使用两次前向传递来估计梯度，但理论上对于优化大型模型来说速度非常慢。在这项工作中，我们提出了一种内存高效的零阶优化器（MeZO），采用经典的 ZO-SGD 方法进行就地操作，从而以与推理相同的内存占用来微调 LM。例如，使用单个 A100 80GB GPU，MeZO 可以训练 300 亿个参数的模型，而反向传播微调在相同预算下只能训练 2.7B LM。我们对模型类型（屏蔽和自回归 LM）、模型规模（高达 66B）和下游任务（分类、多项选择和生成）进行了全面的实验。我们的结果表明（1）MeZO 显着优于上下文学习和线性探测； (2) MeZO 通过跨多个任务的反向传播实现了与微调相当的性能，在我们的实现中，内存减少了高达 12 倍，GPU 小时减少了高达 2 倍； （3）MeZO兼容全参数和参数高效的调谐技术，例如LoRA和前缀调谐； (4) MeZO可以有效地优化不可微目标（例如，最大化准确率或F1）。我们用理论见解支持我们的实证研究结果，强调充分的预训练和任务提示如何使 MeZO 能够微调巨大的模型，尽管经典的 ZO 分析表明情况并非如此。

## Parsel🐍: Algorithmic Reasoning with Language Models by Composing Decompositions<sup>poster<sup>

Authors: Eric Zelikman, Qian Huang, Gabriel Poesia, Noah Goodman, Nick Haber

Link: [https://neurips.cc/virtual/2023/poster/70349](https://neurips.cc/virtual/2023/poster/70349)

Abstract:

 Despite recent success in large language model (LLM) reasoning, LLMs struggle with hierarchical multi-step reasoning tasks like generating complex programs. For these tasks, humans often start with a high-level algorithmic design and implement each part gradually. We introduce Parsel, a framework enabling automatic implementation and validation of complex algorithms with code LLMs. With Parsel, we automatically decompose algorithmic tasks into hierarchical natural language function descriptions and then search over combinations of possible function implementations using tests. We show that Parsel can be used across domains requiring hierarchical reasoning, including program synthesis and robotic planning. We find that, using Parsel, LLMs solve more competition-level problems in the APPS dataset, resulting in pass rates over 75\% higher than prior results from directly sampling AlphaCode and Codex, while often using a smaller sample budget. Moreover, with automatically generated tests, we find that Parsel can improve the state-of-the-art pass@1 performance on HumanEval from 67\% to 85\%. We also find that LLM-generated robotic plans using Parsel are more than twice as likely to be considered accurate than directly generated plans. Lastly, we explore how Parsel addresses LLM limitations and discuss how Parsel may be useful for human programmers. We release our code at https://github.com/ezelikman/parsel.

摘要:

尽管最近在大型语言模型 (LLM) 推理方面取得了成功，但 LLM 仍难以处理分层多步骤推理任务，例如生成复杂的程序。对于这些任务，人类通常从高级算法设计开始，逐步实现每个部分。我们引入了 Parsel，这是一个能够使用代码法学硕士自动实现和验证复杂算法的框架。使用 Parsel，我们自动将算法任务分解为分层自然语言函数描述，然后使用测试搜索可能的函数实现的组合。我们证明 Parsel 可以跨需要分层推理的领域使用，包括程序综合和机器人规划。我们发现，LLM 使用 Parsel 解决了 APPS 数据集中更多的竞争级别问题，其通过率比之前直接采样 AlphaCode 和 Codex 的结果高出 75% 以上，同时通常使用较小的样本预算。此外，通过自动生成的测试，我们发现 Parsel 可以将 HumanEval 上最先进的 pass@1 性能从 67% 提高到 85%。我们还发现，使用 Parsel 的 LLM 生成的机器人计划被认为准确的可能性是直接生成的计划的两倍多。最后，我们探讨 Parsel 如何解决 LLM 限制，并讨论 Parsel 如何对人类程序员有用。我们在 https://github.com/ezelikman/parsel 发布了我们的代码。

## MoCa: Measuring Human-Language Model Alignment on Causal and Moral Judgment Tasks<sup>poster<sup>

Authors: Allen Nie, Yuhui Zhang, Atharva Shailesh Amdekar, Chris Piech, Tatsunori Hashimoto, Tobias Gerstenberg

Link: [https://neurips.cc/virtual/2023/poster/71498](https://neurips.cc/virtual/2023/poster/71498)

Abstract:

 Human commonsense understanding of the physical and social world is organized around intuitive theories. These theories support making causal and moral judgments. When something bad happens, we naturally ask: who did what, and why? A rich literature in cognitive science has studied people's causal and moral intuitions. This work has revealed a number of factors that systematically influence people's judgments, such as the violation of norms and whether the harm is avoidable or inevitable. We collected a dataset of stories from 24 cognitive science papers and developed a system to annotate each story with the factors they investigated. Using this dataset, we test whether large language models (LLMs) make causal and moral judgments about text-based scenarios that align with those of human participants. On the aggregate level, alignment has improved with more recent LLMs. However, using statistical analyses, we find that LLMs weigh the different factors quite differently from human participants. These results show how curated, challenge datasets combined with insights from cognitive science can help us go beyond comparisons based merely on aggregate metrics: we uncover LLMs implicit tendencies and show to what extent these align with human intuitions.

摘要:

人类对物理和社会世界的常识性理解是围绕直觉理论组织的。这些理论支持做出因果和道德判断。当不好的事情发生时，我们自然会问：谁做了什么，为什么？认知科学领域的丰富文献研究了人们的因果直觉和道德直觉。这项工作揭示了许多系统性地影响人们判断的因素，例如违反规范以及伤害是否可以避免或不可避免。我们从 24 篇认知科学论文中收集了故事数据集，并开发了一个系统，用他们调查的因素来注释每个故事。使用此数据集，我们测试大型语言模型 (LLM) 是否对基于文本的场景做出与人类参与者一致的因果和道德判断。总体而言，与最近的法学硕士的一致性有所改善。然而，通过统计分析，我们发现法学硕士对不同因素的权衡与人类参与者截然不同。这些结果表明，精心策划的挑战数据集与认知科学的见解相结合如何帮助我们超越仅仅基于总体指标的比较：我们发现法学硕士的隐含倾向，并显示这些倾向在多大程度上与人类直觉相符。

## Pengi: An Audio Language Model for Audio Tasks<sup>poster<sup>

Authors: Soham Deshmukh, Benjamin Elizalde, Rita Singh, Huaming Wang

Link: [https://neurips.cc/virtual/2023/poster/70860](https://neurips.cc/virtual/2023/poster/70860)

Abstract:

 In the domain of audio processing, Transfer Learning has facilitated the rise of Self-Supervised Learning and Zero-Shot Learning techniques. These approaches have led to the development of versatile models capable of tackling a wide array of tasks, while delivering state-of-the-art performance. However, current models inherently lack the capacity to produce the requisite language for open-ended tasks, such as Audio Captioning or Audio Question Answering. We introduce Pengi, a novel Audio Language Model that leverages Transfer Learning by framing all audio tasks as text-generation tasks. It takes as input, an audio recording, and text, and generates free-form text as output. The input audio is represented as a sequence of continuous embeddings by an audio encoder. A text encoder does the same for the corresponding text input. Both sequences are combined as a prefix to prompt a pre-trained frozen language model. The unified architecture of Pengi enables open-ended tasks and close-ended tasks without any additional fine-tuning or task-specific extensions. When evaluated on 21 downstream tasks, our approach yields state-of-the-art performance in several of them. Our results show that connecting language models with audio models is a major step towards general-purpose audio understanding.

摘要:

在音频处理领域，迁移学习促进了自监督学习和零样本学习技术的兴起。这些方法导致了多功能模型的开发，这些模型能够处理各种任务，同时提供最先进的性能。然而，当前的模型本质上缺乏为开放式任务（例如音频字幕或音频问答）生成所需语言的能力。我们介绍 Pengi，一种新颖的音频语言模型，它通过将所有音频任务构建为文本生成任务来利用迁移学习。它以录音和文本作为输入，并生成自由格式的文本作为输出。输入音频由音频编码器表示为一系列连续嵌入。文本编码器对相应的文本输入执行相同的操作。两个序列组合起来作为前缀，以提示预训练的冻结语言模型。 Pengi的统一架构支持开放式任务和封闭式任务，无需任何额外的微调或特定于任务的扩展。当对 21 个下游任务进行评估时，我们的方法在其中几个任务中产生了最先进的性能。我们的结果表明，将语言模型与音频模型连接起来是迈向通用音频理解的重要一步。

## Language Model Alignment with Elastic Reset<sup>poster<sup>

Authors: Michael Noukhovitch, Samuel Lavoie, Florian Strub, Aaron Courville

Link: [https://neurips.cc/virtual/2023/poster/72738](https://neurips.cc/virtual/2023/poster/72738)

Abstract:

 Finetuning language models with reinforcement learning (RL), e.g. from human feedback (HF), is a prominent method for alignment. But optimizing against a reward model can improve on reward while degrading performance in other areas, a phenomenon known as reward hacking, alignment tax, or language drift. First, we argue that commonly-used test metrics are insufficient and instead measure how different algorithms tradeoff between reward and drift. The standard method modified the reward with a Kullback-Lieber (KL) penalty between the online and initial model. We propose Elastic Reset, a new algorithm that achieves higher reward with less drift without explicitly modifying the training objective. We periodically reset the online model to an exponentially moving average (EMA) of itself, then reset the EMA model to the initial model. Through the use of an EMA, our model recovers quickly after resets and achieves higher reward with less drift in the same number of steps. We demonstrate that fine-tuning language models with Elastic Reset leads to state-of-the-art performance on a small scale pivot-translation benchmark, outperforms all baselines in a medium-scale RLHF-like IMDB mock sentiment task and leads to a more performant and more aligned technical QA chatbot with LLaMA-7B. Code available https://github.com/mnoukhov/elastic-reset

摘要:

通过强化学习（RL）（例如根据人类反馈（HF））微调语言模型是一种重要的对齐方法。但针对奖励模型进行优化可能会提高奖励，同时降低其他领域的表现，这种现象称为奖励黑客、对齐税或语言漂移。首先，我们认为常用的测试指标是不够的，而是衡量不同算法如何在奖励和漂移之间进行权衡。标准方法通过在线模型和初始模型之间的 Kullback-Lieber (KL) 惩罚来修改奖励。我们提出了 Elastic Reset，这是一种新算法，可以在不显式修改训练目标的情况下以更少的漂移实现更高的奖励。我们定期将在线模型重置为其自身的指数移动平均线 (EMA)，然后将 EMA 模型重置为初始模型。通过使用 EMA，我们的模型在重置后可以快速恢复，并在相同步数下以更少的漂移获得更高的奖励。我们证明，使用 Elastic Reset 微调语言模型可以在小规模枢轴翻译基准上实现最先进的性能，在中等规模的类似 RLHF 的 IMDB 模拟情感任务中优于所有基准，并导致更使用 LLaMA-7B 实现高性能且更加一致的技术 QA 聊天机器人。可用代码 https://github.com/mnoukhov/elastic-reset

## HyPoradise: An Open Baseline for Generative Speech Recognition with Large Language Models<sup>poster<sup>

Authors: CHEN CHEN, Yuchen Hu, Chao-Han Huck Yang, Sabato Marco Siniscalchi, Pin-Yu Chen, Eng-Siong Chng

Link: [https://neurips.cc/virtual/2023/poster/73533](https://neurips.cc/virtual/2023/poster/73533)

Abstract:

 Advancements in deep neural networks have allowed automatic speech recognition (ASR) systems to attain human parity on several publicly available clean speech datasets. However, even state-of-the-art ASR systems experience performance degradation when confronted with adverse conditions, as a well-trained acoustic model is sensitive to variations in the speech domain, e.g., background noise. Intuitively, humans address this issue by relying on their linguistic knowledge: the meaning of ambiguous spoken terms is usually inferred from contextual cues thereby reducing the dependency on the auditory system. Inspired by this observation, we introduce the first open-source benchmark to utilize external large language models (LLMs) for ASR error correction, where N-best decoding hypotheses provide informative elements for true transcription prediction. This approach is a paradigm shift from the traditional language model rescoring strategy that can only select one candidate hypothesis as output transcription. The proposed benchmark contains a novel dataset, "HyPoradise" (HP), encompassing more than 316,000 pairs of N-best hypotheses and corresponding accurate transcriptions across prevalent speech domains. Given this dataset, we examine three types of error correction techniques based on LLMs with varying amounts of labeled hypotheses-transcription pairs, which gains significant word error rate (WER) reduction. Experimental evidence demonstrates the proposed technique achieves a breakthrough by surpassing the upper bound of traditional re-ranking based methods. More surprisingly, LLM with reasonable prompt design can even correct those tokens that are missing in N-best list. We make our results publicly accessible for reproducible pipelines with released pre-trained models, thus providing a new paradigm for ASR error correction with LLMs.

摘要:

深度神经网络的进步使得自动语音识别（ASR）系统能够在几个公开可用的干净语音数据集上达到人类的同等水平。然而，即使是最先进的 ASR 系统在遇到不利条件时也会经历性能下降，因为训练有素的声学模型对语音域中的变化（例如背景噪声）很敏感。直观上，人类依靠他们的语言知识来解决这个问题：模糊的口头术语的含义通常是从上下文线索推断出来的，从而减少了对听觉系统的依赖。受这一观察的启发，我们引入了第一个开源基准测试，利用外部大语言模型 (LLM) 进行 ASR 纠错，其中 N 最佳解码假设为真实的转录预测提供了信息元素。这种方法是传统语言模型重新评分策略的范式转变，传统语言模型重新评分策略只能选择一个候选假设作为输出转录。拟议的基准包含一个新颖的数据集“HyPoradise”（HP），包含超过 316,000 对 N 最佳假设以及跨流行语音领域的相应准确转录。给定这个数据集，我们检查了三种基于法学硕士的纠错技术，这些技术具有不同数量的标记假设-转录对，从而显着降低了单词错误率 (WER)。实验证据表明，所提出的技术通过超越传统基于重排序的方法的上限实现了突破。更令人惊讶的是，具有合理提示设计的LLM甚至可以纠正N-best列表中缺失的那些标记。我们通过发布的预训练模型将我们的结果公开用于可重复的管道，从而为法学硕士的 ASR 纠错提供了新的范例。

## Guiding Large Language Models via Directional Stimulus Prompting<sup>poster<sup>

Authors: Zekun Li, Baolin Peng, Pengcheng He, Michel Galley, Jianfeng Gao, Xifeng Yan

Link: [https://neurips.cc/virtual/2023/poster/71484](https://neurips.cc/virtual/2023/poster/71484)

Abstract:

 We introduce Directional Stimulus Prompting, a novel framework for guiding black-box large language models (LLMs) towards specific desired outputs. Instead of directly adjusting LLMs, our method employs a small tunable policy model (e.g., T5) to generate an auxiliary directional stimulus prompt for each input instance. These directional stimulus prompts act as nuanced, instance-specific hints and clues to guide LLMs in generating desired outcomes, such as including specific keywords in the generated summary. Our approach sidesteps the challenges of direct LLM tuning by optimizing the policy model to explore directional stimulus prompts that align LLMs with desired behaviors. The policy model can be optimized through 1) supervised fine-tuning using labeled data and 2) reinforcement learning from offline or online rewards based on the LLM's output. We evaluate our method across various tasks, including summarization, dialogue response generation, and chain-of-thought reasoning. Our experiments indicate a consistent improvement in the performance of LLMs such as ChatGPT, Codex, and InstructGPT on these supervised tasks with minimal labeled data. Remarkably, by utilizing merely 80 dialogues from the MultiWOZ dataset, our approach boosts ChatGPT's performance by a relative 41.4%, achieving or exceeding the performance of some fully supervised state-of-the-art models. Moreover, the instance-specific chain-of-thought prompt generated through our method enhances InstructGPT's reasoning accuracy, outperforming both generalized human-crafted prompts and those generated through automatic prompt engineering. The code and data are publicly available at https://github.com/Leezekun/Directional-Stimulus-Prompting.

摘要:

我们引入了定向刺激提示，这是一种新颖的框架，用于指导黑盒大语言模型（LLM）实现特定的所需输出。我们的方法不是直接调整 LLM，而是采用一个小型可调策略模型（例如 T5）来为每个输入实例生成辅助定向刺激提示。这些定向刺激提示充当细致入微的、特定于实例的提示和线索，指导法学硕士生成所需的结果，例如在生成的摘要中包含特定的关键字。我们的方法通过优化政策模型来探索使法学硕士与期望行为保持一致的定向刺激提示，从而回避了直接法学硕士调整的挑战。政策模型可以通过 1）使用标记数据进行监督微调和 2）基于 LLM 输出的离线或在线奖励进行强化学习来优化。我们在各种任务中评估我们的方法，包括摘要、对话响应生成和思想链推理。我们的实验表明，ChatGPT、Codex 和 InstructGPT 等 LLM 在使用最少标记数据的监督任务上的性能得到了持续改进。值得注意的是，通过仅利用 MultiWOZ 数据集中的 80 个对话，我们的方法将 ChatGPT 的性能提高了相对 41.4%，达到或超过了一些完全监督的最先进模型的性能。此外，通过我们的方法生成的特定于实例的思维链提示提高了 InstructGPT 的推理准确性，优于广义的人工制作的提示和通过自动提示工程生成的提示。代码和数据可在 https://github.com/Leezekun/Directional-Stimulus-Prompting 上公开获取。

## Evaluating and Inducing Personality in Pre-trained Language Models<sup>poster<sup>

Authors: Guangyuan Jiang, Manjie Xu, Song-Chun Zhu, Wenjuan Han, Chi Zhang, Yixin Zhu

Link: [https://neurips.cc/virtual/2023/poster/72136](https://neurips.cc/virtual/2023/poster/72136)

Abstract:

 Standardized and quantified evaluation of machine behaviors is a crux of understanding LLMs. In this study, we draw inspiration from psychometric studies by leveraging human personality theory as a tool for studying machine behaviors. Originating as a philosophical quest for human behaviors, the study of personality delves into how individuals differ in thinking, feeling, and behaving. Toward building and understanding human-like social machines, we are motivated to ask: Can we assess machine behaviors by leveraging human psychometric tests in a **principled** and **quantitative** manner? If so, can we induce a specific personality in LLMs? To answer these questions, we introduce the Machine Personality Inventory (MPI) tool for studying machine behaviors; MPI follows standardizedpersonality tests, built upon the Big Five Personality Factors (Big Five) theory and personality assessment inventories. By systematically evaluating LLMs with MPI, we provide the first piece of evidence demonstrating the efficacy of MPI in studying LLMs behaviors. We further devise a Personality Prompting (P$^2$) method to induce LLMs with specific personalities in a **controllable** way, capable of producing diverse and verifiable behaviors. We hope this work sheds light on future studies by adopting personality as the essential indicator for various downstream tasks, and could further motivate research into equally intriguing human-like machine behaviors.

摘要:

机器行为的标准化和量化评估是理解法学硕士的关键。在这项研究中，我们利用人类人格理论作为研究机器行为的工具，从心理测量研究中汲取灵感。人格研究起源于对人类行为的哲学探索，深入研究个体在思维、情感和行为方面的差异。为了构建和理解类人的社交机器，我们不禁要问：我们能否以**有原则的**和**定量的**方式利用人类心理测试来评估机器行为？如果是这样，我们能否在法学硕士中引入特定的个性？为了回答这些问题，我们引入了机器个性清单（MPI）工具来研究机器行为； MPI 遵循基于大五人格因素（大五）理论和人格评估量表的标准化人格测试。通过使用 MPI 系统地评估法学硕士，我们提供了第一个证据，证明 MPI 在研究法学硕士行为方面的有效性。我们进一步设计了一种人格提示（P$^2$）方法，以**可控**的方式诱导具有特定人格的LLM，能够产生多样化且可验证的行为。我们希望这项工作通过采用个性作为各种下游任务的基本指标来为未来的研究带来启示，并可以进一步推动对同样有趣的类人机器行为的研究。

## On-the-Fly Adapting Code Summarization on Trainable Cost-Effective Language Models<sup>poster<sup>

Authors: Yufan Cai, Yun Lin, Chenyan Liu, Jinglian Wu, Yifan Zhang, Yiming Liu, Yeyun Gong, Jin Song Dong

Link: [https://neurips.cc/virtual/2023/poster/71669](https://neurips.cc/virtual/2023/poster/71669)

Abstract:

 Deep learning models are emerging to summarize source code to comment,  facilitating tasks of code documentation and program comprehension.  Scaled-up large language models trained on large open corpus have achieved good performance in such tasks.  However, in practice, the subject code in one certain project can be specific,  which may not align with the overall training corpus.  Some code samples from other projects may be contradictory and introduce inconsistencies when the models try to fit all the samples.  In this work, we introduce a novel approach, Adacom, to improve the performance of comment generators by on-the-fly model adaptation.  This research is motivated by the observation that deep comment generators  often need to strike a balance as they need to fit all the training samples.  Specifically, for one certain target code $c$,  some training samples $S_p$ could have made more contributions while other samples $S_o$ could have counter effects.  However, the traditional fine-tuned models need to fit both $S_p$ and $S_o$ from a global perspective,   leading to compromised performance for one certain target code $c$.  In this context, we design Adacom to  (1) detect whether the model might have a compromised performance on a target code $c$ and  (2) retrieve a few helpful training samples $S_p$ that have contradictory samples in the training dataset and,  (3) adapt the model on the fly by re-training the $S_p$ to strengthen the helpful samples and unlearn the harmful samples.  Our extensive experiments on 7 comment generators and 4 public datasets show that  (1) can significantly boost the performance of comment generation (BLEU4 score by on average 14.9\%, METEOR by 12.2\%, and ROUGE-L by 7.4\%),  (2) the adaptation on one code sample is cost-effective and acceptable as an on-the-fly solution, and  (3) can adapt well on out-of-distribution code samples.

摘要:

深度学习模型正在兴起，可以总结源代码以进行注释，从而促进代码文档和程序理解的任务。在大型开放语料库上训练的扩展大型语言模型在此类任务中取得了良好的性能。然而，在实践中，某个项目中的主题代码可能是特定的，这可能与整体训练语料库不一致。来自其他项目的某些代码示例可能会相互矛盾，并且当模型尝试拟合所有示例时会引入不一致。在这项工作中，我们引入了一种新颖的方法 Adacom，通过动态模型适应来提高评论生成器的性能。这项研究的动机是观察到深度评论生成器通常需要取得平衡，因为它们需要适合所有训练样本。具体来说，对于某个目标代码$c$，某些训练样本$S_p$可能会做出更多贡献，而其他样本$S_o$可能会产生相反的效果。然而，传统的微调模型需要从全局角度同时拟合$S_p$和$S_o$，导致某个目标代码$c$的性能受到影响。在这种情况下，我们设计 Adacom 来 (1) 检测模型在目标代码 $c$ 上的性能是否可能受到影响，以及 (2) 检索一些有用的训练样本 $S_p$，这些样本在训练数据集中具有矛盾的样本，并且， (3) 通过重新训练 $S_p$ 来动态调整模型，以加强有用的样本并忘记有害的样本。我们对 7 个评论生成器和 4 个公共数据集进行的广泛实验表明，(1) 可以显着提高评论生成的性能（BLEU4 得分平均提高 14.9%，METEOR 平均提高 12.2%，ROUGE-L 平均提高 7.4%）， (2) 对一个代码样本的适应作为一种即时解决方案是具有成本效益且可接受的，并且 (3) 可以很好地适应分布外的代码样本。

## Generating Images with Multimodal Language Models<sup>poster<sup>

Authors: Jing Yu Koh, Daniel Fried, Russ Salakhutdinov

Link: [https://neurips.cc/virtual/2023/poster/71499](https://neurips.cc/virtual/2023/poster/71499)

Abstract:

 We propose a method to fuse frozen text-only large language models (LLMs) with pre-trained image encoder and decoder models, by mapping between their embedding spaces. Our model demonstrates a wide suite of multimodal capabilities: image retrieval, novel image generation, and multimodal dialogue. Ours is the first approach capable of conditioning on arbitrarily interleaved image and text inputs to generate coherent image (and text) outputs. To achieve strong performance on image generation, we propose an efficient mapping network to ground the LLM to an off-the-shelf text-to-image generation model. This mapping network translates hidden representations of text into the embedding space of the visual models, enabling us to leverage the strong text representations of the LLM for visual outputs. Our approach outperforms baseline generation models on tasks with longer and more complex language. In addition to novel image generation, our model is also capable of image retrieval from a prespecified dataset, and decides whether to retrieve or generate at inference time. This is done with a learnt decision module which conditions on the hidden representations of the LLM. Our model exhibits a wider range of capabilities compared to prior multimodal language models. It can process image-and-text inputs, and produce retrieved images, generated images, and generated text — outperforming non-LLM based generation models across several text-to-image tasks that measure context dependence.

摘要:

我们提出了一种方法，通过嵌入空间之间的映射，将冻结的纯文本大语言模型（LLM）与预训练的图像编码器和解码器模型融合。我们的模型展示了一系列广泛的多模态功能：图像检索、新颖图像生成和多模态对话。我们的方法是第一种能够对任意交错的图像和文本输入进行调节以生成连贯的图像（和文本）输出的方法。为了在图像生成方面实现强大的性能，我们提出了一种高效的映射网络，将法学硕士转化为现成的文本到图像生成模型。该映射网络将文本的隐藏表示转换为视觉模型的嵌入空间，使我们能够利用 LLM 的强大文本表示进行视觉输出。我们的方法在使用更长、更复杂的语言的任务上优于基线生成模型。除了新颖的图像生成之外，我们的模型还能够从预先指定的数据集中进行图像检索，并在推理时决定是检索还是生成。这是通过学习决策模块完成的，该模块以法学硕士的隐藏表示为条件。与之前的多模态语言模型相比，我们的模型展示了更广泛的功能。它可以处理图像和文本输入，并生成检索的图像、生成的图像和生成的文本——在多个测量上下文依赖性的文本到图像任务中，其性能优于非基于 LLM 的生成模型。

## Emergent and Predictable Memorization in Large Language Models<sup>poster<sup>

Authors: Stella Biderman, USVSN PRASHANTH, Lintang Sutawika, Hailey Schoelkopf, Quentin Anthony, Shivanshu Purohit, Edward Raff

Link: [https://neurips.cc/virtual/2023/poster/72096](https://neurips.cc/virtual/2023/poster/72096)

Abstract:

 Memorization, or the tendency of large language models (LLMs) to output entire sequences from their training data verbatim, is a key concern for deploying language models. In particular, it is vital to minimize a model's memorization of sensitive datapoints such as those containing personal identifiable information (PII). The prevalence of such undesirable memorization can pose issues for model trainers, and may even require discarding an otherwise functional model. We therefore seek to predict which sequences will be memorized before a large model's full train-time by extrapolating the memorization behavior of lower-compute trial runs. We measure memorization in the Pythia model suite and plot scaling laws for forecasting memorization, allowing us to provide equi-compute recommendations to maximize the reliability (recall) of such predictions. We additionally provide further novel discoveries on the distribution of memorization scores across models and data. We release all code and data necessary to reproduce the results in this paper at https://github.com/EleutherAI/pythia.

摘要:

记忆，或者说大型语言模型（LLM）从训练数据中逐字输出整个序列的趋势，是部署语言模型的一个关键问题。特别是，尽量减少模型对敏感数据点（例如包含个人身份信息 (PII) 的数据点）的记忆至关重要。这种不良记忆的普遍存在会给模型训练者带来问题，甚至可能需要丢弃其他功能模型。因此，我们试图通过推断较低计算量试运行的记忆行为来预测在大型模型的完整训练时间之前将记住哪些序列。我们在 Pythia 模型套件中测量记忆力，并绘制用于预测记忆力的缩放定律，使我们能够提供等计算建议，以最大限度地提高此类预测的可靠性（召回率）。我们还提供了关于模型和数据的记忆分数分布的进一步新发现。我们在 https://github.com/EleutherAI/pythia 发布了重现本文结果所需的所有代码和数据。

## OpenAssistant Conversations - Democratizing Large Language Model Alignment<sup>oral<sup>

Authors: Andreas Köpf, Yannic Kilcher, Dimitri von Rütte, Sotiris Anagnostidis, Zhi Rui Tam, Keith Stevens, Abdullah Barhoum, Duc Nguyen, Oliver Stanley, Richárd Nagyfi, Shahul ES, Sameer Suri, David Glushkov, Arnav Dantuluri, Andrew Maguire, Christoph Schuhmann, Huu Nguyen, Alexander Mattick

Link: [https://neurips.cc/virtual/2023/poster/73573](https://neurips.cc/virtual/2023/poster/73573)

Abstract:

 Aligning large language models (LLMs) with human preferences has proven to drastically improve usability and has driven rapid adoption as demonstrated by ChatGPT.Alignment techniques such as supervised fine-tuning (\textit{SFT}) and  reinforcement learning from human feedback (\textit{RLHF}) greatly reduce the required skill and domain knowledge to effectively harness the capabilities of LLMs, increasing their accessibility and utility across various domains.However, state-of-the-art alignment techniques like \textit{RLHF} rely on high-quality human feedback data, which is expensive to create and often remains proprietary.In an effort to democratize research on large-scale alignment, we release OpenAssistant Conversations, a human-generated, human-annotated assistant-style conversation corpus consisting of 161,443 messages in 35 different languages, annotated with 461,292 quality ratings, resulting in over 10,000 complete and fully annotated conversation trees.The corpus is a product of a worldwide crowd-sourcing effort involving over 13,500 volunteers.Models trained on OpenAssistant Conversations show consistent improvements on standard benchmarks over respective base models.We release our code\footnote{\git} and data\footnote{\data} under a fully permissive licence.

摘要:

事实证明，将大语言模型 (LLM) 与人类偏好结合起来可以极大地提高可用性，并推动了快速采用，如 ChatGPT 所证明的那样。对齐技术，例如监督微调 (\textit{SFT}) 和来自人类反馈的强化学习 ( \textit{RLHF}) 大大减少了有效利用法学硕士能力所需的技能和领域知识，提高了其在各个领域的可访问性和实用性。然而，像 \textit{RLHF} 这样最先进的对齐技术依赖于高质量的人类反馈数据，这些数据的创建成本很高，而且通常仍然是专有的。为了使大规模对齐的研究民主化，我们发布了 OpenAssistant Conversations，这是一个由人类生成、人类注释的助理式对话语料库，包含 161,443 个对话语料库35 种不同语言的消息，带有 461,292 个质量评级注释，从而产生了超过 10,000 个完整且带注释的对话树。该语料库是全球众包工作的成果，涉及超过 13,500 名志愿者。在 OpenAssistant Conversations 上训练的模型显示出标准的持续改进对各自基本模型的基准测试。我们在完全许可的许可下发布我们的代码\脚注{\git}和数据\脚注{\数据}。

## RRHF: Rank Responses to Align Language Models with Human Feedback<sup>poster<sup>

Authors: Hongyi Yuan, Zheng Yuan, Chuanqi Tan, Wei Wang, Songfang Huang, Fei Huang

Link: [https://neurips.cc/virtual/2023/poster/72308](https://neurips.cc/virtual/2023/poster/72308)

Abstract:

 Reinforcement Learning from Human Feedback (RLHF) facilitates the alignment of large language models with human preferences, significantly enhancing the quality of interactions between humans and models. InstructGPT implements RLHF through several stages, including Supervised Fine-Tuning (SFT), reward model training, and Proximal Policy Optimization (PPO). However, PPO is sensitive to hyperparameters and requires multiple models in its standard implementation, making it hard to train and scale up to larger parameter counts.In contrast, we propose a novel learning paradigm called RRHF, which scores sampled responses from different sources via a logarithm of conditional probabilities and learns to align these probabilities with human preferences through ranking loss.RRHF can leverage sampled responses from various sources including the model responses from itself, other large language model responses, and human expert responses to learn to rank them.RRHF only needs 1 to 2 models during tuning and can efficiently align language models with human preferences robustly without complex hyperparameter tuning. Additionally, RRHF can be considered an extension of SFT and reward model training while being simpler than PPO in terms of coding, model counts, and hyperparameters. We evaluate RRHF on the Helpful and Harmless dataset, demonstrating comparable alignment performance with PPO by reward model score and human labeling.Extensive experiments show that the performance of RRHF is highly related to sampling quality which suggests RRHF is a best-of-$n$ learner.

摘要:

人类反馈强化学习（RLHF）有助于将大型语言模型与人类偏好保持一致，从而显着提高人类与模型之间的交互质量。 InstructGPT 通过多个阶段实现 RLHF，包括监督微调 (SFT)、奖励模型训练和近端策略优化 (PPO)。然而，PPO 对超参数很敏感，并且在其标准实现中需要多个模型，这使得训练和扩展到更大的参数数量变得困难。相反，我们提出了一种称为 RRHF 的新颖学习范式，它通过条件概率的对数，并学习通过排名损失将这些概率与人类偏好保持一致。RRHF 可以利用各种来源的采样响应，包括自身的模型响应、其他大型语言模型响应和人类专家响应来学习对它们进行排名。仅限 RRHF在调优过程中需要 1 到 2 个模型，并且可以有效地将语言模型与人类偏好稳健地结合起来，而无需复杂的超参数调优。此外，RRHF 可以被认为是 SFT 和奖励模型训练的扩展，同时在编码、模型计数和超参数方面比 PPO 更简单。我们在 Helpful and Harmless 数据集上评估 RRHF，通过奖励模型评分和人工标记展示了与 PPO 相当的对齐性能。大量实验表明 RRHF 的性能与采样质量高度相关，这表明 RRHF 是 $n$ 中最好的学习者。

## Can Language Models Solve Graph Problems in Natural Language?<sup>poster<sup>

Authors: Heng Wang, Shangbin Feng, Tianxing He, Zhaoxuan Tan, Xiaochuang Han, Yulia Tsvetkov

Link: [https://neurips.cc/virtual/2023/poster/71520](https://neurips.cc/virtual/2023/poster/71520)

Abstract:

 Large language models (LLMs) are increasingly adopted for a variety of tasks with implicit graphical structures, such as planning in robotics, multi-hop question answering or knowledge probing, structured commonsense reasoning, and more. While LLMs have advanced the state-of-the-art on these tasks with structure implications, whether LLMs could explicitly process textual descriptions of graphs and structures, map them to grounded conceptual spaces, and perform structured operations remains underexplored. To this end, we propose NLGraph (Natural Language Graph), a comprehensive benchmark of graph-based problem solving designed in natural language. NLGraph contains 29,370 problems, covering eight graph reasoning tasks with varying complexity from simple tasks such as connectivity and shortest path up to complex problems such as maximum flow and simulating graph neural networks. We evaluate LLMs (GPT-3/4) with various prompting approaches on the NLGraph benchmark and find that 1) language models do demonstrate preliminary graph reasoning abilities, 2) the benefit of advanced prompting and in-context learning diminishes on more complex graph problems, while 3) LLMs are also (un)surprisingly brittle in the face of spurious correlations in graph and problem settings. We then propose Build-a-Graph Prompting and Algorithmic Prompting, two instruction-based approaches to enhance LLMs in solving natural language graph problems. Build-a-Graph and Algorithmic prompting improve the performance of LLMs on NLGraph by 3.07% to 16.85% across multiple tasks and settings, while how to solve the most complicated graph reasoning tasks in our setup with language models remains an open research question.

摘要:

大型语言模型（LLM）越来越多地应用于具有隐式图形结构的各种任务，例如机器人规划、多跳问答或知识探索、结构化常识推理等。虽然法学硕士在这些具有结构含义的任务上取得了最先进的成果，但法学硕士是否可以显式处理图形和结构的文本描述、将它们映射到扎根的概念空间并执行结构化操作仍待探索。为此，我们提出了NLGraph（自然语言图），这是一个用自然语言设计的基于图的问题解决的综合基准。 NLGraph 包含 29,370 个问题，涵盖八种复杂程度不同的图推理任务，从连接性和最短路径等简单任务到最大流和模拟图神经网络等复杂问题。我们在 NLGraph 基准上使用各种提示方法评估法学硕士 (GPT-3/4)，发现 1) 语言模型确实展示了初步的图形推理能力，2) 高级提示和上下文学习的好处在更复杂的图形问题上会减弱，而3）法学硕士在面对图形和问题设置中的虚假相关性时也（并不）令人惊讶地脆弱。然后，我们提出构建图提示和算法提示，这两种基于指令的方法可以增强法学硕士解决自然语言图问题的能力。构建图和算法提示将 NLGraph 上的法学硕士在多个任务和设置中的性能提高了 3.07% 至 16.85%，而如何使用语言模型解决我们设置中最复杂的图推理任务仍然是一个开放的研究问题。

## Language Models Can Improve Event Prediction by Few-Shot Abductive Reasoning<sup>poster<sup>

Authors: Xiaoming Shi, Siqiao Xue, Kangrui Wang, Fan Zhou, James Zhang, Jun Zhou, Chenhao Tan, Hongyuan Mei

Link: [https://neurips.cc/virtual/2023/poster/71194](https://neurips.cc/virtual/2023/poster/71194)

Abstract:

 Large language models have shown astonishing performance on a wide range of reasoning tasks. In this paper, we investigate whether they could reason about real-world events and help improve the prediction performance of event sequence models. We design LAMP, a framework that integrates a large language model in event prediction. Particularly, the language model performs abductive reasoning to assist an event sequence model: the event model proposes predictions on future events given the past; instructed by a few expert-annotated demonstrations, the language model learns to suggest possible causes for each proposal; a search module finds out the previous events that match the causes; a scoring function learns to examine whether the retrieved events could actually cause the proposal. Through extensive experiments on several challenging real-world datasets, we demonstrate that our framework---thanks to the reasoning capabilities of large language models---could significantly outperform the state-of-the-art event sequence models.

摘要:

大型语言模型在广泛的推理任务中表现出了惊人的性能。在本文中，我们研究它们是否可以推理现实世界的事件并帮助提高事件序列模型的预测性能。我们设计了LAMP，一个在事件预测中集成大型语言模型的框架。特别地，语言模型执行溯因推理来辅助事件序列模型：事件模型提出对给定过去的未来事件的预测；在一些专家注释的演示的指导下，语言模型学会为每个提案提出可能的原因；搜索模块找出与原因匹配的先前事件；评分函数学习检查检索到的事件是否确实会导致提案。通过对几个具有挑战性的现实世界数据集进行的广泛实验，我们证明了我们的框架——得益于大型语言模型的推理能力——可以显着优于最先进的事件序列模型。

## Skill-it! A data-driven skills framework for understanding and training language models<sup>poster<sup>

Authors: Mayee Chen, Nicholas Roberts, Kush Bhatia, Jue WANG, Ce Zhang, Frederic Sala, Christopher Ré

Link: [https://neurips.cc/virtual/2023/poster/72098](https://neurips.cc/virtual/2023/poster/72098)

Abstract:

 The quality of training data impacts the performance of pre-trained large language models (LMs). Given a fixed budget of tokens, we study how to best select data that leads to good downstream model performance across tasks. We develop a new framework based on a simple hypothesis: just as humans acquire interdependent skills in a deliberate order, language models also follow a natural order when learning a set of skills from their training data. If such an order exists, it can be utilized for improved understanding of LMs and for data-efficient training. Using this intuition, our framework formalizes the notion of a skill and of an ordered set of skills in terms of the associated data. First, using both synthetic and real data, we demonstrate that these ordered skill sets exist, and that their existence enables more advanced skills to be learned with less data when we train on their prerequisite skills. Second, using our proposed framework, we introduce an online data sampling algorithm, Skill-It, over mixtures of skills for both continual pre-training and fine-tuning regimes, where the objective is to efficiently learn multiple skills in the former and an individual skill in the latter. On the LEGO synthetic in the continual pre-training setting, Skill-It obtains 37.5 points higher accuracy than random sampling. On the Natural Instructions dataset in the fine-tuning setting, Skill-It reduces the validation loss on the target skill by 13.6% versus training on data associated with the target skill itself. We apply our skills framework on the RedPajama dataset to continually pre-train a 3B-parameter LM, achieving higher accuracy on the LM Evaluation Harness with 1B tokens than the baseline approach of sampling uniformly over data sources with 3B tokens.

摘要:

训练数据的质量影响预训练大型语言模型（LM）的性能。给定固定的代币预算，我们研究如何最好地选择数据，从而在任务中实现良好的下游模型性能。我们基于一个简单的假设开发了一个新框架：正如人类以有意的顺序获得相互依赖的技能一样，语言模型在从训练数据中学习一组技能时也遵循自然顺序。如果存在这样的顺序，它可以用于增进对 LM 的理解和数据高效的训练。利用这种直觉，我们的框架根据相关数据形式化了技能和有序技能集的概念。首先，使用合成数据和真实数据，我们证明了这些有序技能集的存在，并且当我们训练其必备技能时，它们的存在使得能够用更少的数据学习更高级的技能。其次，使用我们提出的框架，我们引入了一种在线数据采样算法 Skill-It，该算法混合了持续预训练和微调制度的技能，其目标是有效地学习前者和个人的多种技能后者的技能。在连续预训练设置中的乐高合成上，Skill-It 的准确度比随机采样高 37.5 个百分点。在微调设置的自然指令数据集上，与目标技能本身相关数据的训练相比，Skill-It 将目标技能的验证损失减少了 13.6%。我们在 RedPajama 数据集上应用我们的技能框架来持续预训练 3B 参数 LM，使用 1B 令牌在 LM 评估工具上实现比使用 3B 令牌在数据源上均匀采样的基线方法更高的准确度。

## Large Language Model as Attributed Training Data Generator: A Tale of Diversity and Bias<sup>poster<sup>

Authors: Yue Yu, Yuchen Zhuang, Jieyu Zhang, Yu Meng, Alexander Ratner, Ranjay Krishna, Jiaming Shen, Chao Zhang

Link: [https://neurips.cc/virtual/2023/poster/73693](https://neurips.cc/virtual/2023/poster/73693)

Abstract:

 Large language models (LLMs) have been recently leveraged as training data generators for various natural language processing (NLP) tasks. While previous research has explored different approaches to training models using generated data, they generally rely on simple class-conditional prompts, which may limit the diversity of the generated data and inherit systematic biases of LLM. Thus, we investigate training data generation with diversely attributed prompts (e.g., specifying attributes like length and style), which have the potential to yield diverse and attributed generated data. Our investigation focuses on datasets with high cardinality and diverse domains, wherein we demonstrate that attributed prompts outperform simple class-conditional prompts in terms of the resulting model's performance. Additionally, we present a comprehensive empirical study on data generation encompassing vital aspects like bias, diversity, and efficiency, and highlight three key observations: firstly, synthetic datasets generated by simple prompts exhibit significant biases, such as regional bias; secondly, attribute diversity plays a pivotal role in enhancing model performance; lastly, attributed prompts achieve the performance of simple class-conditional prompts while utilizing only 5\% of the querying cost of ChatGPT associated with the latter. The data and code are available on {\url{https://github.com/yueyu1030/AttrPrompt}}.

摘要:

大型语言模型（LLM）最近被用作各种自然语言处理（NLP）任务的训练数据生成器。虽然之前的研究探索了使用生成数据训练模型的不同方法，但它们通常依赖于简单的类条件提示，这可能会限制生成数据的多样性并继承法学硕士的系统偏差。因此，我们研究具有不同属性提示的训练数据生成（例如，指定长度和样式等属性），这有可能产生不同的属性生成数据。我们的研究重点是具有高基数和不同领域的数据集，其中我们证明，就生成的模型性能而言，归因提示优于简单的类条件提示。此外，我们对数据生成进行了全面的实证研究，涵盖了偏差、多样性和效率等重要方面，并强调了三个关键观察结果：首先，通过简单提示生成的合成数据集表现出显着的偏差，例如区域偏差；其次，属性多样性对于提高模型性能起着关键作用；最后，属性提示实现了简单类条件提示的性能，而仅利用与后者相关的 ChatGPT 的 5\% 查询成本。数据和代码可以在 {\url{https://github.com/yueyu1030/AttrPrompt}} 上找到。

## Distributed Inference and Fine-tuning of Large Language Models Over The Internet<sup>poster<sup>

Authors: Alexander Borzunov, Max Ryabinin, Artem Chumachenko, Dmitry Baranchuk, Tim Dettmers, Younes Belkada, Pavel Samygin, Colin Raffel

Link: [https://neurips.cc/virtual/2023/poster/71336](https://neurips.cc/virtual/2023/poster/71336)

Abstract:

 Large language models (LLMs) are useful in many NLP tasks and become more capable with size, with the best open-source models having over 50 billion parameters. However, using these 50B+ models requires high-end hardware, making them inaccessible to most researchers. In this work, we investigate methods for cost-efficient inference and fine-tuning of LLMs, comparing local and distributed strategies. We observe that a large enough model (50B+) can run efficiently even on geodistributed devices in a consumer-grade network. This could allow running LLM efficiently by pooling together idle compute resources of multiple research groups and volunteers. We address two open problems: (1) how to perform inference and fine-tuning reliably if any device can disconnect abruptly and (2) how to partition LLMs between devices with uneven hardware, joining and leaving at will. In order to do that, we develop special fault-tolerant inference algorithms and load-balancing protocols that automatically assign devices to maximize the total system throughput. We showcase these algorithms in Petals — a decentralized system that runs Llama 2 (70B) and BLOOM (176B) over the Internet up to $10\times$ faster than offloading for interactive generation. We evaluate the performance of our system in simulated conditions and a real-world setup spanning two continents.

摘要:

大型语言模型 (LLM) 在许多 NLP 任务中非常有用，并且随着规模的增大而变得更加强大，最好的开源模型拥有超过 500 亿个参数。然而，使用这些 50B+ 模型需要高端硬件，这使得大多数研究人员无法使用它们。在这项工作中，我们研究了 LLM 的经济有效的推理和微调方法，比较了本地和分布式策略。我们观察到，即使在消费级网络中的地理分布式设备上，足够大的模型（50B+）也可以高效运行。这可以通过将多个研究小组和志愿者的闲置计算资源集中在一起来有效地运行法学硕士。我们解决了两个悬而未决的问题：（1）如果任何设备突然断开连接，如何可靠地执行推理和微调；（2）如何在硬件不均匀的设备之间划分LLM，随意加入和离开。为此，我们开发了特殊的容错推理算法和负载平衡协议，可以自动分配设备以最大化系统总吞吐量。我们在 Petals 中展示了这些算法，这是一个去中心化系统，通过互联网运行 Llama 2 (70B) 和 BLOOM (176B)，比交互式生成卸载速度快 10 倍。我们在模拟条件和跨越两大洲的现实世界设置中评估系统的性能。

## TrojLLM: A Black-box Trojan Prompt Attack on Large Language Models<sup>poster<sup>

Authors: Jiaqi Xue, Mengxin Zheng, Ting Hua, Yilin Shen, Yepeng Liu, Ladislau Bölöni, Qian Lou

Link: [https://neurips.cc/virtual/2023/poster/71224](https://neurips.cc/virtual/2023/poster/71224)

Abstract:

 Large Language Models (LLMs) are progressively being utilized as machine learning services and interface tools for various applications. However, the security implications of LLMs, particularly in relation to adversarial and Trojan attacks, remain insufficiently examined. In this paper, we propose TrojLLM, an automatic and black-box framework to effectively generate universal and stealthy triggers. When these triggers are incorporated into the input data, the LLMs' outputs can be maliciously manipulated.   Moreover, the framework also supports embedding Trojans within discrete prompts, enhancing the overall effectiveness and precision of the triggers' attacks.  Specifically, we propose a trigger discovery algorithm for generating universal triggers for various inputs by querying victim LLM-based APIs using few-shot data samples. Furthermore, we introduce a novel progressive Trojan poisoning algorithm designed to generate poisoned prompts that retain efficacy and transferability across a diverse range of models. Our experiments and results demonstrate TrojLLM's capacity to effectively insert Trojans into text prompts in real-world black-box LLM APIs including GPT-3.5 and GPT-4, while maintaining exceptional performance on clean test sets. Our work sheds light on the potential security risks in current models and offers a potential defensive approach. The source code of TrojLLM is available at https://github.com/UCF-ML-Research/TrojLLM.

摘要:

大型语言模型（LLM）正逐渐被用作各种应用程序的机器学习服务和接口工具。然而，法学硕士的安全影响，特别是与对抗性和特洛伊木马攻击有关的影响，仍未得到充分研究。在本文中，我们提出了 TrojLLM，一种自动黑盒框架，可有效生成通用且隐秘的触发器。当这些触发器被合并到输入数据中时，法学硕士的输出可能会被恶意操纵。此外，该框架还支持在离散提示中嵌入木马，从而提高触发器攻击的整体有效性和精确度。具体来说，我们提出了一种触发器发现算法，通过使用少量数据样本查询受害人基于 LLM 的 API，为各种输入生成通用触发器。此外，我们引入了一种新颖的渐进式木马中毒算法，旨在生成中毒提示，该提示在各种模型中保持有效性和可转移性。我们的实验和结果证明了 TrojLLM 能够有效地将木马插入现实世界黑盒 LLM API（包括 GPT-3.5 和 GPT-4）的文本提示中，同时在干净的测试集上保持卓越的性能。我们的工作揭示了当前模型中的潜在安全风险，并提供了一种潜在的防御方法。 TrojLLM 的源代码可在 https://github.com/UCF-ML-Research/TrojLLM 获取。

## Likelihood-Based Diffusion Language Models<sup>poster<sup>

Authors: Ishaan Gulrajani, Tatsunori Hashimoto

Link: [https://neurips.cc/virtual/2023/poster/70985](https://neurips.cc/virtual/2023/poster/70985)

Abstract:

 Despite a growing interest in diffusion-based language models, existing work has not shown that these models can attain nontrivial likelihoods on standard language modeling benchmarks. In this work, we take the first steps towards closing the likelihood gap between autoregressive and diffusion-based language models, with the goal of building and releasing a diffusion model which outperforms a small but widely-known autoregressive model. We pursue this goal through algorithmic improvements, scaling laws, and increased compute. On the algorithmic front, we introduce several methodological improvements for the maximum-likelihood training of diffusion language models. We then study scaling laws for our diffusion models and find compute-optimal training regimes which differ substantially from autoregressive models. Using our methods and scaling analysis, we train and release Plaid 1B, a large diffusion language model which outperforms GPT-2 124M in likelihood on benchmark datasets and generates fluent samples in unconditional and zero-shot control settings.

摘要:

尽管人们对基于扩散的语言模型越来越感兴趣，但现有的工作尚未表明这些模型可以在标准语言建模基准上获得非平凡的可能性。在这项工作中，我们迈出了缩小自回归和基于扩散的语言模型之间的可能性差距的第一步，目标是构建和发布一个优于小型但广为人知的自回归模型的扩散模型。我们通过算法改进、缩放法则和增加计算来实现这一目标。在算法方面，我们介绍了扩散语言模型最大似然训练的几种方法改进。然后，我们研究扩散模型的缩放定律，并找到与自回归模型有很大不同的计算最佳训练方案。使用我们的方法和尺度分析，我们训练并发布了 Plaid 1B，这是一种大型扩散语言模型，它在基准数据集上的可能性优于 GPT-2 124M，并在无条件和零样本控制设置中生成流畅的样本。

## Scaling Data-Constrained Language Models<sup>oral<sup>

Authors: Niklas Muennighoff, Alexander Rush, Boaz Barak, Teven Le Scao, Nouamane Tazi, Aleksandra Piktus, Sampo Pyysalo, Thomas Wolf, Colin Raffel

Link: [https://neurips.cc/virtual/2023/poster/70706](https://neurips.cc/virtual/2023/poster/70706)

Abstract:

 The current trend of scaling language models involves increasing both parameter count and training dataset size. Extrapolating this trend suggests that training dataset size may soon be limited by the amount of text data available on the internet. Motivated by this limit, we investigate scaling language models in data-constrained regimes. Specifically, we run a large set of experiments varying the extent of data repetition and compute budget, ranging up to 900 billion training tokens and 9 billion parameter models. We find that with constrained data for a fixed compute budget, training with up to 4 epochs of repeated data yields negligible changes to loss compared to having unique data. However, with more repetition, the value of adding compute eventually decays to zero. We propose and empirically validate a scaling law for compute optimality that accounts for the decreasing value of repeated tokens and excess parameters. Finally, we experiment with approaches mitigating data scarcity, including augmenting the training dataset with code data or removing commonly used filters. Models and datasets from our 400 training runs are freely available at https://github.com/huggingface/datablations.

摘要:

当前缩放语言模型的趋势涉及增加参数数量和训练数据集大小。推断这一趋势表明，训练数据集的大小可能很快就会受到互联网上可用文本数据量的限制。受此限制的启发，我们研究了数据受限情况下的扩展语言模型。具体来说，我们运行了大量不同数据重复程度和计算预算的实验，范围高达 9000 亿个训练令牌和 90 亿个参数模型。我们发现，在固定计算预算的约束数据下，与拥有唯一数据相比，使用最多 4 个周期的重复数据进行训练所产生的损失变化可以忽略不计。然而，随着重复次数的增加，增加计算的价值最终会衰减到零。我们提出并凭经验验证了计算最优性的缩放法则，该法则解释了重复标记和多余参数的值递减的情况。最后，我们尝试了缓解数据稀缺的方法，包括使用代码数据增强训练数据集或删除常用的过滤器。我们 400 次训练运行的模型和数据集可在 https://github.com/huggingface/datablations 上免费获取。

## Zero-shot Visual Relation Detection via Composite Visual Cues from Large Language Models<sup>poster<sup>

Authors: Lin Li, Jun Xiao, Guikun Chen, Jian Shao, Yueting Zhuang, Long Chen

Link: [https://neurips.cc/virtual/2023/poster/70046](https://neurips.cc/virtual/2023/poster/70046)

Abstract:

 Pretrained vision-language models, such as CLIP, have demonstrated strong generalization capabilities, making them promising tools in the realm of zero-shot visual recognition. Visual relation detection (VRD) is a typical task that identifies relationship (or interaction) types between object pairs within an image. However, naively utilizing CLIP with prevalent class-based prompts for zero-shot VRD has several weaknesses, e.g., it struggles to distinguish between different fine-grained relation types and it neglects essential spatial information of two objects. To this end, we propose a novel method for zero-shot VRD: RECODE, which solves RElation detection via COmposite DEscription prompts. Specifically, RECODE first decomposes each predicate category into subject, object, and spatial components. Then, it leverages large language models (LLMs) to generate description-based prompts (or visual cues) for each component. Different visual cues enhance the discriminability of similar relation categories from different perspectives, which significantly boosts performance in VRD. To dynamically fuse different cues, we further introduce a chain-of-thought method that prompts LLMs to generate reasonable weights for different visual cues. Extensive experiments on four VRD benchmarks have demonstrated the effectiveness and interpretability of RECODE.

摘要:

预训练的视觉语言模型，例如 CLIP，已经表现出强大的泛化能力，使其成为零样本视觉识别领域的有前途的工具。视觉关系检测（VRD）是识别图像中对象对之间的关系（或交互）类型的典型任务。然而，天真地将 CLIP 与流行的基于类的提示一起用于零样本 VRD 有几个弱点，例如，它很难区分不同的细粒度关系类型，并且忽略了两个对象的基本空间信息。为此，我们提出了一种零样本 VRD 的新方法：RECODE，它通过 COmposite DEscription 提示解决 RElation 检测。具体来说，RECODE 首先将每个谓词类别分解为主语、宾语和空间分量。然后，它利用大型语言模型 (LLM) 为每个组件生成基于描述的提示（或视觉提示）。不同的视觉线索增强了从不同角度对相似关系类别的辨别能力，这显着提高了 VRD 的性能。为了动态融合不同的线索，我们进一步引入了一种思想链方法，提示法学硕士为不同的视觉线索生成合理的权重。对四个 VRD 基准的大量实验证明了 RECODE 的有效性和可解释性。

## In-Context Impersonation Reveals Large Language Models' Strengths and Biases<sup>poster<sup>

Authors: Leonard Salewski, Stephan Alaniz, Isabel Rio-Torto, Eric Schulz, Zeynep Akata

Link: [https://neurips.cc/virtual/2023/poster/72422](https://neurips.cc/virtual/2023/poster/72422)

Abstract:

 In everyday conversations, humans can take on different roles and adapt their vocabulary to their chosen roles. We explore whether LLMs can take on, that is impersonate, different roles when they generate text in-context. We ask LLMs to assume different personas before solving vision and language tasks. We do this by prefixing the prompt with a persona that is associated either with a social identity or domain expertise. In a multi-armed bandit task, we find that LLMs pretending to be children of different ages recover human-like developmental stages of exploration. In a language-based reasoning task, we find that LLMs impersonating domain experts perform better than LLMs impersonating non-domain experts. Finally, we test whether LLMs' impersonations are complementary to visual information when describing different categories. We find that impersonation can improve performance: an LLM prompted to be a bird expert describes birds better than one prompted to be a car expert. However, impersonation can also uncover LLMs' biases: an LLM prompted to be a man describes cars better than one prompted to be a woman. These findings demonstrate that LLMs are capable of taking on diverse roles and that this in-context impersonation can be used to uncover their strengths and hidden biases. Our code is available at https://github.com/ExplainableML/in-context-impersonation.

摘要:

在日常对话中，人类可以扮演不同的角色，并根据自己选择的角色调整词汇。我们探讨法学硕士在上下文中生成文本时是否可以扮演（即模拟）不同的角色。我们要求法学硕士在解决视觉和语言任务之前假设不同的角色。我们通过在提示前添加与社交身份或领域专业知识相关的角色来实现此目的。在多臂老虎机任务中，我们发现假装成不同年龄儿童的法学硕士恢复了类似人类的探索发展阶段。在基于语言的推理任务中，我们发现冒充领域专家的法学硕士比冒充非领域专家的法学硕士表现更好。最后，我们测试法学硕士在描述不同类别时的模仿是否与视觉信息互补。我们发现模仿可以提高表现：被提示成为鸟类专家的法学硕士比被提示成为汽车专家的法学硕士更能描述鸟类。然而，冒充也可以揭露法学硕士的偏见：被提示为男性的法学硕士比被提示为女性的法学硕士更能描述汽车。这些发现表明，法学硕士有能力扮演不同的角色，并且这种在上下文中的模仿可以用来揭示他们的优势和隐藏的偏见。我们的代码可在 https://github.com/ExplainableML/in-context-impersonation 获取。

## Towards Efficient Pre-Trained Language Model via Feature Correlation Distillation<sup>poster<sup>

Authors: Kun Huang, Xin Guo, Meng Wang

Link: [https://neurips.cc/virtual/2023/poster/70640](https://neurips.cc/virtual/2023/poster/70640)

Abstract:

 Knowledge Distillation (KD) has emerged as a promising approach for compressing large Pre-trained Language Models (PLMs). The performance of KD relies on how to effectively formulate and transfer the knowledge from the teacher model to the student model. Prior arts mainly focus on directly aligning output features from the transformer block, which may impose overly strict constraints on the student model's learning process and complicate the training process by introducing extra parameters and computational cost. Moreover, our analysis indicates that the different relations within self-attention, as adopted in other works, involves more computation complexities and can easily be constrained by the number of heads, potentially leading to suboptimal solutions.  To address these issues, we propose a novel approach that builds relationships directly from output features. Specifically, we introduce token-level and sequence-level relations concurrently  to fully exploit the knowledge from the teacher model. Furthermore, we propose a correlation-based distillation loss to alleviate the exact match properties inherent in traditional KL divergence or MSE loss functions. Our method, dubbed FCD, presents a simple yet effective method to compress various architectures (BERT, RoBERTa, and GPT) and model sizes (base-size and large-size).  Extensive experimental results demonstrate that our distilled, smaller language models significantly surpass existing KD methods across various NLP tasks.

摘要:

知识蒸馏（KD）已成为压缩大型预训练语言模型（PLM）的一种有前途的方法。 KD的性能取决于如何有效地制定知识并将其从教师模型迁移到学生模型。现有技术主要集中于直接对齐来自变压器块的输出特征，这可能对学生模型的学习过程施加过于严格的约束，并且通过引入额外的参数和计算成本而使训练过程复杂化。此外，我们的分析表明，自注意力中的不同关系（如其他作品中所采用的那样）涉及更多的计算复杂性，并且很容易受到头数量的限制，可能导致次优解决方案。为了解决这些问题，我们提出了一种直接从输出特征建立关系的新方法。具体来说，我们同时引入令牌级和序列级关系，以充分利用教师模型中的知识。此外，我们提出了一种基于相关性的蒸馏损失，以减轻传统 KL 散度或 MSE 损失函数固有的精确匹配特性。我们的方法称为 FCD，提供了一种简单而有效的方法来压缩各种架构（BERT、RoBERTa 和 GPT）和模型大小（基本大小和大大小）。大量的实验结果表明，我们经过提炼的较小语言模型在各种 NLP 任务中显着超越了现有的 KD 方法。

## Connecting Pre-trained Language Model and Downstream Task via Properties of Representation<sup>poster<sup>

Authors: Chenwei Wu, Holden Lee, Rong Ge

Link: [https://neurips.cc/virtual/2023/poster/71303](https://neurips.cc/virtual/2023/poster/71303)

Abstract:

 Recently, researchers have found that representations learned by large-scale pre-trained language models are useful in various downstream tasks. However, there is little theoretical understanding of how pre-training performance is related to downstream task performance. In this paper, we analyze how this performance transfer depends on the properties of the downstream task and the structure of the representations. We consider a log-linear model where a word can be predicted from its context through a network having softmax as its last layer. We show that even if the downstream task is highly structured and depends on a simple function of the hidden representation, there are still cases when a low pre-training loss cannot guarantee good performance on the downstream task. On the other hand, we propose and empirically validate the existence of an ``anchor vector'' in the representation space, and show that this assumption, together with properties of the downstream task,  guarantees performance transfer.

摘要:

最近，研究人员发现，大规模预训练语言模型学习到的表示在各种下游任务中非常有用。然而，对于预训练性能与下游任务性能之间的关系，理论理解很少。在本文中，我们分析了这种性能转移如何取决于下游任务的属性和表示的结构。我们考虑一个对数线性模型，其中可以通过以 softmax 作为最后一层的网络从上下文中预测单词。我们表明，即使下游任务是高度结构化的并且依赖于隐藏表示的简单函数，仍然存在低预训练损失不能保证下游任务良好性能的情况。另一方面，我们提出并凭经验验证了表示空间中“锚向量”的存在，并表明该假设与下游任务的属性一起保证了性能转移。

## Exposing Attention Glitches with Flip-Flop Language Modeling<sup>poster<sup>

Authors: Bingbin Liu, Jordan Ash, Surbhi Goel, Akshay Krishnamurthy, Cyril Zhang

Link: [https://neurips.cc/virtual/2023/poster/71426](https://neurips.cc/virtual/2023/poster/71426)

Abstract:

 Why do large language models sometimes output factual inaccuracies and exhibit erroneous reasoning? The brittleness of these models, particularly when executing long chains of reasoning, currently seems to be an inevitable price to pay for their advanced capabilities of coherently synthesizing knowledge, pragmatics, and abstract thought. Towards making sense of this fundamentally unsolved problem, this work identifies and analyzes the phenomenon of attention glitches, in which the Transformer architecture's inductive biases intermittently fail to capture robust reasoning. To isolate the issue, we introduce flip-flop language modeling (FFLM), a parametric family of synthetic benchmarks designed to probe the extrapolative behavior of neural language models. This simple generative task requires a model to copy binary symbols over long-range dependencies, ignoring the tokens in between. We find that Transformer FFLMs suffer from a long tail of sporadic reasoning errors, some of which we can eliminate using various regularization techniques. Our preliminary mechanistic analyses show why the remaining errors may be very difficult to diagnose and resolve. We hypothesize that attention glitches account for (some of) the closed-domain hallucinations in natural LLMs.

摘要:

为什么大型语言模型有时会输出不准确的事实并表现出错误的推理？这些模型的脆弱性，特别是在执行长链推理时，目前似乎是为其连贯地综合知识、语用学和抽象思维的先进能力付出的不可避免的代价。为了理解这个根本上未解决的问题，这项工作识别并分析了注意力故障现象，其中 Transformer 架构的归纳偏差间歇性地无法捕获稳健的推理。为了隔离这个问题，我们引入了触发器语言模型（FFLM），这是一个参数化的综合基准系列，旨在探测神经语言模型的外推行为。这个简单的生成任务需要一个模型来复制远程依赖关系上的二进制符号，忽略之间的标记。我们发现 Transformer FFLM 存在长尾的零星推理错误，其中一些错误我们可以使用各种正则化技术来消除。我们的初步机制分析表明了为什么剩余的错误可能很难诊断和解决。我们假设注意力缺陷是自然法学硕士中（部分）封闭域幻觉的原因。

## WalkLM: A Uniform Language Model Fine-tuning Framework for Attributed Graph Embedding<sup>poster<sup>

Authors: Yanchao Tan, Zihao Zhou, Hang Lv, Weiming Liu, Carl Yang

Link: [https://neurips.cc/virtual/2023/poster/71216](https://neurips.cc/virtual/2023/poster/71216)

Abstract:

 Graphs are widely used to model interconnected entities and improve downstream predictions in various real-world applications. However, real-world graphs nowadays are often associated with complex attributes on multiple types of nodes and even links that are hard to model uniformly, while the widely used graph neural networks (GNNs) often require sufficient training toward specific downstream predictions to achieve strong performance. In this work, we take a fundamentally different approach than GNNs, to simultaneously achieve deep joint modeling of complex attributes and flexible structures of real-world graphs and obtain unsupervised generic graph representations that are not limited to specific downstream predictions. Our framework, built on a natural integration of language models (LMs) and random walks (RWs), is straightforward, powerful and data-efficient. Specifically, we first perform attributed RWs on the graph and design an automated program to compose roughly meaningful textual sequences directly from the attributed RWs; then we fine-tune an LM using the RW-based textual sequences and extract embedding vectors from the LM, which encapsulates both attribute semantics and graph structures. In our experiments, we evaluate the learned node embeddings towards different downstream prediction tasks on multiple real-world attributed graph datasets and observe significant improvements over a comprehensive set of state-of-the-art unsupervised node embedding methods. We believe this work opens a door for more sophisticated technical designs and empirical evaluations toward the leverage of LMs for the modeling of real-world graphs.

摘要:

图被广泛用于对互连实体进行建模并改进各种现实应用中的下游预测。然而，当今现实世界的图通常与多种类型的节点甚至链接上的复杂属性相关联，难以统一建模，而广泛使用的图神经网络（GNN）通常需要针对特定下游预测进行充分的训练才能获得强大的性能。在这项工作中，我们采用了与 GNN 根本不同的方法，同时实现现实世界图的复杂属性和灵活结构的深度联合建模，并获得不限于特定下游预测的无监督通用图表示。我们的框架建立在语言模型 (LM) 和随机游走 (RW) 的自然集成之上，简单、强大且数据高效。具体来说，我们首先在图上执行归因 RW，并设计一个自动化程序，直接从归因 RW 组成大致有意义的文本序列；然后我们使用基于 RW 的文本序列对 LM 进行微调，并从 LM 中提取嵌入向量，其中封装了属性语义和图结构。在我们的实验中，我们评估了多个真实世界属性图数据集上不同下游预测任务的学习节点嵌入，并观察到相对于一组最先进的无监督节点嵌入方法的显着改进。我们相信这项工作为更复杂的技术设计和实证评估打开了一扇大门，以利用语言模型对现实世界的图形进行建模。

## Principle-Driven Self-Alignment of Language Models from Scratch with Minimal Human Supervision<sup>poster<sup>

Authors: Zhiqing Sun, Yikang Shen, Qinhong Zhou, Hongxin Zhang, Zhenfang Chen, David Cox, Yiming Yang, Chuang Gan

Link: [https://neurips.cc/virtual/2023/poster/70433](https://neurips.cc/virtual/2023/poster/70433)

Abstract:

 Recent AI-assistant agents, such as ChatGPT, predominantly rely on supervised fine-tuning (SFT) with human annotations and reinforcement learning from human feedback (RLHF) to align the output of large language models (LLMs) with human intentions, ensuring they are helpful, ethical, and reliable. However, this dependence can significantly constrain the true potential of AI-assistant agents due to the high cost of obtaining human supervision and the related issues on quality, reliability, diversity, self-consistency, and undesirable biases. To address these challenges, we propose a novel approach called SELF-ALIGN, which combines principle-driven reasoning and the generative power of LLMs for the self-alignment of AI agents with minimal human supervision. Our approach encompasses four stages: first, we use an LLM to generate synthetic prompts, and a topic-guided method to augment the prompt diversity; second, we use a small set of human-written principles for AI models to follow, and guide the LLM through in-context learning from demonstrations (of principles application) to produce helpful, ethical, and reliable responses to user's queries; third, we fine-tune the original LLM with the high-quality self-aligned responses so that the resulting model can generate desirable responses for each query directly without the principle set and the demonstrations anymore; and finally, we offer a refinement step to address the issues of overly-brief or indirect responses. Applying SELF-ALIGN to the LLaMA-65b base language model, we develop an AI assistant named Dromedary. With fewer than 300 lines of human annotations (including < 200 seed prompts, 16 generic principles, and 5 exemplars for in-context learning). Dromedary significantly surpasses the performance of several state-of-the-art AI systems, including Text-Davinci-003 and Alpaca, on benchmark datasets with various settings.

摘要:

最近的人工智能助理代理，例如 ChatGPT，主要依靠带有人类注释的监督微调（SFT）和来自人类反馈的强化学习（RLHF）来使大语言模型（LLM）的输出与人类意图保持一致，确保他们乐于助人、有道德、可靠。然而，由于获得人类监督的成本高昂以及质量、可靠性、多样性、自我一致性和不良偏差等相关问题，这种依赖性可能会严重限制人工智能助理代理的真正潜力。为了应对这些挑战，我们提出了一种名为“自调整”的新方法，该方法结合了原则驱动的推理和法学硕士的生成能力，可以在最少的人类监督下实现人工智能代理的自调整。我们的方法包括四个阶段：首先，我们使用法学硕士生成合成提示，并使用主题引导方法来增强提示多样性；其次，我们使用一小组人类编写的人工智能模型遵循的原则，并指导法学硕士通过演示（原则应用）进行上下文学习，以对用户的查询产生有用的、道德的和可靠的响应；第三，我们用高质量的自对齐响应对原始LLM进行微调，以便生成的模型可以直接为每个查询生成理想的响应，而不再需要原理集和演示；最后，我们提供了一个改进步骤来解决过于简短或间接的回应问题。将SELF-ALIGN应用于LLaMA-65b基础语言模型，我们开发了一个名为Dromedary的AI助手。人工注释少于 300 行（包括 < 200 条种子提示、16 条通用原则和 5 个上下文学习示例）。 Dromedary 在各种设置的基准数据集上显着超越了几个最先进的人工智能系统的性能，包括 Text-Davinci-003 和 Alpaca。

## StyleTTS 2: Towards Human-Level Text-to-Speech through Style Diffusion and Adversarial Training with Large Speech Language Models<sup>poster<sup>

Authors: Yinghao Aaron Li, Cong Han, Vinay Raghavan, Gavin Mischler, Nima Mesgarani

Link: [https://neurips.cc/virtual/2023/poster/70566](https://neurips.cc/virtual/2023/poster/70566)

Abstract:

 In this paper, we present StyleTTS 2, a text-to-speech (TTS) model that leverages style diffusion and adversarial training with large speech language models (SLMs) to achieve human-level TTS synthesis. StyleTTS 2 differs from its predecessor by modeling styles as a latent random variable through diffusion models to generate the most suitable style for the text without requiring reference speech, achieving efficient latent diffusion while benefiting from the diverse speech synthesis offered by diffusion models. Furthermore, we employ large pre-trained SLMs, such as WavLM, as discriminators with our novel differentiable duration modeling for end-to-end training, resulting in improved speech naturalness. StyleTTS 2 surpasses human recordings on the single-speaker LJSpeech dataset and matches it on the multispeaker VCTK dataset as judged by native English speakers. Moreover, when trained on the LibriTTS dataset, our model outperforms previous publicly available models for zero-shot speaker adaptation. This work achieves the first human-level TTS on both single and multispeaker datasets, showcasing the potential of style diffusion and adversarial training with large SLMs. The audio demos and source code are available at https://styletts2.github.io/.

摘要:

在本文中，我们提出了 StyleTTS 2，这是一种文本转语音 (TTS) 模型，它利用大型语音语言模型 (SLM) 的风格扩散和对抗性训练来实现人类水平的 TTS 合成。 StyleTTS 2 与其前身不同，通过扩散模型将风格建模为潜在随机变量，无需参考语音即可生成最适合文本的风格，实现高效的潜在扩散，同时受益于扩散模型提供的多样化语音合成。此外，我们采用大型预训练 SLM（例如 WavLM）作为判别器，并采用新颖的可微持续时间模型进行端到端训练，从而提高语音自然度。根据以英语为母语的人的判断，StyleTTS 2 在单说话人 LJSpeech 数据集上超越了人类录音，并在多说话人 VCTK 数据集上匹配。此外，当在 LibriTTS 数据集上进行训练时，我们的模型在零样本说话人适应方面优于之前公开可用的模型。这项工作在单说话人和多说话人数据集上实现了第一个人类水平的 TTS，展示了风格扩散和大型 SLM 对抗训练的潜力。音频演示和源代码可在 https://styletts2.github.io/ 获取。

## 3D-LLM: Injecting the 3D World into Large Language Models<sup>poster<sup>

Authors: Yining Hong, Haoyu Zhen, Peihao Chen, Shuhong Zheng, Yilun Du, Zhenfang Chen, Chuang Gan

Link: [https://neurips.cc/virtual/2023/poster/71298](https://neurips.cc/virtual/2023/poster/71298)

Abstract:

 Large language models (LLMs) and Vision-Language Models (VLMs) have been proved to excel at multiple tasks, such as commonsense reasoning. Powerful as these models can be, they are not grounded in the 3D physical world, which involves richer concepts such as spatial relationships, affordances, physics, layout, and so on. In this work, we propose to inject the 3D world into large language models, and introduce a whole new family of 3D-LLMs. Specifically, 3D-LLMs can take 3D point clouds and their features as input and perform a diverse set of 3D-related tasks, including captioning, dense captioning, 3D question answering, task decomposition, 3Dgrounding, 3D-assisted dialog, navigation, and so on. Using three types of prompting mechanisms that we design, we are able to collect over 300k 3D-language data covering these tasks. To efficiently train 3D-LLMs, we first utilize a 3D feature extractor that obtains 3D features from rendered multi-view images. Then, we use 2D VLMs as our backbones to train our 3D-LLMs. By introducing a 3D localization mechanism, 3D-LLMs could better capture 3D spatial information.  Experiments on ScanQA  show that our model outperforms state-of-the-art baselines by a large margin (\textit{e.g.}, the BLEU-1 score surpasses state-of-the-art score by 9\%). Furthermore, experiments on our held-in datasets for 3D captioning, task composition, and 3D-assisted dialogue show that our model outperforms 2D VLMs. Qualitative examples also show that our model could perform more tasks beyond the scope of existing LLMs and VLMs. Our model and data will be publicly available.

摘要:

大型语言模型（LLM）和视觉语言模型（VLM）已被证明在多种任务上表现出色，例如常识推理。尽管这些模型非常强大，但它们并不以 3D 物理世界为基础，而 3D 物理世界涉及更丰富的概念，例如空间关系、可供性、物理、布局等。在这项工作中，我们建议将 3D 世界注入大型语言模型中，并引入全新的 3D-LLM 系列。具体来说，3D-LLM 可以将 3D 点云及其特征作为输入，并执行各种 3D 相关任务，包括字幕、密集字幕、3D 问答、任务分解、3D 基础、3D 辅助对话、导航等在。使用我们设计的三种类型的提示机制，我们能够收集超过 30 万个涵盖这些任务的 3D 语言数据。为了有效地训练 3D-LLM，我们首先利用 3D 特征提取器从渲染的多视图图像中获取 3D 特征。然后，我们使用 2D VLM 作为骨干来训练 3D-LLM。通过引入 3D 定位机制，3D-LLM 可以更好地捕获 3D 空间信息。 ScanQA 上的实验表明，我们的模型大幅优于最先进的基线（\textit{eg}，BLEU-1 分数超过最先进的分数 9\%）。此外，对我们保留的 3D 字幕、任务组合和 3D 辅助对话数据集进行的实验表明，我们的模型优于 2D VLM。定性示例还表明，我们的模型可以执行超出现有 LLM 和 VLM 范围的更多任务。我们的模型和数据将公开。

## Large Language Models can Implement Policy Iteration<sup>poster<sup>

Authors: Ethan Brooks, Logan Walls, Richard L Lewis, Satinder Singh

Link: [https://neurips.cc/virtual/2023/poster/71955](https://neurips.cc/virtual/2023/poster/71955)

Abstract:

 In this work, we demonstrate a method for implementing policy iteration using a large language model. While the application of foundation models to RL has received considerable attention, most approaches rely on either (1) the curation of expert demonstrations (either through manual design or task-specific pretraining) or (2) adaptation to the task of interest using gradient methods (either fine-tuning or training of adapter layers). Both of these techniques have drawbacks. Collecting demonstrations is labor-intensive, and algorithms that rely on them do not outperform the experts from which the demonstrations were derived. All gradient techniques are inherently slow, sacrificing the “few-shot” quality that makes in-context learning attractive to begin with. Our method demonstrates that a large language model can be used to implement policy iteration using the machinery of in-context learning, enabling it to learn to perform RL tasks without expert demonstrations or gradients. Our approach iteratively updates the contents of the prompt from which it derives its policy through trial-and-error interaction with an RL environment. In order to eliminate the role of in-weights learning (on which approaches like Decision Transformer rely heavily), we demonstrate our method using Codex (M. Chen et al. 2021b), a language model with no prior knowledge of the domains on which we evaluate it.

摘要:

在这项工作中，我们演示了一种使用大型语言模型实现策略迭代的方法。虽然基础模型在强化学习中的应用受到了相当多的关注，但大多数方法依赖于（1）专家演示的策划（通过手动设计或特定于任务的预训练）或（2）使用梯度方法适应感兴趣的任务（适配器层的微调或训练）。这两种技术都有缺点。收集演示是一项劳动密集型工作，依赖于这些演示的算法的性能并不比得出演示的专家更好。所有梯度技术本质上都很慢，牺牲了“少样本”的质量，而这使得上下文学习一开始就很有吸引力。我们的方法表明，大型语言模型可用于使用上下文学习机制来实现策略迭代，使其能够学习执行强化学习任务，而无需专家演示或梯度。我们的方法通过与 RL 环境的试错交互来迭代更新提示的内容，并从中导出策略。为了消除权重学习的作用（像 Decision Transformer 这样的方法严重依赖于权重学习），我们使用 Codex（M. Chen 等人，2021b）演示了我们的方法，这是一种语言模型，没有先验知识的领域我们对其进行评估。

## Chameleon: Plug-and-Play Compositional Reasoning with Large Language Models<sup>poster<sup>

Authors: Pan Lu, Baolin Peng, Hao Cheng, Michel Galley, Kai-Wei Chang, Ying Nian Wu, Song-Chun Zhu, Jianfeng Gao

Link: [https://neurips.cc/virtual/2023/poster/72147](https://neurips.cc/virtual/2023/poster/72147)

Abstract:

 Large language models (LLMs) have achieved remarkable progress in solving various natural language processing tasks due to emergent reasoning abilities. However, LLMs have inherent limitations as they are incapable of accessing up-to-date information (stored on the Web or in task-specific knowledge bases), using external tools, and performing precise mathematical and logical reasoning. In this paper, we present Chameleon, an AI system that mitigates these limitations by augmenting LLMs with plug-and-play modules for compositional reasoning. Chameleon synthesizes programs by composing various tools (e.g., LLMs, off-the-shelf vision models, web search engines, Python functions, and heuristic-based modules) for accomplishing complex reasoning tasks. At the heart of Chameleon is an LLM-based planner that assembles a sequence of tools to execute to generate the final response. We showcase the effectiveness of Chameleon on two multi-modal knowledge-intensive reasoning tasks: ScienceQA and TabMWP. Chameleon, powered by GPT-4, achieves an 86.54% overall accuracy on ScienceQA, improving the best published few-shot result by 11.37%. On TabMWP, GPT-4-powered Chameleon improves the accuracy by 17.0%, lifting the state of the art to 98.78%. Our analysis also shows that the GPT-4-powered planner exhibits more consistent and rational tool selection via inferring potential constraints from instructions, compared to a ChatGPT-powered planner.

摘要:

由于新兴的推理能力，大语言模型（LLM）在解决各种自然语言处理任务方面取得了显着的进步。然而，法学硕士有其固有的局限性，因为它们无法访问最新信息（存储在网络上或特定任务的知识库中）、使用外部工具以及执行精确的数学和逻辑推理。在本文中，我们提出了 Chameleon，这是一种人工智能系统，它通过使用用于组合推理的即插即用模块来增强法学硕士，从而缓解这些限制。 Chameleon 通过组合各种工具（例如，LLM、现成的视觉模型、网络搜索引擎、Python 函数和基于启发式的模块）来综合程序，以完成复杂的推理任务。 Chameleon 的核心是一个基于 LLM 的规划器，它组装了一系列工具来执行以生成最终响应。我们展示了 Chameleon 在两个多模态知识密集型推理任务上的有效性：ScienceQA 和 TabMWP。 Chameleon 由 GPT-4 提供支持，在 ScienceQA 上实现了 86.54% 的整体准确率，将最佳已发表的少数结果提高了 11.37%。在 TabMWP 上，由 GPT-4 驱动的 Chameleon 将准确率提高了 17.0%，将最先进的准确率提升至 98.78%。我们的分析还表明，与 ChatGPT 支持的规划器相比，GPT-4 支持的规划器通过从指令推断潜在约束来表现出更加一致和合理的工具选择。

## Direct Preference Optimization: Your Language Model is Secretly a Reward Model<sup>oral<sup>

Authors: Rafael Rafailov, Archit Sharma, Eric Mitchell, Christopher D Manning, Stefano Ermon, Chelsea Finn

Link: [https://neurips.cc/virtual/2023/poster/72164](https://neurips.cc/virtual/2023/poster/72164)

Abstract:

 While large-scale unsupervised language models (LMs) learn broad world knowledge and some reasoning skills, achieving precise control of their behavior is difficult due to the completely unsupervised nature of their training. Existing methods for gaining such steerability collect human labels of the relative quality of model generations and fine-tune the unsupervised LM to align with these preferences, often with reinforcement learning from human feedback (RLHF). However, RLHF is a complex and often unstable procedure, first fitting a reward model that reflects the human preferences, and then fine-tuning the large unsupervised LM using reinforcement learning to maximize this estimated reward without drifting too far from the original model. In this paper, we leverage a mapping between reward functions and optimal policies to show that this constrained reward maximization problem can be optimized exactly with a single stage of policy training, essentially solving a classification problem on the human preference data. The resulting algorithm, which we call Direct Preference Optimization (DPO), is stable, performant, and computationally lightweight, eliminating the need for fitting a reward model, sampling from the LM during fine-tuning, or performing significant hyperparameter tuning. Our experiments show that DPO can fine-tune LMs to align with human preferences as well as or better than existing methods. Notably, fine-tuning with DPO exceeds RLHF's ability to control sentiment of generations and improves response quality in summarization and single-turn dialogue while being substantially simpler to implement and train.

摘要:

虽然大规模无监督语言模型（LM）学习广泛的世界知识和一些推理技能，但由于其训练的完全无监督性质，实现对其行为的精确控制很困难。获得这种可操纵性的现有方法收集模型生成相对质量的人类标签，并微调无监督的 LM 以符合这些偏好，通常通过人类反馈（RLHF）进行强化学习。然而，RLHF 是一个复杂且通常不稳定的过程，首先拟合反映人类偏好的奖励模型，然后使用强化学习对大型无监督 LM 进行微调，以最大化估计的奖励，而不会偏离原始模型太远。在本文中，我们利用奖励函数和最优策略之间的映射来表明，这种约束奖励最大化问题可以通过单阶段的策略训练来精确优化，本质上解决了人类偏好数据的分类问题。由此产生的算法，我们称之为直接偏好优化 (DPO)，稳定、高性能且计算量轻，无需拟合奖励模型、在微调期间从 LM 采样或执行重要的超参数调整。我们的实验表明，DPO 可以微调 LM 以符合人类偏好，并且比现有方法更好。值得注意的是，使用 DPO 进行微调超出了 RLHF 控制各代情绪的能力，并提高了摘要和单轮对话中的响应质量，同时大大简化了实施和训练。

## Tree of Thoughts: Deliberate Problem Solving with Large Language Models<sup>oral<sup>

Authors: Shunyu Yao, Dian Yu, Jeffrey Zhao, Izhak Shafran, Tom Griffiths, Yuan Cao, Karthik Narasimhan

Link: [https://neurips.cc/virtual/2023/poster/72797](https://neurips.cc/virtual/2023/poster/72797)

Abstract:

 Language models are increasingly being deployed for general problem solving across a wide range of tasks, but are still confined to token-level, left-to-right decision-making processes during inference. This means they can fall short in tasks that require exploration, strategic lookahead, or where initial decisions play a pivotal role. To surmount these challenges, we introduce a new framework for language model inference, Tree of Thoughts (ToT), which generalizes over the popular Chain of Thought approach to prompting language models, and enables exploration over coherent units of text (thoughts) that serve as intermediate steps toward problem solving. ToT allows LMs to perform deliberate decision making by considering multiple different reasoning paths and self-evaluating choices to decide the next course of action, as well as looking ahead or backtracking when necessary to make global choices.Our experiments show that ToT significantly enhances language models’ problem-solving abilities on three novel tasks requiring non-trivial planning or search: Game of 24, Creative Writing, and Mini Crosswords. For instance, in Game of 24, while GPT-4 with chain-of-thought prompting only solved 4\% of tasks, our method achieved a success rate of 74\%. Code repo with all prompts: https://github.com/princeton-nlp/tree-of-thought-llm.

摘要:

语言模型越来越多地被部署用于解决各种任务中的一般问题，但在推理过程中仍然仅限于标记级、从左到右的决策过程。这意味着他们可能无法完成需要探索、战略前瞻性或初始决策发挥关键作用的任务。为了克服这些挑战，我们引入了一种新的语言模型推理框架——思想树（ToT），它概括了流行的思想链方法来提示语言模型，并能够探索作为文本（思想）的连贯单元。解决问题的中间步骤。 ToT 允许 LM 进行深思熟虑的决策，通过考虑多种不同的推理路径和自我评估选择来决定下一步的行动，以及在必要时向前看或回溯以做出全局选择。我们的实验表明，ToT 显着增强了语言模型” 解决三项需要不平凡的计划或搜索的新颖任务的问题的能力：24 人游戏、创意写作和迷你填字游戏。例如，在 Game of 24 中，虽然带有思维链提示的 GPT-4 仅解决了 4% 的任务，但我们的方法取得了 74% 的成功率。包含所有提示的代码存储库：https://github.com/princeton-nlp/tree-of-thought-llm。

## H2O: Heavy-Hitter Oracle for Efficient Generative Inference of Large Language Models<sup>poster<sup>

Authors: Zhenyu Zhang, Ying Sheng, Tianyi Zhou, Tianlong Chen, Lianmin Zheng, Ruisi Cai, Zhao Song, Yuandong Tian, Christopher Ré, Clark Barrett, Zhangyang "Atlas" Wang, Beidi Chen

Link: [https://neurips.cc/virtual/2023/poster/71645](https://neurips.cc/virtual/2023/poster/71645)

Abstract:

 Large Language Models (LLMs), despite their recent impressive accomplishments, are notably cost-prohibitive to deploy, particularly for applications involving long-content generation, such as dialogue systems and story writing. Often, a large amount of transient state information, referred to as the $\mathsf{KV}$ $\mathsf{cache}$, is stored in GPU memory in addition to model parameters, scaling linearly with the sequence length and batch size. In this paper, we introduce a novel approach for implementing the  $\mathsf{KV}$ $\mathsf{cache}$ which significantly reduces its memory footprint.  Our approach is based on the noteworthy observation that a small portion of tokens contributes most of the value when computing attention scores.  We call these tokens Heavy Hitters ($\mathsf{H_2}$). Through a comprehensive investigation, we find that ($i$) the emergence of $\mathsf{H_2}$ is natural and strongly correlates with the frequent co-occurrence of tokens in the text, and ($ii$) removing them results in significant performance degradation. Based on these insights, we propose Heavy Hitter Oracle ($\mathsf{H_2O}$), a $\mathsf{KV}$ $\mathsf{cache}$ eviction policy that dynamically retains a balance of recent and $\mathsf{H_2}$ tokens. We formulate the $\mathsf{KV}$ $\mathsf{cache}$ eviction as a dynamic submodular problem and prove (under mild assumptions) a theoretical guarantee for our novel eviction algorithm which could help guide future work. We validate the accuracy of our algorithm with OPT, LLaMA, and GPT-NeoX across a wide range of tasks. Our implementation of $\mathsf{H_2O}$ with 20\% heavy hitters improves the throughput over three leading inference systems DeepSpeed Zero-Inference, Hugging Face Accelerate, and FlexGen by up to $29\times$, $29\times$, and $3\times$ on OPT-6.7B and OPT-30B. With the same batch size, $\mathsf{H_2O}$ can reduce the latency by up to $1.9\times$.

摘要:

大型语言模型（LLM）尽管最近取得了令人印象深刻的成就，但其部署成本明显过高，特别是对于涉及长内容生成的应用程序，例如对话系统和故事写作。通常，除了模型参数之外，大量瞬态信息（称为 $\mathsf{KV}$ $\mathsf{cache}$）也存储在 GPU 内存中，并随序列长度和批量大小线性缩放。在本文中，我们介绍了一种实现 $\mathsf{KV}$ $\mathsf{cache}$ 的新颖方法，该方法显着减少了其内存占用。我们的方法基于值得注意的观察，即在计算注意力分数时，一小部分令牌贡献了大部分价值。我们称这些代币为重击者 ($\mathsf{H_2}$)。通过全面的调查，我们发现($i$)$\mathsf{H_2}$的出现是自然的，并且与文本中标记的频繁共现有很强的相关性，而($ii$)删除它们会导致性能显着下降。基于这些见解，我们提出了 Heavy Hitter Oracle ($\mathsf{H_2O}$)，这是一个 $\mathsf{KV}$ $\mathsf{cache}$ 驱逐策略，动态地保持最近和 $\mathsf{H_2 的平衡}$ 代币。我们将 $\mathsf{KV}$ $\mathsf{cache}$ 驱逐制定为动态子模问题，并证明（在温和的假设下）我们新颖的驱逐算法的理论保证，这有助于指导未来的工作。我们使用 OPT、LLaMA 和 GPT-NeoX 在各种任务中验证了算法的准确性。我们采用 20% 重量级的 $\mathsf{H_2O}$ 实现，与三个领先的推理系统 DeepSpeed Zero-Inference、Hugging Face Accelerate 和 FlexGen 相比，吞吐量提高了高达 $29\times$、$29\times$ 和 $3 OPT-6.7B 和 OPT-30B 上的 \times$。在相同批量大小的情况下，$\mathsf{H_2O}$ 最多可以将延迟降低 $1.9\times$。

## PlanBench: An Extensible Benchmark for Evaluating Large Language Models on Planning and Reasoning about Change<sup>poster<sup>

Authors: Karthik Valmeekam, Matthew Marquez, Alberto Olmo, Sarath Sreedharan, Subbarao Kambhampati

Link: [https://neurips.cc/virtual/2023/poster/73553](https://neurips.cc/virtual/2023/poster/73553)

Abstract:

 Generating plans of action, and reasoning about change have long been considered a core competence of intelligent agents. It is thus no surprise that evaluating the planning and reasoning capabilities of large language models (LLMs) has become a hot topic of research. Most claims about LLM planning capabilities are however based on common sense tasks–where it becomes hard to tell whether LLMs are planning or merely retrieving from their vast world knowledge.  There is a strong need for systematic and extensible planning benchmarks with sufficient diversity to evaluate whether LLMs have innate planning capabilities. Motivated by this, we propose PlanBench, an extensible benchmark suite based on the kinds of domains used in the automated planning community, especially in the International Planning Competition, to test the capabilities of LLMs in planning or reasoning about actions and change. PlanBench provides sufficient diversity in both the task domains and the specific planning capabilities. Our studies also show that on many critical capabilities–including plan generation–LLM performance falls quite short, even with the SOTA models. PlanBench can thus function as a useful marker of progress of LLMs in planning and reasoning.

摘要:

生成行动计划和推理变化长期以来一直被认为是智能代理的核心能力。因此，评估大型语言模型（LLM）的规划和推理能力已成为研究热点也就不足为奇了。然而，大多数关于法学硕士规划能力的说法都是基于常识性任务——很难判断法学硕士是在规划还是只是从他们广泛的世界知识中检索。强烈需要系统的、可扩展的、具有足够多样性的规划基准来评估法学硕士是否具有先天的规划能力。受此启发，我们提出了 PlanBench，这是一个可扩展的基准套件，基于自动化规划社区（尤其是国际规划竞赛）中使用的领域类型，用于测试法学硕士在规划或推理行动和变更方面的能力。 PlanBench 在任务领域和特定规划功能方面都提供了足够的多样性。我们的研究还表明，即使使用 SOTA 模型，LLM 的许多关键功能（包括计划生成）的性能也相当不足。因此，PlanBench 可以作为法学硕士在规划和推理方面的进展的有用标记。

## Mass-Producing Failures of Multimodal Systems with Language Models<sup>poster<sup>

Authors: Shengbang Tong, Erik Jones, Jacob Steinhardt

Link: [https://neurips.cc/virtual/2023/poster/71572](https://neurips.cc/virtual/2023/poster/71572)

Abstract:

 Deployed multimodal models can fail in ways that evaluators did not anticipate. In order to find these failures before deployment, we introduce MultiMon, a system that automatically identifies systematic failures---generalizable, natural-language descriptions that describe categories of individual failures. To uncover systematic failures, MultiMon scrapes for examples of erroneous agreement: inputs that produce the same output, but should not. It then prompts a language model to identify common categories and describe them in natural language. We use MultiMon to find 14 systematic failures (e.g."ignores quantifiers'') of the CLIP text-encoder, each comprising hundreds of distinct inputs (e.g."a shelf with a few/many books''). Because CLIP is the backbone for most state-of-the-art multimodal models, these inputs produce failures in Midjourney 5.1, DALL-E, VideoFusion, and others. MultiMon can also steer towards failures relevant to specific use cases, such as self-driving cars. We see MultiMon as a step towards evaluation that autonomously explores the long-tail of potential system failures.

摘要:

部署的多模式模型可能会以评估者没有预料到的方式失败。为了在部署之前发现这些故障，我们引入了 MultiMon，这是一个自动识别系统故障的系统——描述单个故障类别的可概括的自然语言描述。为了发现系统性故障，MultiMon 搜集了错误协议的示例：输入产生相同的输出，但不应该产生相同的输出。然后，它提示语言模型识别常见类别并用自然语言描述它们。我们使用 MultiMon 找到了 CLIP 文本编码器的 14 个系统故障（例如“忽略量词”），每个故障都包含数百个不同的输入（例如“一个书架上有几本书/很多书”）。由于 CLIP 是大多数最先进的多模式模型的支柱，因此这些输入会在 Midjourney 5.1、DALL-E、VideoFusion 等中产生失败。 MultiMon 还可以引导与特定用例相关的故障，例如自动驾驶汽车。我们将 MultiMon 视为评估的一个步骤，可以自主探索潜在系统故障的长尾。

## FELM: Benchmarking Factuality Evaluation of Large Language Models<sup>poster<sup>

Authors: shiqi chen, Yiran Zhao, Jinghan Zhang, I-Chun Chern, Siyang Gao, Pengfei Liu, Junxian He

Link: [https://neurips.cc/virtual/2023/poster/73491](https://neurips.cc/virtual/2023/poster/73491)

Abstract:

 Assessing factuality of text generated by large language models (LLMs) is an emerging yet crucial research area, aimed at alerting users to potential errors and guiding the development of more reliable LLMs. Nonetheless, the evaluators assessing factuality necessitate suitable evaluation themselves to gauge progress and foster advancements. This direction remains under-explored, resulting in substantial impediments to the progress of factuality evaluators. To mitigate this issue, we introduce a benchmark for Factuality Evaluation of large Language Models, referred to as FELM. In this benchmark, we collect responses generated from LLMs and annotate factuality labels in a fine-grained manner. Contrary to previous studies that primarily concentrate on the factuality of world knowledge (e.g. information from Wikipedia), FELM focuses on factuality across diverse domains, spanning from world knowledge to math and reasoning. Our annotation is based on text segments, which can help pinpoint specific factual errors. The factuality annotations are further supplemented by predefined error types and reference links that either support or contradict the statement. In our experiments, we investigate the performance of several LLM-based factuality evaluators on FELM, including both vanilla LLMs and those augmented with retrieval mechanisms and chain-of-thought processes. Our findings reveal that while retrieval aids factuality evaluation, current LLMs are far from satisfactory to faithfully detect factual errors.

摘要:

评估大型语言模型（LLM）生成的文本的真实性是一个新兴但重要的研究领域，旨在提醒用户潜在的错误并指导更可靠的 LLM 的开发。尽管如此，评估事实性的评估者本身也需要进行适当的评估，以衡量进展并促进进步。这一方向仍未得到充分探索，这对事实评估者的进步造成了重大障碍。为了缓解这个问题，我们引入了大型语言模型事实性评估的基准，称为 FELM。在此基准测试中，我们收集法学硕士生成的回复，并以细粒度的方式注释事实标签。与之前主要关注世界知识的真实性（例如来自维基百科的信息）的研究相反，FELM 关注跨不同领域的真实性，涵盖从世界知识到数学和推理。我们的注释基于文本片段，这可以帮助查明特定的事实错误。事实性注释由预定义的错误类型和支持或反驳该陈述的参考链接进一步补充。在我们的实验中，我们研究了几个基于 LLM 的事实性评估器在 FELM 上的性能，包括普通的 LLM 和那些通过检索机制和思维过程增强的 LLM。我们的研究结果表明，虽然检索有助于事实评估，但目前的法学硕士在忠实地检测事实错误方面还远远不能令人满意。

## Knowledge-Augmented Reasoning Distillation for Small Language Models in Knowledge-Intensive Tasks<sup>poster<sup>

Authors: Minki Kang, Seanie Lee, Jinheon Baek, Kenji Kawaguchi, Sung Ju Hwang

Link: [https://neurips.cc/virtual/2023/poster/70015](https://neurips.cc/virtual/2023/poster/70015)

Abstract:

 Large Language Models (LLMs) have shown promising performance in knowledge-intensive reasoning tasks that require a compound understanding of knowledge. However, deployment of the LLMs in real-world applications can be challenging due to their high computational requirements and concerns on data privacy.Previous studies have focused on building task-specific small Language Models (LMs) by fine-tuning them with labeled data or distilling LLMs. However, these approaches are ill-suited for knowledge-intensive reasoning tasks due to the limited capacity of small LMs in memorizing the knowledge required.Motivated by our theoretical analysis on memorization, we propose Knowledge-Augmented Reasoning Distillation (KARD), a novel method that fine-tunes small LMs to generate rationales obtained from LLMs with augmented knowledge retrieved from an external knowledge base. Moreover, we further propose a neural reranker to obtain documents relevant to rationale generation. We empirically show that KARD significantly improves the performance of small T5 and GPT models on the challenging knowledge-intensive reasoning datasets, namely MedQA-USMLE, StrategyQA, and OpenbookQA.Notably, our method makes the 250M T5 models achieve superior performance against the fine-tuned 3B models, having 12 times larger parameters, on both MedQA-USMLE and StrategyQA benchmarks.

摘要:

大型语言模型（LLM）在需要对知识进行复合理解的知识密集型推理任务中表现出了良好的性能。然而，由于 LLM 的高计算要求和对数据隐私的担忧，在实际应用中部署 LLM 可能具有挑战性。之前的研究主要集中在通过使用标记数据或数据进行微调来构建特定于任务的小型语言模型 (LM)。蒸馏法学硕士。然而，由于小型 LM 记忆所需知识的能力有限，这些方法不适合知识密集型推理任务。在我们对记忆的理论分析的推动下，我们提出了知识增强推理蒸馏（KARD），这是一种新方法微调小型 LM，以生成从 LLM 获得的基本原理，并使用从外部知识库检索的增强知识。此外，我们进一步提出了一种神经重新排序器来获取与基本原理生成相关的文档。我们的经验表明，KARD 显着提高了小型 T5 和 GPT 模型在具有挑战性的知识密集型推理数据集（即 MedQA-USMLE、StrategyQA 和 OpenbookQA）上的性能。值得注意的是，我们的方法使 250M T5 模型在精细推理数据集上取得了优异的性能。在 MedQA-USMLE 和 StrategyQA 基准上调整了 3B 模型，参数增加了 12 倍。

## QuIP: 2-Bit Quantization of Large Language Models With Guarantees<sup>poster<sup>

Authors: Jerry Chee, Yaohui Cai, Volodymyr Kuleshov, Christopher De Sa

Link: [https://neurips.cc/virtual/2023/poster/69982](https://neurips.cc/virtual/2023/poster/69982)

Abstract:

 This work studies post-training parameter quantization in large language models (LLMs). We introduce quantization with incoherence processing (QuIP), a new method based on the insight that quantization benefits from incoherent weight and Hessian matrices, i.e., from the weights being even in magnitude and the directions in which it is important to round them accurately being unaligned with the coordinate axes. QuIP consists of two steps: (1) an adaptive rounding procedure minimizing a quadratic proxy objective; (2) efficient pre- and post-processing that ensures weight and Hessian incoherence via multiplication by random orthogonal matrices. We complement QuIP with the first theoretical analysis for an LLM-scale quantization algorithm, and show that our theory also applies to an existing method, OPTQ. Empirically, we find that our incoherence preprocessing improves several existing quantization algorithms and yields the first LLM quantization methods that produce viable results using only two bits per weight. Our code can be found at https://github.com/jerry-chee/QuIP.

摘要:

这项工作研究大型语言模型（LLM）中的训练后参数量化。我们引入了不相干处理量化（QuIP），这是一种新方法，它基于这样的见解：量化受益于不相干权重和 Hessian 矩阵，即权重的大小均匀，并且准确舍入它们的方向不对齐很重要与坐标轴。 QuIP 包含两个步骤：(1) 自适应舍入过程，最小化二次代理目标； (2) 高效的预处理和后处理，通过随机正交矩阵的乘法确保权重和 Hessian 不相干性。我们通过对 LLM 规模量化算法的首次理论分析来补充 QuIP，并表明我们的理论也适用于现有方法 OPTQ。根据经验，我们发现我们的不相干预处理改进了几种现有的量化算法，并产生了第一个 LLM 量化方法，该方法仅使用每个权重两位即可产生可行的结果。我们的代码可以在 https://github.com/jerry-chee/QuIP 找到。

## Testing the General Deductive Reasoning Capacity of Large Language Models Using OOD Examples<sup>poster<sup>

Authors: Abulhair Saparov, Richard Yuanzhe Pang, Vishakh Padmakumar, Nitish Joshi, Mehran Kazemi, Najoung Kim, He He

Link: [https://neurips.cc/virtual/2023/poster/71923](https://neurips.cc/virtual/2023/poster/71923)

Abstract:

 Given the intractably large size of the space of proofs, any model that is capable of general deductive reasoning must generalize to proofs of greater complexity. Recent studies have shown that large language models (LLMs) possess some abstract deductive reasoning ability given chain-of-thought prompts. However, they have primarily been tested on proofs using modus ponens or of a specific size, and from the same distribution as the in-context examples. To measure the general deductive reasoning ability of LLMs, we test on a broad set of deduction rules and measure their ability to generalize to more complex proofs from simpler demonstrations from multiple angles: depth-, width-, and compositional generalization. To facilitate systematic exploration, we construct a new synthetic and programmable reasoning dataset that enables control over deduction rules and proof complexity. Our experiments on four LLMs of various sizes and training objectives show that they are able to generalize to compositional proofs. However, they have difficulty generalizing to longer proofs, and they require explicit demonstrations to produce hypothetical subproofs, specifically in proof by cases and proof by contradiction.

摘要:

鉴于证明空间极其庞大，任何能够进行一般演绎推理的模型都必须推广到更复杂的证明。最近的研究表明，大型语言模型（LLM）在给定思维链提示的情况下具有一定的抽象演绎推理能力。然而，它们主要是在使用前件或特定大小的证明上进行测试的，并且来自与上下文示例相同的分布。为了衡量法学硕士的一般演绎推理能力，我们测试了一系列广泛的演绎规则，并衡量他们从多个角度（深度、宽度和组合概括）从更简单的演示推广到更复杂证明的能力。为了促进系统探索，我们构建了一个新的合成和可编程推理数据集，可以控制演绎规则和证明复杂性。我们对四个不同规模和培训目标的法学硕士进行的实验表明，它们能够推广到组合证明。然而，它们很难推广到更长的证明，并且需要明确的论证来产生假设的子证明，特别是在案例证明和矛盾证明中。

## Large Language Models Are Latent Variable Models: Explaining and Finding Good Demonstrations for In-Context Learning<sup>poster<sup>

Authors: Xinyi Wang, Wanrong Zhu, Michael Saxon, Mark Steyvers, William Yang Wang

Link: [https://neurips.cc/virtual/2023/poster/72494](https://neurips.cc/virtual/2023/poster/72494)

Abstract:

 In recent years, pre-trained large language models (LLMs) have demonstrated remarkable efficiency in achieving an inference-time few-shot learning capability known as in-context learning. However, existing literature has highlighted the sensitivity of this capability to the selection of few-shot demonstrations. Current understandings of the underlying mechanisms by which this capability arises from regular language model pretraining objectives remain disconnected from the real-world LLMs. This study aims to examine the in-context learning phenomenon through a Bayesian lens, viewing real-world LLMs as latent variable models. On this premise, we propose an algorithm to select optimal demonstrations from a set of annotated data with a small LM, and then directly generalize the selected demonstrations to larger LMs. We demonstrate significant improvement over baselines, averaged over eight GPT models on eight real-world text classification datasets. We also demonstrate the real-world usefulness of our algorithm on GSM8K, a math word problem dataset. Our empirical findings support our hypothesis that LLMs implicitly infer a latent variable containing task information.

摘要:

近年来，预训练的大型语言模型（LLM）在实现推理时间小样本学习能力（即上下文学习）方面表现出了显着的效率。然而，现有文献强调了这种能力对小样本演示选择的敏感性。目前对常规语言模型预训练目标产生这种能力的底层机制的理解仍然与现实世界的法学硕士脱节。本研究旨在通过贝叶斯透镜检验情境学习现象，将现实世界的法学硕士视为潜在变量模型。在此前提下，我们提出了一种算法，使用小型 LM 从一组带注释的数据中选择最佳演示，然后直接将所选演示推广到更大的 LM。我们展示了相对于基线的显着改进，在八个真实文本分类数据集上对八个 GPT 模型进行平均。我们还展示了我们的算法在数学应用题数据集 GSM8K 上的现实实用性。我们的实证研究结果支持我们的假设，即法学硕士隐式推断出包含任务信息的潜在变量。

## Understanding Social Reasoning in Language Models with Language Models<sup>poster<sup>

Authors: Kanishk Gandhi, Jan-Philipp Franken, Tobias Gerstenberg, Noah Goodman

Link: [https://neurips.cc/virtual/2023/poster/73680](https://neurips.cc/virtual/2023/poster/73680)

Abstract:

 As Large Language Models (LLMs) become increasingly integrated into our everyday lives, understanding their ability to comprehend human mental states becomes critical for ensuring effective interactions. However, despite the recent attempts to assess the Theory-of-Mind (ToM) reasoning capabilities of LLMs, the degree to which these models can align with human ToM remains a nuanced topic of exploration. This is primarily due to two distinct challenges: (1) the presence of inconsistent results from previous evaluations, and (2) concerns surrounding the validity of existing evaluation methodologies. To address these challenges, we present a novel framework for procedurally generating evaluations with LLMs by populating causal templates. Using our framework, we create a new social reasoning benchmark (BigToM) for LLMs which consists of 25 controls and 5,000 model-written evaluations. We find that human participants rate the quality of our benchmark higher than previous crowd-sourced evaluations and comparable to expert-written evaluations. Using BigToM, we evaluate the social reasoning capabilities of a variety of LLMs and compare model performances with human performance. Our results suggest that GPT4 has ToM capabilities that mirror human inference patterns, though less reliable, while other LLMs struggle.

摘要:

随着大型语言模型（LLM）越来越融入我们的日常生活，了解它们理解人类心理状态的能力对于确保有效的交互变得至关重要。然而，尽管最近尝试评估法学硕士的心智理论 (ToM) 推理能力，但这些模型与人类心智理论 (ToM) 的一致性程度仍然是一个微妙的探索话题。这主要是由于两个不同的挑战：（1）以前的评估结果不一致，（2）对现有评估方法有效性的担忧。为了应对这些挑战，我们提出了一个新颖的框架，通过填充因果模板来程序化地生成法学硕士的评估。使用我们的框架，我们为法学硕士创建了一个新的社会推理基准 (BigToM)，其中包含 25 个对照和 5,000 个模型编写的评估。我们发现，人类参与者对我们基准的质量评价高于以前的众包评估，并且与专家撰写的评估相当。使用 BigToM，我们评估了各种法学硕士的社会推理能力，并将模型表现与人类表现进行比较。我们的结果表明，GPT4 具有反映人类推理模式的 ToM 功能，尽管不太可靠，而其他法学硕士则苦苦挣扎。

## PIXIU: A Comprehensive Benchmark, Instruction Dataset and Large Language Model for Finance<sup>poster<sup>

Authors: Qianqian Xie, Weiguang Han, Xiao Zhang, Yanzhao Lai, Min Peng, Alejandro Lopez-Lira, Jimin Huang

Link: [https://neurips.cc/virtual/2023/poster/73431](https://neurips.cc/virtual/2023/poster/73431)

Abstract:

 Although large language models (LLMs) have shown great performance in natural language processing (NLP) in the financial domain, there are no publicly available financially tailored LLMs, instruction tuning datasets, and evaluation benchmarks, which is critical for continually pushing forward the open-source development of financial artificial intelligence (AI). This paper introduces PIXIU, a comprehensive framework including the first financial LLM based on fine-tuning LLaMA with instruction data, the first instruction data with 128K data samples to support the fine-tuning, and an evaluation benchmark with 8 tasks and 15 datasets. We first construct the large-scale multi-task instruction data considering a variety of financial tasks, financial document types, and financial data modalities. We then propose a financial LLM called FinMA by fine-tuning LLaMA with the constructed dataset to be able to follow instructions for various financial tasks. To support the evaluation of financial LLMs, we propose a standardized benchmark that covers a set of critical financial tasks, including six financial NLP tasks and two financial prediction tasks. With this benchmark, we conduct a detailed analysis of FinMA and several existing LLMs, uncovering their strengths and weaknesses in handling critical financial tasks. The model, datasets, benchmark, and experimental results are open-sourced to facilitate future research in financial AI.

摘要:

虽然大型语言模型（LLM）在金融领域的自然语言处理（NLP）方面表现出了出色的性能，但目前还没有公开的金融定制LLM、指令调优数据集和评估基准，这对于持续推动金融领域的LLM、指令调优数据集和评估基准至关重要。金融人工智能（AI）的开源开发。本文介绍了PIXIU，这是一个综合框架，包括第一个基于指令数据微调LLaMA的金融LLM、第一个具有128K数据样本支持微调的指令数据以及具有8个任务和15个数据集的评估基准。我们首先考虑各种财务任务、财务文档类型和财务数据模式来构建大规模多任务指令数据。然后，我们通过使用构建的数据集对 LLaMA 进行微调，提出了一种名为 FinMA 的金融法学硕士，以便能够遵循各种金融任务的说明。为了支持金融法学硕士的评估，我们提出了一个标准化基准，涵盖一组关键的金融任务，包括六个金融 NLP 任务和两个金融预测任务。借助这一基准，我们对 FinMA 和几位现有的法学硕士进行了详细分析，揭示了他们在处理关键财务任务方面的优势和劣势。该模型、数据集、基准和实验结果均开源，以促进金融人工智能的未来研究。

## Defending Pre-trained Language Models as Few-shot Learners against Backdoor Attacks<sup>poster<sup>

Authors: Zhaohan Xi, Tianyu Du, Changjiang Li, Ren Pang, Shouling Ji, Jinghui Chen, Fenglong Ma, Ting Wang

Link: [https://neurips.cc/virtual/2023/poster/72193](https://neurips.cc/virtual/2023/poster/72193)

Abstract:

 Pre-trained language models (PLMs) have demonstrated remarkable performance as few-shot learners. However, their security risks under such settings are largely unexplored. In this work, we conduct a pilot study showing that PLMs as few-shot learners are highly vulnerable to backdoor attacks while existing defenses are inadequate due to the unique challenges of few-shot scenarios. To address such challenges, we advocate MDP, a novel lightweight, pluggable, and effective defense for PLMs as few-shot learners. Specifically, MDP leverages the gap between the masking-sensitivity of poisoned and clean samples: with reference to the limited few-shot data as distributional anchors, it compares the representations of given samples under varying masking and identifies poisoned samples as ones with significant variations. We show analytically that MDP creates an interesting dilemma for the attacker to choose between attack effectiveness and detection evasiveness. The empirical evaluation using benchmark datasets and representative attacks validates the efficacy of MDP. The code of MDP is publicly available.

摘要:

预训练语言模型（PLM）在小样本学习器方面表现出了卓越的性能。然而，在这种设置下它们的安全风险很大程度上尚未被探索。在这项工作中，我们进行了一项试点研究，表明 PLM 作为少样本学习器非常容易受到后门攻击，而由于少样本场景的独特挑战，现有防御措施不足。为了应对这些挑战，我们提倡 MDP，这是一种新颖的轻量级、可插拔且有效的防御方法，用于将 PLM 作为小样本学习器。具体来说，MDP利用了中毒样本和干净样本的掩蔽敏感性之间的差距：参考有限的少样本数据作为分布锚，比较给定样本在不同掩蔽下的表示，并将中毒样本识别为具有显着变化的样本。我们分析表明，MDP 为攻击者在攻击有效性和检测规避性之间做出选择创造了一个有趣的困境。使用基准数据集和代表性攻击的实证评估验证了 MDP 的有效性。 MDP 的代码是公开的。

## How does GPT-2 compute greater-than?: Interpreting mathematical abilities in a pre-trained language model<sup>poster<sup>

Authors: Michael Hanna, Ollie Liu, Alexandre Variengien

Link: [https://neurips.cc/virtual/2023/poster/70432](https://neurips.cc/virtual/2023/poster/70432)

Abstract:

 Pre-trained language models can be surprisingly adept at tasks they were not explicitly trained on, but how they implement these capabilities is poorly understood. In this paper, we investigate the basic mathematical abilities often acquired by pre-trained language models. Concretely, we use mechanistic interpretability techniques to explain the (limited) mathematical abilities of GPT-2 small. As a case study, we examine its ability to take in sentences such as "The war lasted from the year 1732 to the year 17", and predict valid two-digit end years (years > 32). We first identify a circuit, a small subset of GPT-2 small's computational graph that computes this task's output. Then, we explain the role of each circuit component, showing that GPT-2 small's final multi-layer perceptrons boost the probability of end years greater than the start year. Finally, we find related tasks that activate our circuit. Our results suggest that GPT-2 small computes greater-than using a complex but general mechanism that activates across diverse contexts.

摘要:

预训练的语言模型可能出人意料地擅长执行它们未经过明确训练的任务，但人们对它们如何实现这些功能却知之甚少。在本文中，我们研究了预训练语言模型通常获得的基本数学能力。具体来说，我们使用机械可解释性技术来解释 GPT-2 小的（有限的）数学能力。作为一个案例研究，我们检查了它接受诸如“战争从 1732 年持续到第 17 年”之类的句子的能力，并预测有效的两位数结束年份（年份 > 32）。我们首先确定一个电路，它是 GPT-2 Small 计算图的一个小子集，用于计算该任务的输出。然后，我们解释了每个电路组件的作用，表明 GPT-2 Small 的最终多层感知器使结束年的概率大于开始年的概率。最后，我们找到激活我们电路的相关任务。我们的结果表明，GPT-2 小型计算量大于使用跨不同上下文激活的复杂但通用的机制。

## Language Models Meet World Models: Embodied Experiences Enhance Language Models<sup>poster<sup>

Authors: Jiannan Xiang, Tianhua Tao, Yi Gu, Tianmin Shu, Zirui Wang, Zichao Yang, Zhiting Hu

Link: [https://neurips.cc/virtual/2023/poster/71603](https://neurips.cc/virtual/2023/poster/71603)

Abstract:

 While large language models (LMs) have shown remarkable capabilities across numerous tasks, they often struggle with simple reasoning and planning in physical environments, such as understanding object permanence or planning household activities. The limitation arises from the fact that LMs are trained only on written text and miss essential embodied knowledge and skills. In this paper, we propose a new paradigm of enhancing LMs by finetuning them with world models, to gain diverse embodied knowledge while retaining their general language capabilities. Our approach deploys an embodied agent in a world model, particularly a simulator of the physical world (VirtualHome), and acquires a diverse set of embodied experiences through both goal-oriented planning and random exploration. These experiences are then used to finetune LMs to teach diverse abilities of reasoning and acting in the physical world, e.g., planning and completing goals, object permanence and tracking, etc. Moreover, it is desirable to preserve the generality of LMs during finetuning, which facilitates generalizing the embodied knowledge across tasks rather than being tied to specific simulations. We thus further introduce the classical elastic weight consolidation (EWC) for selective weight updates, combined with low-rank adapters (LoRA) for training efficiency. Extensive experiments show our approach substantially improves base LMs on 18 downstream tasks by 64.28% on average. In particular, the small LMs (1.3B, 6B, and 13B) enhanced by our approach match or even outperform much larger LMs (e.g., ChatGPT).

摘要:

虽然大型语言模型（LM）在众多任务中表现出了卓越的能力，但它们常常难以在物理环境中进行简单的推理和规划，例如理解物体的持久性或规划家庭活动。其局限性在于，LM 仅接受书面文本培训，而忽略了必要的具体知识和技能。在本文中，我们提出了一种通过世界模型对其进行微调来增强语言模型的新范式，以获得多样化的具体知识，同时保留其通用语言能力。我们的方法在世界模型中部署一个具体代理，特别是物理世界的模拟器（VirtualHome），并通过目标导向的规划和随机探索获得一组多样化的具体经验。然后，这些经验被用来微调 LM，以教授物理世界中的各种推理和行动能力，例如规划和完成目标、对象持久性和跟踪等。此外，在微调过程中最好保留 LM 的通用性，这有助于概括跨任务的具体知识，而不是与特定的模拟联系在一起。因此，我们进一步引入经典的弹性权重合并（EWC）来进行选择性权重更新，并结合低秩适配器（LoRA）来提高训练效率。大量实验表明，我们的方法将 18 个下游任务的基础 LM 平均显着提高了 64.28%。特别是，通过我们的方法增强的小型 LM（1.3B、6B 和 13B）可以匹配甚至优于更大的 LM（例如 ChatGPT）。

## Flocks of Stochastic Parrots: Differentially Private Prompt Learning for Large Language Models<sup>poster<sup>

Authors: Haonan Duan, Adam Dziedzic, Nicolas Papernot, Franziska Boenisch

Link: [https://neurips.cc/virtual/2023/poster/70167](https://neurips.cc/virtual/2023/poster/70167)

Abstract:

 Large language models (LLMs) are excellent in-context learners. However, the sensitivity of data contained in prompts raises privacy concerns. Our work first shows that these concerns are valid: we instantiate a simple but highly effective membership inference attack against the data used to prompt LLMs. To address this vulnerability, one could forego prompting and resort to fine-tuning LLMs with known algorithms for private gradient descent. However, this comes at the expense of the practicality and efficiency offered by prompting. Therefore, we propose to privately learn to prompt. We first show that soft prompts can be obtained privately through gradient descent on downstream data. However, this is not the case for discrete prompts. Thus, we orchestrate a noisy vote among an ensemble of LLMs presented with different prompts, i.e., a flock of stochastic parrots. The vote privately transfers the flock's knowledge into a single public prompt. We show that LLMs prompted with our private algorithms closely match the non-private baselines. For example, using GPT3 as the base model, we achieve a downstream accuracy of 92.7% on the sst2 dataset with $(\varepsilon=0.147, \delta=10^{-6})$-differential privacy vs. 95.2% for the non-private baseline. Through our experiments, we also show that our prompt-based approach is easily deployed with existing commercial~APIs.

摘要:

大型语言模型（LLM）是优秀的上下文学习器。然而，提示中包含的数据的敏感性引起了隐私问题。我们的工作首先表明这些担忧是有效的：我们针对用于提示法学硕士的数据实例化了一个简单但高效的成员推理攻击。为了解决这一漏洞，人们可以放弃提示，转而使用已知的私有梯度下降算法来微调 LLM。然而，这是以牺牲提示所提供的实用性和效率为代价的。所以，我们建议私下学习提示。我们首先证明可以通过下游数据的梯度下降来私下获得软提示。然而，离散提示的情况并非如此。因此，我们在一群提出不同提示的法学硕士（即一群随机鹦鹉）中精心策划了一场喧闹的投票。投票私下将群体的知识转化为单一的公共提示。我们表明，使用我们的私有算法提示的法学硕士与非私有基线非常匹配。例如，使用 GPT3 作为基础模型，我们在 sst2 数据集上使用 $(\varepsilon=0.147, \delta=10^{-6})$-差分隐私实现了 92.7% 的下游准确率，而在非私人基线。通过我们的实验，我们还表明我们基于提示的方法可以轻松地与现有的商业 API 一起部署。

## Large Language Models are Fixated by Red Herrings: Exploring Creative Problem Solving and Einstellung Effect using the Only Connect Wall Dataset<sup>poster<sup>

Authors: Saeid Alavi Naeini, Raeid Saqur, Mozhgan Saeidi, John Giorgi, Babak Taati

Link: [https://neurips.cc/virtual/2023/poster/73547](https://neurips.cc/virtual/2023/poster/73547)

Abstract:

 The quest for human imitative AI has been an enduring topic in AI research since inception. The technical evolution and emerging capabilities of the latest cohort of large language models (LLMs) have reinvigorated the subject beyond academia to cultural zeitgeist. While recent NLP evaluation benchmark tasks test some aspects of human-imitative behaviour (e.g., BIG-bench's `human-like behavior' tasks), few, if not none, examine creative problem solving abilities. Creative problem solving in humans is a well-studied topic in cognitive neuroscience with standardized tests that predominantly use ability to associate (heterogeneous) connections among clue words as a metric for creativity. Exposure to misleading stimuli --- distractors dubbed red herrings --- impede human performance in such tasks via the fixation effect and Einstellung paradigm. In cognitive neuroscience studies, such fixations are experimentally induced by pre-exposing participants to orthographically similar incorrect words to subsequent word-fragments or clues. The popular British quiz show Only Connect's Connecting Wall segment essentially mimics Mednick's Remote Associates Test (RAT) formulation with built-in, deliberate red herrings, that makes it an ideal proxy dataset to explore and study fixation effect and Einstellung paradigm from cognitive neuroscience in LLMs. In addition to presenting the novel Only Connect Wall (OCW) dataset, we also report results from our evaluation of selected pre-trained language models and LLMs (including OpenAI's GPT series) on creative problem solving tasks like grouping clue words by heterogeneous connections, and identifying correct open knowledge domain connections in respective groups. We synthetically generate two additional datasets: OCW-Randomized, OCW-WordNet to further analyze our red-herrings hypothesis in language models.The code and link to the dataset is available at url.

摘要:

自人工智能研究诞生以来，寻求模仿人类的人工智能一直是人工智能研究中经久不衰的话题。最新一批大型语言模型 (LLM) 的技术发展和新兴功能使这一学科从学术界走向文化时代精神。虽然最近的 NLP 评估基准任务测试了人类模仿行为的某些方面（例如，BIG-bench 的“类人行为”任务），但很少（如果不是没有的话）检查创造性解决问题的能力。人类的创造性问题解决是认知神经科学中一个经过充分研究的主题，其标准化测试主要使用关联线索词之间（异质）联系的能力作为创造力的衡量标准。暴露于误导性刺激（被称为转移注意力的干扰物）会通过固着效应和固定范式阻碍人类在此类任务中的表现。在认知神经科学研究中，这种固定是通过预先让参与者接触与后续单词片段或线索拼写相似的不正确单词来实验诱导的。英国流行的问答节目 Only Connect 的 Connecting Wall 部分本质上模仿了 Mednick 的远程关联测试 (RAT) 公式，并内置了故意的转移注意力的内容，这使其成为探索和研究法学硕士认知神经科学中的注视效应和 Einstellung 范式的理想代理数据集。除了展示新颖的 Only Connect Wall (OCW) 数据集外，我们还报告了对选定的预训练语言模型和 LLM（包括 OpenAI 的 GPT 系列）在创造性问题解决任务（例如通过异构连接对线索词进行分组）上的评估结果识别各个组中正确的开放知识域连接。我们综合生成了两个额外的数据集：OCW-Randomized、OCW-WordNet，以进一步分析语言模型中的转移注意力的假设。数据集的代码和链接可在 url 中找到。

## SwapPrompt: Test-Time Prompt Adaptation for Vision-Language Models<sup>poster<sup>

Authors: XIAOSONG MA, Jie ZHANG, Song Guo, Wenchao Xu

Link: [https://neurips.cc/virtual/2023/poster/72303](https://neurips.cc/virtual/2023/poster/72303)

Abstract:

 Test-time adaptation (TTA) is a special and practical setting in unsupervised domain adaptation, which allows a pre-trained model in a source domain to adapt to unlabeled test data in another target domain. To avoid the computation-intensive backbone fine-tuning process, the zero-shot generalization potentials of the emerging pre-trained vision-language models (e.g., CLIP, CoOp) are leveraged to only tune the run-time prompt for unseen test domains. However, existing solutions have yet to fully exploit the representation capabilities of pre-trained models as they only focus on the entropy-based optimization and the performance is far below the supervised prompt adaptation methods, e.g., CoOp. In this paper, we propose SwapPrompt, a novel framework that can effectively leverage the self-supervised contrastive learning to facilitate the test-time prompt adaptation. SwapPrompt employs a dual prompts paradigm, i.e., an online prompt and a target prompt that averaged from the online prompt to retain historical information. In addition, SwapPrompt applies a swapped prediction mechanism, which takes advantage of the representation capabilities of pre-trained models to enhance the online prompt via contrastive learning. Specifically, we use the online prompt together with an augmented view of the input image to predict the class assignment generated by the target prompt together with an alternative augmented view of the same image. The proposed SwapPrompt can be easily deployed on vision-language models without additional requirement, and experimental results show that it achieves state-of-the-art test-time adaptation performance on ImageNet and nine other datasets. It is also shown that SwapPrompt can even achieve comparable performance with supervised prompt adaptation methods.

摘要:

测试时间适应（TTA）是无监督域适应中的一种特殊且实用的设置，它允许源域中的预训练模型适应另一个目标域中的未标记测试数据。为了避免计算密集型主干微调过程，利用新兴预训练视觉语言模型（例如 CLIP、CoOp）的零样本泛化潜力，仅调整未见过的测试域的运行时提示。然而，现有的解决方案尚未充分利用预训练模型的表示能力，因为它们只关注基于熵的优化，并且性能远远低于有监督的即时适应方法，例如CoOp。在本文中，我们提出了 SwapPrompt，这是一种新颖的框架，可以有效地利用自监督对比学习来促进测试时提示的适应。 SwapPrompt采用双重提示范例，即在线提示和对在线提示进行平均以保留历史信息的目标提示。此外，SwapPrompt应用了交换预测机制，利用预训练模型的表示能力，通过对比学习来增强在线提示。具体来说，我们使用在线提示和输入图像的增强视图来预测目标提示和同一图像的替代增强视图生成的类分配。所提出的 SwapPrompt 可以轻松部署在视觉语言模型上，无需额外要求，实验结果表明，它在 ImageNet 和其他九个数据集上实现了最先进的测试时适应性能。它还表明，SwapPrompt 甚至可以达到与监督提示适应方法相当的性能。

## Fine-Grained Human Feedback Gives Better Rewards for Language Model Training<sup>poster<sup>

Authors: Zeqiu Wu, Yushi Hu, Weijia Shi, Nouha Dziri, Alane Suhr, Prithviraj (Raj) Ammanabrolu, Noah Smith, Mari Ostendorf, Hannaneh Hajishirzi

Link: [https://neurips.cc/virtual/2023/poster/72428](https://neurips.cc/virtual/2023/poster/72428)

Abstract:

 Language models (LMs) often exhibit undesirable text generation behaviors, including generating false, toxic, or irrelevant outputs. Reinforcement learning from human feedback (RLHF)---where human preference judgments on LM outputs are transformed into a learning signal---has recently shown promise in addressing these issues. However, such holistic feedback conveys limited information on long text outputs; it does not indicate which aspects of the outputs influenced user preference; e.g., which parts contain what type(s) of errors. In this paper, we use fine-grained human feedback (e.g., which sentence is false, which sub-sentence is irrelevant) as an explicit training signal. We introduce Fine-Grained RLHF, a framework that enables training and learning from reward functions that are fine-grained in two respects: (1) density, providing a reward after every segment (e.g., a sentence) is generated; and (2) incorporating multiple reward models associated with different feedback types (e.g., factual incorrectness, irrelevance, and information incompleteness). We conduct experiments on detoxification and long-form question answering to illustrate how learning with this reward function leads to improved performance, supported by both automatic and human evaluation. Additionally, we show that LM behaviors can be customized using different combinations of fine-grained reward models. We release all data, collected human feedback, and codes at https://FineGrainedRLHF.github.io.

摘要:

语言模型（LM）经常表现出不良的文本生成行为，包括生成错误的、有毒的或不相关的输出。来自人类反馈的强化学习（RLHF）——人类对 LM 输出的偏好判断被转化为学习信号——最近在解决这些问题方面显示出了希望。然而，这种整体反馈传达的长文本输出信息有限；它没有表明输出的哪些方面影响了用户的偏好；例如，哪些部分包含哪些类型的错误。在本文中，我们使用细粒度的人类反馈（例如，哪个句子是错误的，哪个子句子不相关）作为显式训练信号。我们引入了 Fine-Grained RLHF，这是一个框架，可以从两个方面细粒度的奖励函数中进行训练和学习：（1）密度，在生成每个片段（例如，一个句子）后提供奖励； (2) 合并与不同反馈类型（例如，事实不正确、不相关和信息不完整）相关的多种奖励模型。我们进行了排毒和长篇问答实验，以说明在自动和人工评估的支持下，利用这种奖励函数进行学习如何提高表现。此外，我们还表明可以使用细粒度奖励模型的不同组合来定制 LM 行为。我们在 https://FineGrainedRLHF.github.io 上发布了所有数据、收集的人类反馈和代码。

## SheetCopilot: Bringing Software Productivity to the Next Level through Large Language Models<sup>poster<sup>

Authors: Hongxin Li, Jingran Su, Yuntao Chen, Qing Li, ZHAO-XIANG ZHANG

Link: [https://neurips.cc/virtual/2023/poster/70193](https://neurips.cc/virtual/2023/poster/70193)

Abstract:

 Computer end users have spent billions of hours completing daily tasks like tabular data processing and project timeline scheduling. Most of these tasks are repetitive and error-prone, yet most end users lack the skill to automate these burdensome works. With the advent of large language models (LLMs), directing software with natural language user requests become a reachable goal. In this work, we propose a SheetCopilot agent that takes natural language task and control spreadsheet to fulfill the requirements. We propose a set of atomic actions as an abstraction of spreadsheet software functionalities. We further design a state machine-based task planning framework for LLMs to robustly interact with spreadsheets. We curate a representative dataset containing 221 spreadsheet control tasks and establish a fully automated evaluation pipeline for rigorously benchmarking the ability of LLMs in software control tasks. Our SheetCopilot correctly completes 44.3\% of tasks for a single generation, outperforming the strong code generation baseline by a wide margin. Our project page: https://sheetcopilot.github.io/.

摘要:

计算机最终用户花费了数十亿小时来完成表格数据处理和项目时间安排等日常任务。这些任务大多数都是重复性的且容易出错，但大多数最终用户缺乏自动化这些繁重工作的技能。随着大语言模型（LLM）的出现，用自然语言用户请求指导软件成为一个可以实现的目标。在这项工作中，我们提出了一个 SheetCopilot 代理，它接受自然语言任务和控制电子表格来满足要求。我们提出了一组原子操作作为电子表格软件功能的抽象。我们进一步为法学硕士设计了一个基于状态机的任务规划框架，以便与电子表格进行稳健的交互。我们整理了一个包含 221 个电子表格控制任务的代表性数据集，并建立了一个完全自动化的评估管道，以严格对法学硕士在软件控制任务中的能力进行基准测试。我们的 SheetCopilot 在单代中正确完成了 44.3% 的任务，远远超过了强大的代码生成基线。我们的项目页面：https://sheetcopilot.github.io/。

## Setting the Trap: Capturing and Defeating Backdoors in Pretrained Language Models through Honeypots<sup>poster<sup>

Authors: Ruixiang Tang, Jiayi Yuan, Yiming Li, Zirui Liu, Rui Chen, Xia Hu

Link: [https://neurips.cc/virtual/2023/poster/72945](https://neurips.cc/virtual/2023/poster/72945)

Abstract:

 In the field of natural language processing, the prevalent approach involves fine-tuning pretrained language models (PLMs) using local samples. Recent research has exposed the susceptibility of PLMs to backdoor attacks, wherein the adversaries can embed malicious prediction behaviors by manipulating a few training samples. In this study, our objective is to develop a backdoor-resistant tuning procedure that yields a backdoor-free model, no matter whether the fine-tuning dataset contains poisoned samples. To this end, we propose and integrate an \emph{honeypot module} into the original PLM, specifically designed to absorb backdoor information exclusively. Our design is motivated by the observation that lower-layer representations in PLMs carry sufficient backdoor features while carrying minimal information about the original tasks. Consequently, we can impose penalties on the information acquired by the honeypot module to inhibit backdoor creation during the fine-tuning process of the stem network. Comprehensive experiments conducted on benchmark datasets substantiate the effectiveness and robustness of our defensive strategy. Notably, these results indicate a substantial reduction in the attack success rate ranging from 10\% to 40\% when compared to prior state-of-the-art methods.

摘要:

在自然语言处理领域，普遍的方法是使用本地样本微调预训练语言模型（PLM）。最近的研究暴露了 PLM 容易受到后门攻击，其中攻击者可以通过操纵一些训练样本来嵌入恶意预测行为。在本研究中，我们的目标是开发一种抗后门的调整程序，无论微调数据集是否包含中毒样本，都可以生成无后门模型。为此，我们提出并将\emph{honeypot module}集成到原始PLM中，专门用于吸收后门信息。我们的设计动机是观察到 PLM 中的较低层表示具有足够的后门功能，同时携带有关原始任务的最少信息。因此，我们可以对蜜罐模块获取的信息进行惩罚，以抑制主干网络微调过程中后门的创建。在基准数据集上进行的综合实验证实了我们防御策略的有效性和稳健性。值得注意的是，这些结果表明，与之前最先进的方法相比，攻击成功率大幅降低了 10% 到 40%。

## Are Emergent Abilities of Large Language Models a Mirage?<sup>oral<sup>

Authors: Rylan Schaeffer, Brando Miranda, Sanmi Koyejo

Link: [https://neurips.cc/virtual/2023/poster/72117](https://neurips.cc/virtual/2023/poster/72117)

Abstract:

 Recent work claims that large language models display \textit{emergent abilities}, abilities not present in smaller-scale models that are present in larger-scale models.What makes emergent abilities intriguing is two-fold: their \textit{sharpness}, transitioning seemingly instantaneously from not present to present, and their \textit{unpredictability}, appearing at seemingly unforeseeable model scales.Here, we present an alternative explanation for emergent abilities: that for a particular task and model family, when analyzing fixed model outputs, emergent abilities appear due the researcher’s choice of metric rather than due to fundamental changes in model behavior with scale. Specifically, nonlinear or discontinuous metrics produce apparent emergent abilities, whereas linear or continuous metrics produce smooth, continuous, predictable changes in model performance.We present our alternative explanation in a simple mathematical model, then test it in three complementary ways: we (1) make, test and confirm three predictions on the effect of metric choice using the InstructGPT/GPT-3 family on tasks with claimed emergent abilities, (2) make, test and confirm two predictions about metric choices in a meta-analysis of emergent abilities on BIG-Bench; and (3) show how to choose metrics to produce never-before-seen seemingly emergent abilities in multiple vision tasks across diverse deep networks.Via all three analyses, we provide evidence that alleged emergent abilities evaporate with different metrics or with better statistics, and may not be a fundamental property of scaling AI models.

摘要:

最近的工作声称大型语言模型显示出 \textit{emergent 能力}，这种能力在较小规模的模型中不存在，但在较大规模的模型中却存在。使涌现能力有趣的原因有两个：它们的 \textit{sharpness} ，似乎瞬间从不存在过渡到存在，以及它们的 \textit{不可预测性}，以看似不可预见的模型规模出现。在这里，我们对涌现能力提出了另一种解释：对于特定任务和模型族，在分析固定模型输出时，涌现能力的出现是由于研究人员对度量的选择，而不是由于模型行为随规模的根本变化。具体来说，非线性或不连续指标会产生明显的涌现能力，而线性或连续指标会在模型性能中产生平滑、连续、可预测的变化。我们在一个简单的数学模型中提出我们的替代解释，然后以三种互补的方式对其进行测试：我们（1）使用 InstructGPT/GPT-3 系列对具有声称的新兴能力的任务做出、测试和确认关于度量选择影响的三个预测，(2) 在对新兴能力的荟萃分析中做出、测试和确认关于度量选择的两个预测大长凳； （3）展示如何选择指标来在不同深度网络的多个视觉任务中产生前所未见的看似突现的能力。通过所有三项分析，我们提供的证据表明，所谓的突现能力会随着不同的指标或更好的统计数据而消失，并且可能不是扩展人工智能模型的基本属性。

## On the Planning Abilities of Large Language Models - A Critical Investigation<sup>poster<sup>

Authors: Karthik Valmeekam, Matthew Marquez, Sarath Sreedharan, Subbarao Kambhampati

Link: [https://neurips.cc/virtual/2023/poster/71377](https://neurips.cc/virtual/2023/poster/71377)

Abstract:

 Intrigued by the claims of emergent reasoning capabilities in LLMs trained on general web corpora, in this paper, we set out to investigate their planning capabilities. We aim to evaluate (1) the effectiveness of LLMs in generating plans autonomously in commonsense planning tasks and (2) the potential of LLMs as a source of heuristic guidance for other agents (AI planners) in their planning tasks. We conduct a systematic study by generating a suite of instances on domains similar to the ones employed in the International Planning Competition and evaluate LLMs in two distinct modes: autonomous and heuristic. Our findings reveal that LLMs’ ability to generate executable plans autonomously is rather limited, with the best model (GPT-4) having an average success rate of ~12% across the domains. However, the results in the heuristic mode show more promise. In the heuristic mode, we demonstrate that LLM-generated plans can improve the search process for underlying sound planners and additionally show that external verifiers can help provide feedback on the generated plans and back-prompt the LLM for better plan generation.

摘要:

出于对在通用网络语料库上训练的法学硕士的紧急推理能力的说法的兴趣，在本文中，我们着手研究他们的规划能力。我们的目标是评估（1）LLM 在常识性规划任务中自主生成计划的有效性，以及（2）LLM 作为其他智能体（AI 规划者）在规划任务中启发式指导来源的潜力。我们通过在类似于国际规划竞赛中使用的领域生成一组实例来进行系统研究，并以两种不同的模式评估法学硕士：自主模式和启发式模式。我们的研究结果表明，法学硕士自主生成可执行计划的能力相当有限，最佳模型 (GPT-4) 在各个领域的平均成功率约为 12%。然而，启发式模式的结果显示出更多的希望。在启发式模式中，我们证明了 LLM 生成的计划可以改进底层合理规划器的搜索过程，并且还表明外部验证者可以帮助提供对生成的计划的反馈，并反向提示 LLM 以更好地生成计划。

## DDCoT: Duty-Distinct Chain-of-Thought Prompting for Multimodal Reasoning in Language Models<sup>poster<sup>

Authors: Ge Zheng, Bin Yang, Jiajin Tang, Hong-Yu Zhou, Sibei Yang

Link: [https://neurips.cc/virtual/2023/poster/70625](https://neurips.cc/virtual/2023/poster/70625)

Abstract:

 A long-standing goal of AI systems is to perform complex multimodal reasoning like humans. Recently, large language models (LLMs) have made remarkable strides in such multi-step reasoning on the language modality solely by leveraging the chain of thought (CoT) to mimic human thinking. However, the transfer of these advancements to multimodal contexts introduces heightened challenges, including but not limited to the impractical need for labor-intensive annotation and the limitations in terms of flexibility, generalizability, and explainability. To evoke CoT reasoning in multimodality, this work first conducts an in-depth analysis of these challenges posed by multimodality and presents two key insights: “keeping critical thinking” and “letting everyone do their jobs” in multimodal CoT reasoning. Furthermore, this study proposes a novel DDCoT prompting that maintains a critical attitude through negative-space prompting and incorporates multimodality into reasoning by first dividing the reasoning responsibility of LLMs into reasoning and recognition and then integrating the visual recognition capability of visual models into the joint reasoning process. The rationales generated by DDCoT not only improve the reasoning abilities of both large and small language models in zero-shot prompting and fine-tuning learning, significantly outperforming state-of-the-art methods but also exhibit impressive generalizability and explainability.

摘要:

人工智能系统的一个长期目标是像人类一样执行复杂的多模态推理。最近，大型语言模型（LLM）仅通过利用思维链（CoT）来模仿人类思维，就在语言模态的多步推理方面取得了显着的进步。然而，将这些进步转移到多模态环境中带来了更大的挑战，包括但不限于对劳动密集型注释的不切实际的需求以及灵活性、普遍性和可解释性方面的限制。为了唤起多模态中的 CoT 推理，这项工作首先对多模态带来的这些挑战进行了深入分析，并提出了两个关键见解：多模态 CoT 推理中的“保持批判性思维”和“让每个人各司其职”。此外，本研究提出了一种新颖的DDCoT提示，通过负空间提示保持批判态度，并将多模态融入推理，首先将法学硕士的推理责任划分为推理和识别，然后将视觉模型的视觉识别能力融入联合推理。过程。 DDCoT 生成的基本原理不仅提高了大小语言模型在零样本提示和微调学习中的推理能力，显着优于最先进的方法，而且还表现出令人印象深刻的概括性和可解释性。

## Thrust: Adaptively Propels Large Language Models with External Knowledge<sup>poster<sup>

Authors: Xinran Zhao, Hongming Zhang, Xiaoman Pan, Wenlin Yao, Dong Yu, Jianshu Chen

Link: [https://neurips.cc/virtual/2023/poster/70026](https://neurips.cc/virtual/2023/poster/70026)

Abstract:

 Although large-scale pre-trained language models (PTLMs) are shown to encode rich knowledge in their model parameters, the inherent knowledge in PTLMs can be opaque or static, making external knowledge necessary. However, the existing information retrieval techniques could be costly and may even introduce noisy and sometimes misleading knowledge. To address these challenges, we propose the instance-level adaptive propulsion of external knowledge (IAPEK), where we only conduct the retrieval when necessary. To achieve this goal, we propose to model whether a PTLM contains enough knowledge to solve an instance with a novel metric, Thrust, which leverages the representation distribution of a small amount of seen instances. Extensive experiments demonstrate that Thrust is a good measurement of models' instance-level knowledgeability. Moreover, we can achieve higher cost-efficiency with the Thrust score as the retrieval indicator than the naive usage of external knowledge on 88% of the evaluated tasks with 26% average performance improvement. Such findings shed light on the real-world practice of knowledge-enhanced LMs with a limited budget for knowledge seeking due to computation latency or costs.

摘要:

虽然大规模预训练语言模型（PTLM）被证明可以在其模型参数中编码丰富的知识，但 PTLM 中的固有知识可能是不透明的或静态的，使得外部知识变得必要。然而，现有的信息检索技术可能成本高昂，甚至可能引入嘈杂的、有时甚至是误导性的知识。为了应对这些挑战，我们提出了外部知识的实例级自适应推进（IAPEK），我们仅在必要时进行检索。为了实现这一目标，我们建议对 PTLM 是否包含足够的知识来使用新颖的度量 Thrust 来解决实例进行建模，该度量利用了少量已见实例的表示分布。大量实验表明，Thrust 可以很好地衡量模型的实例级知识能力。此外，在 88% 的评估任务上，以 Thrust 分数作为检索指标，我们可以实现比单纯使用外部知识更高的成本效率，平均性能提高 26%。这些发现揭示了知识增强型语言模型的现实世界实践，由于计算延迟或成本，知识搜索的预算有限。

## Language Models Don't Always Say What They Think: Unfaithful Explanations in Chain-of-Thought Prompting<sup>poster<sup>

Authors: Miles Turpin, Julian Michael, Ethan Perez, Samuel Bowman

Link: [https://neurips.cc/virtual/2023/poster/71118](https://neurips.cc/virtual/2023/poster/71118)

Abstract:

 Large Language Models (LLMs) can achieve strong performance on many tasks by producing step-by-step reasoning before giving a final output, often referred to as chain-of-thought reasoning (CoT). It is tempting to interpret these CoT explanations as the LLM's process for solving a task. This level of transparency into LLMs' predictions would yield significant safety benefits. However, we find that CoT explanations can systematically misrepresent the true reason for a model's prediction. We demonstrate that CoT explanations can be heavily influenced by adding biasing features to model inputs—e.g., by reordering the multiple-choice options in a few-shot prompt to make the answer always "(A)"—which models systematically fail to mention in their explanations. When we bias models toward incorrect answers, they frequently generate CoT explanations rationalizing those answers. This causes accuracy to drop by as much as 36% on a suite of 13 tasks from BIG-Bench Hard, when testing with GPT-3.5 from OpenAI and Claude 1.0 from Anthropic. On a social-bias task, model explanations justify giving answers in line with stereotypes without mentioning the influence of these social biases. Our findings indicate that CoT explanations can be plausible yet misleading, which risks increasing our trust in LLMs without guaranteeing their safety. Building more transparent and explainable systems will require either improving CoT faithfulness through targeted efforts or abandoning CoT in favor of alternative methods.

摘要:

大型语言模型（LLM）可以通过在给出最终输出之前进行逐步推理（通常称为思想链推理（CoT））来在许多任务上取得出色的性能。人们很容易将这些 CoT 解释解释为法学硕士解决任务的过程。法学硕士预测的这种透明度将带来显着的安全效益。然而，我们发现 CoT 解释可能会系统地歪曲模型预测的真实原因。我们证明，在模型输入中添加偏差特征会严重影响 CoT 解释——例如，通过在几次提示中重新排序多项选择选项，使答案始终为“(A)”——模型系统地在他们的解释。当我们将模型偏向于错误答案时，它们经常会生成 CoT 解释，使这些答案合理化。当使用 OpenAI 的 GPT-3.5 和 Anthropic 的 Claude 1.0 进行测试时，这会导致 BIG-Bench Hard 的一组 13 项任务的准确性下降多达 36%。在社会偏见任务中，模型解释证明给出符合刻板印象的答案是合理的，而没有提及这些社会偏见的影响。我们的研究结果表明，CoT 的解释可能看似合理，但却具有误导性，这可能会增加我们对法学硕士的信任，但无法保证其安全。建立更加透明和可解释的系统需要通过有针对性的努力来提高 CoT 的忠诚度，或者放弃 CoT 而转而采用替代方法。

## ZipLM: Inference-Aware Structured Pruning of Language Models<sup>poster<sup>

Authors: Eldar Kurtić, Elias Frantar, Dan Alistarh

Link: [https://neurips.cc/virtual/2023/poster/71044](https://neurips.cc/virtual/2023/poster/71044)

Abstract:

 The breakthrough performance of large language models (LLMs) comes with major computational footprints and high deployment costs. In this paper, we progress towards resolving this problem by proposing a novel structured compression approach for LLMs, called ZipLM. ZipLM achieves state-of-the-art accuracy-vs-speedup, while matching a set of desired target runtime speedups in any given inference environment. Specifically, given a model, a dataset, an inference environment, as well as a set of speedup targets, ZipLM iteratively identifies and removes components with the worst loss-runtime trade-off. Unlike prior methods that specialize in either the post-training/one-shot or the gradual compression setting, and only for specific families of models such as BERT (encoder) or GPT (decoder), ZipLM produces state-of-the-art compressed models across all these settings. Furthermore, ZipLM achieves superior results for a fraction of the computational cost relative to prior distillation and pruning techniques, making it a cost-effective approach for generating an entire family of smaller, faster, and highly accurate models, guaranteed to meet the desired inference specifications. In particular, ZipLM outperforms all prior BERT-base distillation and pruning techniques, such as CoFi, MiniLM, and TinyBERT. Moreover, it matches the performance of the heavily optimized MobileBERT model, obtained via extensive architecture search, by simply pruning the baseline BERT-large model. When compressing GPT2, ZipLM outperforms DistilGPT2 while being 60\% smaller and 30\% faster. Our code is available at: https://github.com/IST-DASLab/ZipLM.

摘要:

大型语言模型（LLM）的突破性性能伴随着大量的计算占用和高昂的部署成本。在本文中，我们通过提出一种新型的 LLM 结构化压缩方法（称为 ZipLM）来解决这个问题。 ZipLM 实现了最先进的精度与速度比，同时在任何给定的推理环境中匹配一组所需的目标运行时加速比。具体来说，给定一个模型、一个数据集、一个推理环境以及一组加速目标，ZipLM 会迭代地识别并删除损失与运行时间权衡最差的组件。与专注于后训练/一次性或渐进压缩设置并且仅针对特定模型系列（例如 BERT（编码器）或 GPT（解码器））的现有方法不同，ZipLM 生成最先进的压缩跨所有这些设置的模型。此外，与之前的蒸馏和剪枝技术相比，ZipLM 只需一小部分计算成本就能获得优异的结果，使其成为生成整个系列更小、更快且高精度模型的经济有效的方法，并保证满足所需的推理规范。特别是，ZipLM 优于所有现有的基于 BERT 的蒸馏和剪枝技术，例如 CoFi、MiniLM 和 TinyBERT。此外，它与经过广泛架构搜索而获得的高度优化的 MobileBERT 模型的性能相匹配，只需修剪基线 BERT-large 模型即可。压缩 GPT2 时，ZipLM 的性能优于 DistilGPT2，同时体积小 60%，速度快 30%。我们的代码位于：https://github.com/IST-DASLab/ZipLM。

## Inference-Time Intervention: Eliciting Truthful Answers from a Language Model<sup>poster<sup>

Authors: Kenneth Li, Oam Patel, Fernanda Viégas, Hanspeter Pfister, Martin Wattenberg

Link: [https://neurips.cc/virtual/2023/poster/71200](https://neurips.cc/virtual/2023/poster/71200)

Abstract:

 We introduce Inference-Time Intervention (ITI), a technique designed to enhance the "truthfulness" of large language models (LLMs). ITI operates by shifting model activations during inference, following a learned set of directions across a limited number of attention heads. This intervention significantly improves the performance of LLaMA models on the TruthfulQA benchmark. On an instruction-finetuned LLaMA called Alpaca, ITI improves its truthfulness from $32.5\%$ to $65.1\%$. We identify a tradeoff between truthfulness and helpfulness and demonstrate how to balance it by tuning the intervention strength. ITI is minimally invasive and computationally inexpensive. Moreover, the technique is data efficient: while approaches like RLHF require extensive annotations, ITI locates truthful directions using only few hundred examples. Our findings suggest that LLMs may have an internal representation of the likelihood of something being true, even as they produce falsehoods on the surface.

摘要:

我们介绍了推理时间干预（ITI），这是一种旨在增强大型语言模型（LLM）“真实性”的技术。 ITI 的运作方式是在推理过程中改变模型激活，遵循有限数量的注意力头学习到的一组方向。这种干预显着提高了 LLaMA 模型在 TruthfulQA 基准上的性能。在名为 Alpaca 的指令微调 LLaMA 上，ITI 将其真实性从 $32.5\%$ 提高到 $65.1\%$。我们确定了真实性和乐于助人之间的权衡，并演示了如何通过调整干预强度来平衡它。 ITI 是微创且计算成本低廉的。此外，该技术的数据效率很高：虽然 RLHF 等方法需要大量注释，但 ITI 仅使用数百个示例即可找到真实的方向。我们的研究结果表明，法学硕士可能对某些事情为真的可能性有一种内在的表征，即使他们在表面上产生了谎言。

## Language Models are Weak Learners<sup>poster<sup>

Authors: Hariharan Manikandan, Yiding Jiang, J. Zico Kolter

Link: [https://neurips.cc/virtual/2023/poster/72822](https://neurips.cc/virtual/2023/poster/72822)

Abstract:

 A central notion in practical and theoretical machine learning is that of a weak learner, classifiers that achieve better-than-random performance (on any given distribution over data), even by a small margin.  Such weak learners form the practical basis for canonical machine learning methods such as boosting.  In this work, we illustrate that prompt-based large language models can operate effectively as said weak learners.  Specifically, we illustrate the use of a large language model (LLM) as a weak learner in a boosting algorithm applied to tabular data.  We show that by providing (properly sampled according to the distribution of interest) text descriptions of tabular data samples, LLMs can produce a summary of the samples that serves as a template for classification, and achieves the aim of acting as a weak learner on this task.  We incorporate these models into a boosting approach, which in many settings can leverage the knowledge within the LLM to outperform traditional tree-based boosting.  The model outperforms both few-shot learning and occasionally even more involved fine-tuning procedures, particularly for some tasks involving small numbers of data points.  The results illustrate the potential for prompt-based LLMs to function not just as few-shot learners themselves, but as components of larger machine learning models.

摘要:

机器学习实践和理论中的一个核心概念是弱学习器，分类器能够实现优于随机的性能（在任何给定的数据分布上），即使是很小的差距。这种弱学习器构成了诸如 boosting 之类的规范机器学习方法的实践基础。在这项工作中，我们证明基于提示的大型语言模型可以像弱学习者一样有效地运行。具体来说，我们说明了如何使用大型语言模型（LLM）作为应用于表格数据的增强算法中的弱学习器。我们表明，通过提供（根据兴趣分布适当采样）表格数据样本的文本描述，法学硕士可以生成样本摘要，作为分类模板，并达到充当弱学习者的目的任务。我们将这些模型融入到一种提升方法中，在许多情况下，这种方法可以利用法学硕士中的知识来超越传统的基于树的提升。该模型的性能优于小样本学习，有时甚至更多地涉及微调过程，特别是对于涉及少量数据点的某些任务。结果表明，基于提示的法学硕士不仅可以作为小样本学习者本身，而且可以作为更大的机器学习模型的组成部分。

## ComSL: A Composite Speech-Language Model for End-to-End Speech-to-Text Translation<sup>poster<sup>

Authors: Chenyang Le, Yao Qian, Long Zhou, Shujie LIU, Yanmin Qian, Michael Zeng, Xuedong Huang

Link: [https://neurips.cc/virtual/2023/poster/72758](https://neurips.cc/virtual/2023/poster/72758)

Abstract:

 Joint speech-language training is challenging due to the large demand for training data and GPU consumption, as well as the modality gap between speech and language. We present ComSL, a speech-language model built atop a composite architecture of public pre-trained speech-only and language-only models and optimized data-efficiently for spoken language tasks. Particularly, we propose to incorporate cross-modality learning into transfer learning and conduct them simultaneously for downstream tasks in a multi-task learning manner. Our approach has demonstrated effectiveness in end-to-end speech-to-text translation tasks, achieving a new state-of-the-art average BLEU score of 31.5 on the multilingual speech to English text translation task for 21 languages, as measured on the public CoVoST2 evaluation set.

摘要:

由于对训练数据和 GPU 消耗的大量需求，以及语音和语言之间的模态差距，联合语音语言训练具有挑战性。我们提出了 ComSL，这是一种语音语言模型，构建在公共预训练纯语音和纯语言模型的复合架构之上，并针对口语任务高效地优化了数据。特别是，我们建议将跨模态学习纳入迁移学习中，并以多任务学习的方式对下游任务同时进行。我们的方法在端到端语音到文本翻译任务中展现了有效性，在 21 种语言的多语言语音到英语文本翻译任务中取得了 31.5 分的最新平均 BLEU 分数（根据以下指标衡量）公共 CoVoST2 评估集。

## Toolformer: Language Models Can Teach Themselves to Use Tools<sup>oral<sup>

Authors: Timo Schick, Jane Dwivedi-Yu, Roberto Dessi, Roberta Raileanu, Maria Lomeli, Eric Hambro, Luke Zettlemoyer, Nicola Cancedda, Thomas Scialom

Link: [https://neurips.cc/virtual/2023/poster/71288](https://neurips.cc/virtual/2023/poster/71288)

Abstract:

 Language models (LMs) exhibit remarkable abilities to solve new tasks from just a few examples or textual instructions, especially at scale. They also, paradoxically, struggle with basic functionality, such as arithmetic or factual lookup, where much simpler and smaller specialized models excel. In this paper, we show that LMs can teach themselves to use external tools via simple APIs and achieve the best of both worlds. We introduce Toolformer, a model trained to decide which APIs to call, when to call them, what arguments to pass, and how to best incorporate the results into future token prediction. This is done in a self-supervised way, requiring nothing more than a handful of demonstrations for each API. We incorporate a range of tools, including a calculator, a Q&A system, a search engine, a translation system, and a calendar. Toolformer achieves substantially improved zero-shot performance across a variety of downstream tasks, often competitive with much larger models, without sacrificing its core language modeling abilities.

摘要:

语言模型（LM）表现出非凡的能力，可以仅通过几个示例或文本指令来解决新任务，尤其是大规模任务。矛盾的是，它们还难以实现基本功能，例如算术或事实查找，而更简单和更小的专用模型在这些功能上表现出色。在本文中，我们展示了 LM 可以通过简单的 API 自学使用外部工具，并实现两全其美。我们引入了 Toolformer，这是一个经过训练的模型，用于决定调用哪些 API、何时调用它们、传递哪些参数以及如何最好地将结果合并到未来的令牌预测中。这是通过自我监督的方式完成的，只需要为每个 API 进行少量演示即可。我们整合了一系列工具，包括计算器、问答系统、搜索引擎、翻译系统和日历。 Toolformer 在各种下游任务中显着提高了零样本性能，通常可以与更大的模型竞争，而无需牺牲其核心语言建模能力。

## GraphAdapter: Tuning Vision-Language Models With Dual Knowledge Graph<sup>poster<sup>

Authors: Xin Li, Dongze Lian, Zhihe Lu, Jiawang Bai, Zhibo Chen, Xinchao Wang

Link: [https://neurips.cc/virtual/2023/poster/71275](https://neurips.cc/virtual/2023/poster/71275)

Abstract:

 Adapter-style efficient transfer learning (ETL) has shown excellent performance in the tuning of vision-language models (VLMs) under the low-data regime, where only a few additional parameters are introduced to excavate the task-specific knowledge based on the general and powerful representation of VLMs. However, most adapter-style works face two limitations: (i) modeling task-specific knowledge with a single modality only; and (ii) overlooking the exploitation of the inter-class relationships in downstream tasks, thereby leading to sub-optimal solutions. To mitigate that, we propose an effective adapter-style tuning strategy, dubbed GraphAdapter, which performs the textual adapter by explicitly modeling the dual-modality structure knowledge (i.e., the correlation of different semantics/classes in textual and visual modalities) with a dual knowledge graph. In particular, the dual knowledge graph is established with two sub-graphs, i.e., a textual knowledge sub-graph, and a visual knowledge sub-graph, where the nodes and edges represent the semantics/classes and their correlations in two modalities, respectively. This enables the textual feature of each prompt to leverage the task-specific structure knowledge from both textual and visual modalities, yielding a more effective classifier for downstream tasks. Extensive experimental results on 11 benchmark datasets reveal that our GraphAdapter significantly outperforms the previous adapter-based methods.

摘要:

适配器式高效迁移学习（ETL）在低数据条件下的视觉语言模型（VLM）调优中表现出了优异的性能，其中仅引入一些额外参数来挖掘基于VLM 的通用且强大的表示。然而，大多数适配器风格的作品面临两个限制：（i）仅使用单一模态对特定于任务的知识进行建模； (ii) 忽视下游任务中类间关系的利用，从而导致次优解决方案。为了缓解这个问题，我们提出了一种有效的适配器式调整策略，称为 GraphAdapter，它通过使用双模态结构知识（即文本和视觉模态中不同语义/类的相关性）显式建模来执行文本适配器。知识图。具体地，双知识图由两个子图建立，即文本知识子图和视觉知识子图，其中节点和边分别表示两种模态的语义/类及其相关性。这使得每个提示的文本特征能够利用来自文本和视觉模式的特定于任务的结构知识，从而为下游任务产生更有效的分类器。对 11 个基准数据集的广泛实验结果表明，我们的 GraphAdapter 显着优于之前基于适配器的方法。

## SatLM: Satisfiability-Aided Language Models Using Declarative Prompting<sup>poster<sup>

Authors: Xi Ye, Qiaochu Chen, Isil Dillig, Greg Durrett

Link: [https://neurips.cc/virtual/2023/poster/71537](https://neurips.cc/virtual/2023/poster/71537)

Abstract:

 Prior work has combined chain-of-thought prompting in large language models (LLMs) with programmatic representations to perform effective and transparent reasoning. While such an approach works well for tasks that only require forward reasoning (e.g., straightforward arithmetic), it is less effective for constraint solving problems that require more sophisticated planning and search. In this paper, we propose a new satisfiability-aided language modeling (SatLM) approach for improving the reasoning capabilities of LLMs. We use an LLM to generate a declarative task specification rather than an imperative program and leverage an off-the-shelf automated theorem prover to derive the final answer. This approach has two key advantages. The declarative specification is closer to the problem description than the reasoning steps are, so the LLM can parse it out of the description more accurately. Furthermore, by offloading the actual reasoning task to an automated theorem prover, our approach can guarantee the correctness of the answer with respect to the parsed specification and avoid planning errors in the solving process. We evaluate SATLM on 8 different datasets and show that it consistently outperforms program-aided LMs in the imperative paradigm. In particular, SATLM outperforms program-aided LMs by 23% on a challenging subset of the GSM arithmetic reasoning dataset; SATLM also achieves a new SoTA on LSAT and BoardgameQA, surpassing previous models that are trained on the respective training sets.

摘要:

先前的工作将大语言模型（LLM）中的思维链提示与程序化表示相结合，以执行有效且透明的推理。虽然这种方法对于只需要前向推理（例如，简单算术）的任务效果很好，但对于需要更复杂的规划和搜索的约束求解问题来说效果较差。在本文中，我们提出了一种新的可满足性辅助语言建模（SatLM）方法，用于提高法学硕士的推理能力。我们使用法学硕士来生成声明性任务规范而不是命令式程序，并利用现成的自动定理证明器来得出最终答案。这种方法有两个主要优点。声明性规范比推理步骤更接近问题描述，因此法学硕士可以更准确地从描述中解析出来。此外，通过将实际推理任务卸载给自动定理证明器，我们的方法可以保证答案相对于解析规范的正确性，并避免求解过程中的计划错误。我们在 8 个不同的数据集上评估 SATLM，并表明它在命令式范式中始终优于程序辅助的 LM。特别是，在 GSM 算术推理数据集的一个具有挑战性的子集上，SATLM 的性能比程序辅助的 LM 提高了 23%； SATLM 还在 LSAT 和 BoardgameQA 上实现了新的 SoTA，超越了之前在各自训练集上训练的模型。

## Passive learning of active causal strategies in agents and language models<sup>poster<sup>

Authors: Andrew Lampinen, Stephanie Chan, Ishita Dasgupta, Andrew Nam, Jane Wang

Link: [https://neurips.cc/virtual/2023/poster/72481](https://neurips.cc/virtual/2023/poster/72481)

Abstract:

 What can be learned about causality and experimentation from passive data? This question is salient given recent successes of passively-trained language models in interactive domains such as tool use. Passive learning is inherently limited. However, we show that purely passive learning can in fact allow an agent to learn generalizable strategies for determining and using causal structures, as long as the agent can intervene at test time. We formally illustrate that learning a strategy of first experimenting, then seeking goals, can allow generalization from passive learning in principle. We then show empirically that agents trained via imitation on expert data can indeed generalize at test time to infer and use causal links which are never present in the training data; these agents can also generalize experimentation strategies to novel variable sets never observed in training.We then show that strategies for causal intervention and exploitation can be generalized from passive data even in a more complex environment with high-dimensional observations, with the support of natural language explanations. Explanations can even allow passive learners to generalize out-of-distribution from perfectly-confounded training data. Finally, we show that language models, trained only on passive next-word prediction, can generalize causal intervention strategies from a few-shot prompt containing explanations and reasoning. These results highlight the surprising power of passive learning of active causal strategies, and have implications for understanding the behaviors and capabilities of language models.

摘要:

从被动数据中可以了解因果关系和实验什么？鉴于最近被动训练语言模型在工具使用等交互领域取得的成功，这个问题就显得尤为突出。被动学习本质上是有限的。然而，我们表明，纯粹的被动学习实际上可以让代理学习用于确定和使用因果结构的通用策略，只要代理可以在测试时进行干预。我们正式说明，学习先进行实验，然后寻求目标的策略原则上可以从被动学习中进行概括。然后，我们凭经验证明，通过模仿专家数据训练的智能体确实可以在测试时进行概括，以推断和使用训练数据中从未存在的因果关系；这些代理还可以将实验策略推广到训练中从未观察到的新变量集。然后，我们证明，即使在具有高维观察的更复杂的环境中，在自然语言的支持下，也可以从被动数据中推广因果干预和利用的策略解释。解释甚至可以让被动学习者从完全混杂的训练数据中概括出分布不均的情况。最后，我们表明，仅接受被动下一个单词预测训练的语言模型可以从包含解释和推理的几次提示中概括出因果干预策略。这些结果凸显了主动因果策略的被动学习的惊人力量，并且对于理解语言模型的行为和能力具有重要意义。

## Large Language Models for Automated Data Science: Introducing CAAFE for Context-Aware Automated Feature Engineering<sup>poster<sup>

Authors: Noah Hollmann, Samuel Müller, Frank Hutter

Link: [https://neurips.cc/virtual/2023/poster/72592](https://neurips.cc/virtual/2023/poster/72592)

Abstract:

 As the field of automated machine learning (AutoML) advances, it becomes increasingly important to incorporate domain knowledge into these systems.We present an approach for doing so by harnessing the power of large language models (LLMs). Specifically, we introduce Context-Aware Automated Feature Engineering (CAAFE), a feature engineering method for tabular datasets that utilizes an LLM to iteratively generate additional semantically meaningful features for tabular datasets based on the description of the dataset. The method produces both Python code for creating new features and explanations for the utility of the generated features.Despite being methodologically simple, CAAFE improves performance on 11 out of 14 datasets -- boosting mean ROC AUC performance from 0.798 to 0.822 across all dataset - similar to the improvement achieved by using a random forest instead of logistic regression on our datasets. Furthermore, CAAFE is interpretable by providing a textual explanation for each generated feature.CAAFE paves the way for more extensive semi-automation in data science tasks and emphasizes the significance of context-aware solutions that can extend the scope of AutoML systems to semantic AutoML. We release our code, a simple demo and a python package.

摘要:

随着自动化机器学习 (AutoML) 领域的进步，将领域知识纳入这些系统变得越来越重要。我们提出了一种通过利用大型语言模型 (LLM) 的力量来实现这一目标的方法。具体来说，我们介绍了上下文感知自动特征工程（CAAFE），这是一种针对表格数据集的特征工程方法，它利用 LLM 根据数据集的描述迭代地为表格数据集生成附加的语义上有意义的特征。该方法生成用于创建新特征的 Python 代码以及对所生成特征的实用性的解释。尽管方法简单，但 CAAFE 提高了 14 个数据集中的 11 个数据集的性能 - 将所有数据集的平均 ROC AUC 性能从 0.798 提高到 0.822 - 类似通过在我们的数据集上使用随机森林而不是逻辑回归所实现的改进。此外，CAAFE 可以通过为每个生成的特征提供文本解释来进行解释。CAAFE 为数据科学任务中更广泛的半自动化铺平了道路，并强调了上下文感知解决方案的重要性，这些解决方案可以将 AutoML 系统的范围扩展到语义 AutoML。我们发布了我们的代码、一个简单的演示和一个 python 包。

## Post Hoc Explanations of Language Models Can Improve Language Models<sup>poster<sup>

Authors: Satyapriya Krishna, Jiaqi Ma, Dylan Slack, Asma Ghandeharioun, Sameer Singh, Himabindu Lakkaraju

Link: [https://neurips.cc/virtual/2023/poster/72907](https://neurips.cc/virtual/2023/poster/72907)

Abstract:

 Large Language Models (LLMs) have demonstrated remarkable capabilities in performing complex tasks. Moreover, recent research has shown that incorporating human-annotated rationales (e.g., Chain-of-Thought prompting) during in-context learning can significantly enhance the performance of these models, particularly on tasks that require reasoning capabilities. However, incorporating such rationales poses challenges in terms of scalability as this requires a high degree of human involvement. In this work, we present a novel framework, Amplifying Model Performance by Leveraging In-Context Learning with Post Hoc Explanations (AMPLIFY), which addresses the aforementioned challenges by automating the process of rationale generation. To this end, we leverage post hoc explanation methods which output attribution scores (explanations) capturing the influence of each of the input features on model predictions. More specifically, we construct automated natural language rationales that embed insights from post hoc explanations to provide corrective signals to LLMs. Extensive experimentation with real-world datasets demonstrates that our framework, AMPLIFY, leads to prediction accuracy improvements of about 10-25% over a wide range of tasks, including those where prior approaches which rely on human-annotated rationales such as Chain-of-Thought prompting fall short. Our work makes one of the first attempts at highlighting the potential of post hoc explanations as valuable tools for enhancing the effectiveness of LLMs. Furthermore, we conduct additional empirical analyses and ablation studies to demonstrate the impact of each of the components of AMPLIFY, which, in turn, lead to critical insights for refining in context learning.

摘要:

大型语言模型（LLM）在执行复杂任务方面表现出了卓越的能力。此外，最近的研究表明，在上下文学习过程中纳入人工注释的基本原理（例如，思维链提示）可以显着提高这些模型的性能，特别是在需要推理能力的任务上。然而，纳入这些基本原理在可扩展性方面提出了挑战，因为这需要高度的人类参与。在这项工作中，我们提出了一个新颖的框架，通过利用上下文学习和事后解释来放大模型性能（AMPLIFY），它通过自动化原理生成过程来解决上述挑战。为此，我们利用事后解释方法输出归因分数（解释），捕获每个输入特征对模型预测的影响。更具体地说，我们构建了自动化的自然语言原理，其中嵌入了事后解释的见解，为法学硕士提供纠正信号。对现实世界数据集的广泛实验表明，我们的框架 AMPLIFY 在各种任务中使预测精度提高了约 10-25%，包括那些依赖于人工注释原理的先前方法（例如 Chain-of-）思考提示不足。我们的工作是强调事后解释作为提高法学硕士有效性的宝贵工具的潜力的首次尝试之一。此外，我们还进行了额外的实证分析和消融研究，以证明 AMPLIFY 每个组件的影响，这反过来又为上下文学习的改进提供了重要的见解。

## Textually Pretrained Speech Language Models<sup>poster<sup>

Authors: Michael Hassid, Tal Remez, Tu Anh Nguyen, Itai Gat, Alexis CONNEAU, Felix Kreuk, Jade Copet, Alexandre Defossez, Gabriel Synnaeve, Emmanuel Dupoux, Roy Schwartz, Yossi Adi

Link: [https://neurips.cc/virtual/2023/poster/71490](https://neurips.cc/virtual/2023/poster/71490)

Abstract:

 Speech language models (SpeechLMs) process and generate acoustic data only, without textual supervision. In this work, we propose TWIST, a method for training SpeechLMs using a warm-start from a pretrained textual language models. We show using both automatic and human evaluations that TWIST outperforms a cold-start SpeechLM across the board. We empirically analyze the effect of different model design choices such as the speech tokenizer, the pretrained textual model, and the dataset size. We find that model and dataset scale both play an important role in constructing better-performing SpeechLMs. Based on our observations, we present the largest (to the best of our knowledge) SpeechLM both in terms of number of parameters and training data. We additionally introduce two spoken versions of the StoryCloze textual benchmark to further improve model evaluation and advance future research in the field. We make speech samples, code and models publicly available.

摘要:

语音语言模型（SpeechLM）仅处理和生成声学数据，没有文本监督。在这项工作中，我们提出了 TWIST，一种使用预训练文本语言模型的热启动来训练 SpeechLM 的方法。我们使用自动和人工评估表明 TWIST 全面优于冷启动 SpeechLM。我们根据经验分析了不同模型设计选择（例如语音标记器、预训练文本模型和数据集大小）的效果。我们发现模型和数据集规模在构建性能更好的 SpeechLM 方面都发挥着重要作用。根据我们的观察，我们提出了（据我们所知）在参数数量和训练数据方面最大的 SpeechLM。我们还引入了 StoryCloze 文本基准的两个口语版本，以进一步改进模型评估并推进该领域的未来研究。我们公开提供语音样本、代码和模型。

## CAMEL: Communicative Agents for "Mind" Exploration of Large Language Model Society<sup>poster<sup>

Authors: Guohao Li, Hasan Abed Al Kader Hammoud, Hani Itani, Dmitrii Khizbullin, Bernard Ghanem

Link: [https://neurips.cc/virtual/2023/poster/72905](https://neurips.cc/virtual/2023/poster/72905)

Abstract:

 The rapid advancement of chat-based language models has led to remarkable progress in complex task-solving. However, their success heavily relies on human input to guide the conversation, which can be challenging and time-consuming. This paper explores the potential of building scalable techniques to facilitate autonomous cooperation among communicative agents, and provides insight into their “cognitive” processes. To address the challenges of achieving autonomous cooperation, we propose a novel communicative agent framework named role-playing . Our approach involves using inception prompting to guide chat agents toward task completion while maintaining consistency with human intentions. We showcase how role-playing can be used to generate conversational data for studying the behaviors and capabilities of a society of agents, providing a valuable resource for investigating conversational language models. In particular, we conduct comprehensive studies on instruction-following cooperation in multi-agent settings. Our contributions include introducing a novel communicative agent framework, offering a scalable approach for studying the cooperative behaviors and capabilities of multi-agent systems, and open-sourcing our library to support research on communicative agents and beyond: https://github.com/camel-ai/camel.

摘要:

基于聊天的语言模型的快速发展导致复杂任务解决方面取得了显着进展。然而，他们的成功在很大程度上依赖于人类输入来指导对话，这可能具有挑战性且耗时。本文探讨了构建可扩展技术以促进通信代理之间自主合作的潜力，并深入了解其“认知”过程。为了解决实现自主合作的挑战，我们提出了一种名为角色扮演的新型通信代理框架。我们的方法涉及使用初始提示来引导聊天代理完成任务，同时保持与人类意图的一致性。我们展示了如何使用角色扮演来生成对话数据，以研究代理社会的行为和能力，为研究对话语言模型提供宝贵的资源。特别是，我们对多智能体环境中的指令遵循合作进行了全面的研究。我们的贡献包括引入一种新颖的通信代理框架，提供一种可扩展的方法来研究多代理系统的合作行为和功能，以及开源我们的库以支持通信代理及其他方面的研究：https://github.com/骆驼-艾/骆驼。

## Large Language Models Are Semi-Parametric Reinforcement Learning Agents<sup>poster<sup>

Authors: Danyang Zhang, Lu Chen, Situo Zhang, Hongshen Xu, Zihan Zhao, Kai Yu

Link: [https://neurips.cc/virtual/2023/poster/71228](https://neurips.cc/virtual/2023/poster/71228)

Abstract:

 Inspired by the insights in cognitive science with respect to human memory and reasoning mechanism, a novel evolvable LLM-based (Large Language Model) agent framework is proposed as Rememberer. By equipping the LLM with a long-term experience memory, Rememberer is capable of exploiting the experiences from the past episodes even for different task goals, which excels an LLM-based agent with fixed exemplars or equipped with a transient working memory. We further introduce Reinforcement Learning with Experience Memory (RLEM) to update the memory. Thus, the whole system can learn from the experiences of both success and failure, and evolve its capability without fine-tuning the parameters of the LLM. In this way, the proposed Rememberer constitutes a semi-parametric RL agent. Extensive experiments are conducted on two RL task sets to evaluate the proposed framework. The average results with different initialization and training sets exceed the prior SOTA by 4% and 2% for the success rate on two task sets and demonstrate the superiority and robustness of Rememberer.

摘要:

受认知科学对人类记忆和推理机制的见解的启发，提出了一种新型可进化的基于 LLM（大语言模型）的代理框架：Rememberer。通过为 LLM 配备长期经验记忆，Rememberer 能够利用过去的经验来实现不同的任务目标，这优于具有固定样本或配备瞬时工作记忆的基于 LLM 的代理。我们进一步引入带有经验记忆的强化学习（RLEM）来更新记忆。因此，整个系统可以从成功和失败的经验中学习，并在不微调LLM参数的情况下发展其能力。这样，所提出的 Rememberer 就构成了一个半参数 RL 代理。在两个 RL 任务集上进行了大量的实验来评估所提出的框架。不同初始化和训练集的平均结果在两个任务集上的成功率分别比之前的 SOTA 提高了 4% 和 2%，证明了 Rememberer 的优越性和鲁棒性。

## Benchmarking Robustness of Adaptation Methods on Pre-trained Vision-Language Models<sup>poster<sup>

Authors: Shuo Chen, Jindong Gu, Zhen Han, Yunpu Ma, Philip Torr, Volker Tresp

Link: [https://neurips.cc/virtual/2023/poster/73702](https://neurips.cc/virtual/2023/poster/73702)

Abstract:

 Various adaptation methods, such as LoRA, prompts, and adapters, have been proposed to enhance the performance of pre-trained vision-language models in specific domains. As test samples in real-world applications usually differ from adaptation data, the robustness of these adaptation methods against distribution shifts are essential. In this study, we assess the robustness of 11 widely-used adaptation methods across 4 vision-language datasets under multimodal corruptions. Concretely, we introduce 7 benchmark datasets, including 96 visual and 87 textual corruptions, to investigate the robustness of different adaptation methods, the impact of available adaptation examples, and the influence of trainable parameter size during adaptation. Our analysis reveals that: 1) Adaptation methods are more sensitive to text corruptions than visual corruptions. 2) Full fine-tuning does not consistently provide the highest robustness; instead, adapters can achieve better robustness with comparable clean performance. 3) Contrary to expectations, our findings indicate that increasing the number of adaptation data and parameters does not guarantee enhanced robustness; instead, it results in even lower robustness. We hope this study could benefit future research in the development of robust multimodal adaptation methods. The benchmark, code, and dataset used in this study can be accessed at https://adarobustness.github.io.

摘要:

人们提出了多种适应方法，例如 LoRA、提示和适配器，以增强预训练视觉语言模型在特定领域的性能。由于现实应用中的测试样本通常与适应数据不同，因此这些适应方法针对分布变化的鲁棒性至关重要。在这项研究中，我们评估了 4 个视觉语言数据集上 11 种广泛使用的适应方法在多模态损坏下的稳健性。具体来说，我们引入了 7 个基准数据集，包括 96 个视觉损坏和 87 个文本损坏，以研究不同适应方法的鲁棒性、可用适应示例的影响以及适应过程中可训练参数大小的影响。我们的分析表明：1）适应方法对文本损坏比视觉损坏更敏感。 2) 完全微调并不能始终提供最高的鲁棒性；相反，适配器可以实现更好的鲁棒性和相当的清洁性能。 3）与预期相反，我们的研究结果表明，增加适应数据和参数的数量并不能保证增强的稳健性；相反，它会导致鲁棒性更低。我们希望这项研究能够有益于未来开发稳健的多模式适应方法的研究。本研究中使用的基准、代码和数据集可以在 https://adarobustness.github.io 访问。

## On Evaluating Adversarial Robustness of Large Vision-Language Models<sup>poster<sup>

Authors: Yunqing Zhao, Tianyu Pang, Chao Du, Xiao Yang, Chongxuan LI, Ngai-Man (Man) Cheung, Min Lin

Link: [https://neurips.cc/virtual/2023/poster/69997](https://neurips.cc/virtual/2023/poster/69997)

Abstract:

 Large vision-language models (VLMs) such as GPT-4 have achieved unprecedented performance in response generation, especially with visual inputs, enabling more creative and adaptable interaction than large language models such as ChatGPT. Nonetheless, multimodal generation exacerbates safety concerns, since adversaries may successfully evade the entire system by subtly manipulating the most vulnerable modality (e.g., vision). To this end, we propose evaluating the robustness of open-source large VLMs in the most realistic and high-risk setting, where adversaries have only black-box system access and seek to deceive the model into returning the targeted responses. In particular, we first craft targeted adversarial examples against pretrained models such as CLIP and BLIP, and then transfer these adversarial examples to other VLMs such as MiniGPT-4, LLaVA, UniDiffuser, BLIP-2, and Img2Prompt. In addition, we observe that black-box queries on these VLMs can further improve the effectiveness of targeted evasion, resulting in a surprisingly high success rate for generating targeted responses. Our findings provide a quantitative understanding regarding the adversarial vulnerability of large VLMs and call for a more thorough examination of their potential security flaws before deployment in practice. Our project page: https://yunqing-me.github.io/AttackVLM/.

摘要:

GPT-4 等大型视觉语言模型 (VLM) 在响应生成方面取得了前所未有的性能，特别是在视觉输入方面，与 ChatGPT 等大型语言模型相比，能够实现更具创造性和适应性的交互。尽管如此，多模态生成加剧了安全问题，因为对手可以通过巧妙地操纵最脆弱的模态（例如视觉）来成功逃避整个系统。为此，我们建议在最现实和高风险的环境中评估开源大型 VLM 的稳健性，在这种环境中，对手只有黑盒系统访问权限，并试图欺骗模型返回目标响应。特别是，我们首先针对 CLIP 和 BLIP 等预训练模型制作有针对性的对抗性示例，然后将这些对抗性示例转移到其他 VLM，如 MiniGPT-4、LLaVA、UniDiffuser、BLIP-2 和 Img2Prompt。此外，我们观察到对这些 VLM 的黑盒查询可以进一步提高有针对性的规避的有效性，从而导致生成有针对性的响应的成功率高得惊人。我们的研究结果提供了对大型 VLM 的对抗性漏洞的定量理解，并呼吁在实际部署之前对其潜在的安全缺陷进行更彻底的检查。我们的项目页面：https://yunqing-me.github.io/AttackVLM/。

## What can Large Language Models do in chemistry? A comprehensive benchmark on eight tasks<sup>poster<sup>

Authors: Taicheng Guo, kehan Guo, Bozhao Nan, Zhenwen Liang, Zhichun Guo, Nitesh Chawla, Olaf Wiest, Xiangliang Zhang

Link: [https://neurips.cc/virtual/2023/poster/73716](https://neurips.cc/virtual/2023/poster/73716)

Abstract:

 Large Language Models (LLMs) with strong abilities in natural language processing tasks have emerged and have been applied in various kinds of areas such as science, finance and software engineering. However, the capability of LLMs to advance the field of chemistry remains unclear. In this paper, rather than pursuing state-of-the-art performance, we aim to evaluate capabilities of LLMs in a wide range of tasks across the chemistry domain. We identify three key chemistry-related capabilities including understanding, reasoning and explaining to explore in LLMs and establish a benchmark containing eight chemistry tasks. Our analysis draws on widely recognized datasets facilitating a broad exploration of the capacities of LLMs within the context of practical chemistry. Five LLMs (GPT-4,GPT-3.5, Davinci-003, Llama and Galactica) are evaluated for each chemistry task in zero-shot and few-shot in-context learning settings with carefully selected demonstration examples and specially crafted prompts. Our investigation found that GPT-4 outperformed other models and LLMs exhibit different competitive levels in eight chemistry tasks. In addition to the key findings from the comprehensive benchmark analysis, our work provides insights into the limitation of current LLMs and the impact of in-context learning settings on LLMs’ performance across various chemistry tasks. The code and datasets used in this study are available at https://github.com/ChemFoundationModels/ChemLLMBench.

摘要:

 具有强大的自然语言处理任务能力的大型语言模型（LLM）已经出现，并已应用于科学、金融和软件工程等各个领域。然而，法学硕士推动化学领域发展的能力仍不清楚。在本文中，我们的目标不是追求最先进的表现，而是评估法学硕士在化学领域各种任务中的能力。我们确定了法学硕士中需要探索的三种关键的化学相关能力，包括理解、推理和解释，并建立了包含八项化学任务的基准。我们的分析利用了广泛认可的数据集，促进了法学硕士在实用化学背景下能力的广泛探索。五个法学硕士（GPT-4、GPT-3.5、Davinci-003、Llama 和 Gactica）在零样本和少样本上下文学习环境中的每项化学任务中进行评估，并使用精心挑选的演示示例和专门制作的提示。我们的调查发现，GPT-4 优于其他模型，法学硕士在八项化学任务中表现出不同的竞争水平。除了综合基准分析的主要发现之外，我们的工作还深入了解了当前法学硕士的局限性以及情境学习设置对法学硕士在各种化学任务中表现的影响。本研究中使用的代码和数据集可从 https://github.com/ChemFoundationModels/ChemmLLMBench 获取。

## CoLLAT: On Adding Fine-grained Audio Understanding to Language Models using Token-Level Locked-Language Tuning<sup>poster<sup>

Authors: Dadallage A R Silva, Spencer Whitehead, Christopher Lengerich, Hugh Leather

Link: [https://neurips.cc/virtual/2023/poster/72956](https://neurips.cc/virtual/2023/poster/72956)

Abstract:

 Humans can easily understand various audio concepts, but conventional audio classification models fail due to their inability to predict unseen classes during training. To address this challenge, recent literature has explored contrastive language-audio pretraining to learn an audio understanding model using natural language supervision from a pretrained language model. However, despite their reasonable zero-shot performance in audio understanding, these models typically fail to achieve optimal performance while preserving the text understanding capabilities of the pretrained language model. They also perform poorly when comprehending audio clips with multiple audio concepts. To bridge these gaps, we propose $CoLLAT$: $Co$ntrastive $L$ocked $L$anguage and $A$udio $T$uning. This is a framework to effectively learn an audio understanding model with a locked language model, which is learned using a novel pretraining objective for audio-to-text grounding to yield fine-grained audio understanding. Our extensive experiments, which include several downstream applications such as audio classification, cross-modal retrieval, and audio-guided image generation, demonstrate that $CoLLAT$ yields state-of-the-art performance for audio understanding. Additionally, it unlocks audio guidance to applications built on top of pretrained language models.

摘要:

人类可以轻松理解各种音频概念，但传统的音频分类模型由于无法预测训练过程中看不见的类别而失败。为了应对这一挑战，最近的文献探索了对比语言-音频预训练，以使用来自预训练语言模型的自然语言监督来学习音频理解模型。然而，尽管它们在音频理解方面具有合理的零样本性能，但这些模型通常无法在保留预训练语言模型的文本理解能力的同时实现最佳性能。他们在理解具有多个音频概念的音频剪辑时也表现不佳。为了弥补这些差距，我们建议 $CoLLAT$：$Co$ntrastive $L$ocked $L$anguage 和 $A$udio $T$uning。这是一个使用锁定语言模型有效学习音频理解模型的框架，该框架是使用一种新颖的音频到文本基础的预训练目标来学习的，以产生细粒度的音频理解。我们的广泛实验（包括音频分类、跨模态检索和音频引导图像生成等多个下游应用）表明，$CoLLAT$ 在音频理解方面具有最先进的性能。此外，它还为基于预训练语言模型构建的应用程序解锁了音频指导。

## VisionLLM: Large Language Model is also an Open-Ended Decoder for Vision-Centric Tasks<sup>poster<sup>

Authors: Wenhai Wang, Zhe Chen, Xiaokang Chen, Jiannan Wu, Xizhou Zhu, Gang Zeng, Ping Luo, Tong Lu, Jie Zhou, Yu Qiao, Jifeng Dai

Link: [https://neurips.cc/virtual/2023/poster/71428](https://neurips.cc/virtual/2023/poster/71428)

Abstract:

 Large language models (LLMs) have notably accelerated progress towards artificial general intelligence (AGI), with their impressive zero-shot capacity for user-tailored tasks, endowing them with immense potential across a range of applications. However, in the field of computer vision, despite the availability of numerous powerful vision foundation models (VFMs), they are still restricted to tasks in a pre-defined form, struggling to match the open-ended task capabilities of LLMs. In this work, we present an LLM-based framework for vision-centric tasks, termed VisionLLM. This framework provides a unified perspective for vision and language tasks by treating images as a foreign language and aligning vision-centric tasks with language tasks that can be flexibly defined and managed using language instructions. An LLM-based decoder can then make appropriate predictions based on these instructions for open-ended tasks. Extensive experiments show that the proposed VisionLLM can achieve different levels of task customization through language instructions, from fine-grained object-level to coarse-grained task-level customization, all with good results. It's noteworthy that, with a generalist LLM-based framework, our model can achieve over 60% mAP on COCO, on par with detection-specific models. We hope this model can set a new baseline for generalist vision and language models. The code shall be released.

摘要:

大型语言模型（LLM）显着加速了通用人工智能（AGI）的进步，其对用户定制任务具有令人印象深刻的零样本能力，赋予它们在一系列应用中的巨大潜力。然而，在计算机视觉领域，尽管有众多强大的视觉基础模型（VFM）可用，但它们仍然仅限于预定义形式的任务，难以与法学硕士的开放式任务能力相匹配。在这项工作中，我们提出了一个基于 LLM 的框架，用于以视觉为中心的任务，称为 VisionLLM。该框架通过将图像视为外语，并将以视觉为中心的任务与可以使用语言指令灵活定义和管理的语言任务结合起来，为视觉和语言任务提供了统一的视角。然后，基于 LLM 的解码器可以根据这些指令对开放式任务做出适当的预测。大量实验表明，所提出的VisionLLM可以通过语言指令实现不同级别的任务定制，从细粒度的对象级到粗粒度的任务级定制，均取得了良好的效果。值得注意的是，通过基于 LLM 的通用框架，我们的模型可以在 COCO 上实现超过 60% 的 mAP，与特定于检测的模型相当。我们希望这个模型能够为通才视觉和语言模型设定新的基线。代码将被发布。

## Large language models transition from integrating across position-yoked, exponential windows to structure-yoked, power-law windows<sup>poster<sup>

Authors: David Skrill, Samuel Norman-Haignere

Link: [https://neurips.cc/virtual/2023/poster/73028](https://neurips.cc/virtual/2023/poster/73028)

Abstract:

 Modern language models excel at integrating across long temporal scales needed to encode linguistic meaning and show non-trivial similarities to biological neural systems. Prior work suggests that human brain responses to language exhibit hierarchically organized "integration windows" that substantially constrain the overall influence of an input token (e.g., a word) on the neural response. However, little prior work has attempted to use integration windows to characterize computations in large language models (LLMs). We developed a simple word-swap procedure for estimating integration windows from black-box language models that does not depend on access to gradients or knowledge of the model architecture (e.g., attention weights). Using this method, we show that trained LLMs exhibit stereotyped integration windows that are well-fit by a convex combination of an exponential and a power-law function, with a partial transition from exponential to power-law dynamics across network layers. We then introduce a metric for quantifying the extent to which these integration windows vary with structural boundaries (e.g., sentence boundaries), and using this metric, we show that integration windows become increasingly yoked to structure at later network layers. None of these findings were observed in an untrained model, which as expected integrated uniformly across its input. These results suggest that LLMs learn to integrate information in natural language using a stereotyped pattern: integrating across position-yoked, exponential windows at early layers, followed by structure-yoked, power-law windows at later layers. The methods we describe in this paper provide a general-purpose toolkit for understanding temporal integration in language models, facilitating cross-disciplinary research at the intersection of biological and artificial intelligence.

摘要:

现代语言模型擅长整合编码语言意义所需的长时间尺度，并显示出与生物神经系统的非平凡相似性。先前的工作表明，人脑对语言的反应表现出分层组织的“整合窗口”，该窗口实质上限制了输入标记（例如，单词）对神经反应的总体影响。然而，之前很少有工作尝试使用集成窗口来表征大型语言模型（LLM）中的计算。我们开发了一个简单的单词交换过程，用于估计黑盒语言模型的集成窗口，该过程不依赖于对梯度的访问或模型架构的知识（例如，注意力权重）。使用这种方法，我们表明训练有素的 LLM 表现出刻板的积分窗口，该窗口非常适合指数函数和幂律函数的凸组合，并且跨网络层从指数到幂律动态的部分过渡。然后，我们引入一个度量来量化这些集成窗口随结构边界（例如，句子边界）变化的程度，并使用该度量，我们表明集成窗口越来越与后面的网络层的结构相关联。在未经训练的模型中没有观察到这些发现，正如预期的那样，该模型在其输入中统一整合。这些结果表明，法学硕士学习使用刻板模式整合自然语言中的信息：在早期层跨位置关联的指数窗口进行整合，然后在后面的层进行结构关联的幂律窗口整合。我们在本文中描述的方法提供了一个通用工具包，用于理解语言模型中的时间整合，促进生物和人工智能交叉领域的跨学科研究。

## Text Promptable Surgical Instrument Segmentation with Vision-Language Models<sup>poster<sup>

Authors: Zijian Zhou, Oluwatosin Alabi, Meng Wei, Tom Vercauteren, Miaojing Shi

Link: [https://neurips.cc/virtual/2023/poster/71267](https://neurips.cc/virtual/2023/poster/71267)

Abstract:

 In this paper, we propose a novel text promptable surgical instrument segmentation approach to overcome challenges associated with diversity and differentiation of surgical instruments in minimally invasive surgeries. We redefine the task as text promptable, thereby enabling a more nuanced comprehension of surgical instruments and adaptability to new instrument types. Inspired by recent advancements in vision-language models, we leverage pretrained image and text encoders as our model backbone and design a text promptable mask decoder consisting of attention- and convolution-based prompting schemes for surgical instrument segmentation prediction. Our model leverages multiple text prompts for each surgical instrument through a new mixture of prompts mechanism, resulting in enhanced segmentation performance. Additionally, we introduce a hard instrument area reinforcement module to improve image feature comprehension and segmentation precision. Extensive experiments on several surgical instrument segmentation datasets demonstrate our model's superior performance and promising generalization capability. To our knowledge, this is the first implementation of a promptable approach to surgical instrument segmentation, offering significant potential for practical application in the field of robotic-assisted surgery.

摘要:

在本文中，我们提出了一种新颖的文本提示手术器械分割方法，以克服微创手术中手术器械多样性和差异化带来的挑战。我们将任务重新定义为文本提示，从而能够更细致地理解手术器械并适应新的器械类型。受视觉语言模型最新进展的启发，我们利用预训练的图像和文本编码器作为我们的模型主干，并设计了一个文本提示掩模解码器，其中包括用于手术器械分割预测的基于注意力和卷积的提示方案。我们的模型通过新的混合提示机制利用每个手术器械的多个文本提示，从而增强了分割性能。此外，我们引入了硬仪器区域增强模块来提高图像特征理解和分割精度。对多个手术器械分割数据集的广泛实验证明了我们的模型的卓越性能和有前途的泛化能力。据我们所知，这是手术器械分割的快速方法的首次实施，为机器人辅助手术领域的实际应用提供了巨大的潜力。

## Data Selection for Language Models via Importance Resampling<sup>poster<sup>

Authors: Sang Michael Xie, Shibani Santurkar, Tengyu Ma, Percy Liang

Link: [https://neurips.cc/virtual/2023/poster/70154](https://neurips.cc/virtual/2023/poster/70154)

Abstract:

 Selecting a suitable pretraining dataset is crucial for both general-domain (e.g., GPT-3) and domain-specific (e.g., Codex) language models (LMs). We formalize this problem as selecting a subset of a large raw unlabeled dataset to match a desired target distribution given some unlabeled target samples. Due to the large scale and dimensionality of the raw text data, existing methods use simple heuristics or use experts to manually curate data. Instead, we extend the classic importance resampling approach used in low-dimensions for LM data selection. We propose Data Selection with Importance Resampling (DSIR), an efficient and scalable framework that estimates importance weights in a reduced feature space for tractability and selects data with importance resampling according to these weights. To determine an appropriate feature space, we show that KL reduction, a data metric that measures the proximity between selected pretraining data and the target in a feature space, has high correlation with average downstream accuracy (r=0.89) when computed with simple n-gram features. This motivates our instantiation of DSIR using n-gram features. When performing continued pretraining towards a specific domain, DSIR performs comparably to expert curation across 8 target distributions. When pretraining general-domain models (target is Wikipedia + books), DSIR improves over random selection and heuristic filtering baselines by 2-2.5% on the GLUE benchmark.

摘要:

选择合适的预训练数据集对于通用领域（例如 GPT-3）和特定领域（例如 Codex）语言模型（LM）都至关重要。我们将这个问题形式化为选择一个大型原始未标记数据集的子集来匹配给定一些未标记目标样本的所需目标分布。由于原始文本数据规模大、维度多，现有方法使用简单的启发式方法或使用专家手动整理数据。相反，我们扩展了低维 LM 数据选择中使用的经典重要性重采样方法。我们提出了具有重要性重采样的数据选择（DSIR），这是一种高效且可扩展的框架，可以估计缩小的特征空间中的重要性权重以实现易处理，并根据这些权重选择具有重要性重采样的数据。为了确定合适的特征空间，我们证明了 KL 缩减（一种衡量特征空间中选定的预训练数据与目标之间的接近程度的数据度量）在使用简单的 n- 计算时与平均下游精度 (r=0.89) 具有高度相关性克特征。这促使我们使用 n-gram 特征来实例化 DSIR。当针对特定领域进行持续预训练时，DSIR 在 8 个目标分布上的表现与专家管理相当。在预训练通用领域模型（目标是维基百科 + 书籍）时，DSIR 在 GLUE 基准上比随机选择和启发式过滤基线提高了 2-2.5%。

## Large language models implicitly learn to straighten neural sentence trajectories to construct a predictive representation of natural language.<sup>poster<sup>

Authors: Eghbal Hosseini, Evelina Fedorenko

Link: [https://neurips.cc/virtual/2023/poster/70807](https://neurips.cc/virtual/2023/poster/70807)

Abstract:

 Predicting upcoming events is critical to our ability to effectively interact with ourenvironment and conspecifics. In natural language processing, transformer models,which are trained on next-word prediction, appear to construct a general-purposerepresentation of language that can support diverse downstream tasks. However, westill lack an understanding of how a predictive objective shapes such representations.Inspired by recent work in vision neuroscience Hénaff et al. (2019), here we test ahypothesis about predictive representations of autoregressive transformer models.In particular, we test whether the neural trajectory of a sequence of words in asentence becomes progressively more straight as it passes through the layers of thenetwork. The key insight behind this hypothesis is that straighter trajectories shouldfacilitate prediction via linear extrapolation. We quantify straightness using a 1-dimensional curvature metric, and present four findings in support of the trajectorystraightening hypothesis: i) In trained models, the curvature progressively decreasesfrom the first to the middle layers of the network. ii) Models that perform better onthe next-word prediction objective, including larger models and models trained onlarger datasets, exhibit greater decreases in curvature, suggesting that this improvedability to straighten sentence neural trajectories may be the underlying driver ofbetter language modeling performance. iii) Given the same linguistic context, thesequences that are generated by the model have lower curvature than the groundtruth (the actual continuations observed in a language corpus), suggesting thatthe model favors straighter trajectories for making predictions. iv) A consistentrelationship holds between the average curvature and the average surprisal ofsentences in the middle layers of models, such that sentences with straighter neuraltrajectories also have lower surprisal. Importantly, untrained models don’t exhibitthese behaviors. In tandem, these results support the trajectory straighteninghypothesis and provide a possible mechanism for how the geometry of the internalrepresentations of autoregressive models supports next word prediction.

摘要:

预测即将发生的事件对于我们与环境和同类有效互动的能力至关重要。在自然语言处理中，经过下一个单词预测训练的 Transformer 模型似乎构建了可以支持各种下游任务的通用语言表示。然而，我们仍然缺乏对预测目标如何形成这种表征的理解。受到视觉神经科学 Hénaff 等人最近工作的启发。 （2019），在这里我们测试了关于自回归变压器模型的预测表示的假设。特别是，我们测试了句子中单词序列的神经轨迹在穿过网络层时是否逐渐变得更加直。这一假设背后的关键见解是，更直的轨迹应该有助于通过线性外推进行预测。我们使用一维曲率度量来量化直线度，并提出四个发现来支持轨迹拉直假设：i）在训练模型中，曲率从网络的第一层到中间层逐渐减小。 ii）在下一个单词预测目标上表现更好的模型，包括更大的模型和在更大数据集上训练的模型，表现出更大的曲率下降，这表明这种拉直句子神经轨迹的改进能力可能是更好的语言建模性能的潜在驱动力。 iii）在相同的语言环境下，模型生成的序列的曲率低于真实值（在语言语料库中观察到的实际连续），这表明该模型倾向于使用更直的轨迹进行预测。 iv) 模型中间层句子的平均曲率和平均惊讶度之间存在一致的关系，使得神经轨迹较直的句子也具有较低的惊讶度。重要的是，未经训练的模型不会表现出这些行为。同时，这些结果支持轨迹矫直假设，并为自回归模型内部表示的几何如何支持下一个单词预测提供了可能的机制。

## Grammar Prompting for Domain-Specific Language Generation with  Large Language Models<sup>poster<sup>

Authors: Bailin Wang, Zi Wang, Xuezhi Wang, Yuan Cao, Rif A. Saurous, Yoon Kim

Link: [https://neurips.cc/virtual/2023/poster/72512](https://neurips.cc/virtual/2023/poster/72512)

Abstract:

 Large language models (LLMs)  can learn to perform a wide range of natural language tasks from just a  handful of in-context examples. However, for generating strings from highly structured  languages (e.g., semantic parsing to complex domain-specific languages), it is challenging for the LLM to generalize from just a few exemplars. We propose \emph{grammar prompting}, a simple approach to enable LLMs to use external knowledge and domain-specific constraints, expressed through a grammar in Backus--Naur Form (BNF), during in-context learning. Grammar prompting augments each demonstration example with a specialized grammar that is minimally sufficient for generating the particular output example, where the specialized grammar is a subset of the full DSL grammar.  For inference, the LLM first predicts a BNF grammar given a test input, and then generates the output according to the rules of the grammar. Experiments demonstrate that grammar prompting can enable LLMs to perform competitively on a diverse set of DSL generation tasks, including semantic parsing (SMCalFlow, Overnight, GeoQuery), PDDL planning, and SMILES-based molecule generation.

摘要:

大型语言模型（LLM）可以通过少量的上下文示例来学习执行各种自然语言任务。然而，为了从高度结构化的语言（例如，语义解析到复杂的特定领域语言）生成字符串，法学硕士很难从几个范例中进行概括。我们提出\emph{语法提示}，这是一种简单的方法，使法学硕士能够在上下文学习期间使用外部知识和特定领域的约束，通过巴科斯-诺尔范式（BNF）语法来表达。语法提示通过专门的语法增强了每个演示示例，该语法至少足以生成特定的输出示例，其中专门的语法是完整 DSL 语法的子集。对于推理，LLM 首先在给定测试输入的情况下预测 BNF 语法，然后根据语法规则生成输出。实验表明，语法提示可以使法学硕士能够在各种 DSL 生成任务上具有竞争力，包括语义解析（SMCalFlow、Overnight、GeoQuery）、PDDL 规划和基于 SMILES 的分子生成。

## Large Language Models are Visual Reasoning Coordinators<sup>poster<sup>

Authors: Liangyu Chen, Bo Li, Sheng Shen, Jingkang Yang, Chunyuan Li, Kurt Keutzer, Trevor Darrell, Ziwei Liu

Link: [https://neurips.cc/virtual/2023/poster/72992](https://neurips.cc/virtual/2023/poster/72992)

Abstract:

 Visual reasoning requires multimodal perception and commonsense cognition of the world. Recently, multiple vision-language models (VLMs) have been proposed with excellent commonsense reasoning ability in various domains. However, how to harness the collective power of these complementary VLMs is rarely explored. Existing methods like ensemble still struggle to aggregate these models with the desired higher-order communications. In this work, we propose Cola, a novel paradigm that coordinates multiple VLMs for visual reasoning. Our key insight is that a large language model (LLM) can efficiently coordinate multiple VLMs by facilitating natural language communication that leverages their distinct and complementary capabilities. Extensive experiments demonstrate that our instruction tuning variant, Cola-FT, achieves state-of-the-art performance on visual question answering (VQA), outside knowledge VQA, visual entailment, and visual spatial reasoning tasks. Moreover, we show that our in-context learning variant, Cola-Zero, exhibits competitive performance in zero and few-shot settings, without finetuning. Through systematic ablation studies and visualizations, we validate that a coordinator LLM indeed comprehends the instruction prompts as well as the separate functionalities of VLMs; it then coordinates them to enable impressive visual reasoning capabilities.

摘要:

视觉推理需要多模态感知和对世界的常识认知。最近，人们提出了多种视觉语言模型（VLM），在各个领域都具有出色的常识推理能力。然而，如何利用这些互补的 VLM 的集体力量却很少被探讨。像集成这样的现有方法仍然难以将这些模型与所需的高阶通信聚合起来。在这项工作中，我们提出了 Cola，这是一种协调多个 VLM 进行视觉推理的新颖范式。我们的主要见解是，大型语言模型 (LLM) 可以通过促进利用其独特且互补的功能的自然语言通信来有效地协调多个 VLM。大量实验表明，我们的指令调整变体 Cola-FT 在视觉问答 (VQA)、外部知识 VQA、视觉蕴涵和视觉空间推理任务上实现了最先进的性能。此外，我们还表明，我们的上下文学习变体 Cola-Zero 在零次和少次设置中表现出有竞争力的性能，无需进行微调。通过系统的消融研究和可视化，我们验证了法学硕士协调员确实理解了指令提示以及 VLM 的单独功能；然后它协调它们以实现令人印象深刻的视觉推理能力。

## Can Language Models Teach? Teacher Explanations Improve Student Performance via Personalization<sup>poster<sup>

Authors: Swarnadeep Saha, Peter Hase, Mohit Bansal

Link: [https://neurips.cc/virtual/2023/poster/72111](https://neurips.cc/virtual/2023/poster/72111)

Abstract:

 A hallmark property of explainable AI models is the ability to teach other agents, communicating knowledge of how to perform a task. While Large Language Models (LLMs) perform complex reasoning by generating explanations for their predictions, it is unclear whether they also make good teachers for weaker agents. To address this, we consider a student-teacher framework between two LLM agents and study if, when, and how the teacher should intervene with natural language explanations to improve the student’s performance. Since communication is expensive, we define a budget such that the teacher only communicates explanations for a fraction of the data, after which the student should perform well on its own. We decompose the teaching problem along four axes: (1) if teacher’s test time in- tervention improve student predictions, (2) when it is worth explaining a data point, (3) how the teacher should personalize explanations to better teach the student, and (4) if teacher explanations also improve student performance on future unexplained data. We first show that teacher LLMs can indeed intervene on student reasoning to improve their performance. Next, inspired by the Theory of Mind abilities of effective teachers, we propose building two few-shot mental models of the student. The first model defines an Intervention Function that simulates the utility of an intervention, allowing the teacher to intervene when this utility is the highest and improving student performance at lower budgets. The second model enables the teacher to personalize explanations for a particular student and outperform unpersonalized teachers. We also demonstrate that in multi-turn interactions, teacher explanations generalize and learning from explained data improves student performance on future unexplained data. Finally, we also verify that misaligned teachers can lower student performance to random chance by intentionally misleading them.

摘要:

可解释的人工智能模型的一个标志性特性是能够教导其他智能体，交流如何执行任务的知识。虽然大型语言模型（LLM）通过为其预测生成解释来执行复杂的推理，但尚不清楚它们是否也能成为较弱智能体的好老师。为了解决这个问题，我们考虑了两个法学硕士代理人之间的学生-教师框架，并研究教师是否、何时以及如何干预自然语言解释以提高学生的表现。由于沟通的成本很高，我们定义了一个预算，让老师只传达对一小部分数据的解释，之后学生应该自己表现良好。我们沿着四个轴分解教学问题：（1）教师的测试时间干预是否改善了学生的预测，（2）何时值得解释数据点，（3）教师应如何个性化解释以更好地教导学生， (4) 教师的解释是否也能提高学生在未来未解释数据上的表现。我们首先证明法学硕士教师确实可以干预学生的推理以提高他们的表现。接下来，受到高效教师心智理论能力的启发，我们建议建立两个学生的小样本心智模型。第一个模型定义了模拟干预效用的干预函数，允许教师在效用最高时进行干预，并以较低的预算提高学生的表现。第二种模型使教师能够对特定学生进行个性化解释，并超越非个性化的教师。我们还证明，在多轮交互中，教师的解释可以概括，并且从解释的数据中学习可以提高学生在未来未解释的数据上的表现。最后，我们还验证了不一致的教师可以通过故意误导学生来随机降低学生的表现。

## Language Model Tokenizers Introduce Unfairness Between Languages<sup>poster<sup>

Authors: Aleksandar Petrov, Emanuele La Malfa, Philip Torr, Adel Bibi

Link: [https://neurips.cc/virtual/2023/poster/72721](https://neurips.cc/virtual/2023/poster/72721)

Abstract:

 Recent language models have shown impressive multilingual performance, even when not explicitly trained for it.Despite this, there are concerns about the quality of their outputs across different languages.In this paper, we show how disparity in the treatment of different languages arises at the tokenization stage, well before a model is even invoked.The same text translated into different languages can have drastically different tokenization lengths, with differences up to 15 times in some cases.These disparities persist even for tokenizers that are intentionally trained for multilingual support.Character-level and byte-level models also exhibit over 4 times the difference in the encoding length for some language pairs.This induces unfair treatment for some language communities in regard to the cost of accessing commercial language services, the processing time and latency, as well as the amount of content that can be provided as context to the models.Therefore, we make the case that we should train future language models using multilingually fair subword tokenizers.

摘要:

即使没有明确训练，最近的语言模型也表现出了令人印象深刻的多语言性能。尽管如此，不同语言的输出质量仍令人担忧。在本文中，我们展示了不同语言的处理差异是如何产生的在标记化阶段，甚至在模型被调用之前。翻译成不同语言的相同文本可能具有截然不同的标记化长度，在某些情况下差异高达 15 倍。即使对于专门训练多语言支持的标记化器，这些差异仍然存在对于某些语言对，字符级和字节级模型的编码长度也存在超过 4 倍的差异。这导致某些语言社区在访问商业语言服务的成本、处理时间和延迟方面受到不公平待遇，以及可以作为模型上下文提供的内容量。因此，我们认为应该使用多语言公平的子词标记器来训练未来的语言模型。

## LLMScore: Unveiling the Power of Large Language Models in Text-to-Image Synthesis Evaluation<sup>poster<sup>

Authors: Yujie Lu, Xianjun Yang, Xiujun Li, Xin Eric Wang, William Yang Wang

Link: [https://neurips.cc/virtual/2023/poster/71821](https://neurips.cc/virtual/2023/poster/71821)

Abstract:

 Existing automatic evaluation on text-to-image synthesis can only provide an image-text matching score, without considering the object-level compositionality, which results in poor correlation with human judgments. In this work, we propose LLMScore, a new framework that offers evaluation scores with multi-granularity compositionality. LLMScore leverages the large language models (LLMs) to evaluate text-to-image models. Initially, it transforms the image into image-level and object-level visual descriptions. Then an evaluation instruction is fed into the LLMs to measure the alignment between the synthesized image and the text, ultimately generating a score accompanied by a rationale. Our substantial analysis reveals the highest correlation of LLMScore with human judgments on a wide range of datasets (Attribute Binding Contrast, Concept Conjunction, MSCOCO, DrawBench, PaintSkills). Notably, our LLMScore achieves Kendall's tau correlation with human evaluations that is 58.8% and 31.2% higher than the commonly-used text-image matching metrics CLIP and BLIP, respectively.

摘要:

 现有的文本到图像合成的自动评估只能提供图像到文本的匹配分数，而没有考虑对象级别的组合性，这导致与人类判断的相关性较差。在这项工作中，我们提出了 LLMScore，这是一个提供多粒度组合性评估分数的新框架。 LLMScore 利用大型语言模型 (LLM) 来评估文本到图像模型。最初，它将图像转换为图像级和对象级视觉描述。然后，将评估指令输入到法学硕士中，以测量合成图像和文本之间的对齐情况，最终生成附有理由的分数。我们的实质性分析揭示了 LLMScore 与人类对各种数据集（属性绑定对比度、概念连接、MSCOCO、DrawBench、PaintSkills）的判断具有最高的相关性。值得注意的是，我们的 LLMScore 实现了 Kendall tau 与人类评估的相关性，分别比常用的文本图像匹配指标 CLIP 和 BLIP 高 58.8% 和 31.2%。

## Joint processing of linguistic properties in brains and language models<sup>poster<sup>

Authors: SUBBAREDDY OOTA, Manish Gupta, Mariya Toneva

Link: [https://neurips.cc/virtual/2023/poster/72702](https://neurips.cc/virtual/2023/poster/72702)

Abstract:

 Language models have been shown to be very effective in predicting brain recordings of subjects experiencing complex language stimuli. For a deeper understanding of this alignment, it is important to understand the correspondence between the detailed processing of linguistic information by the human brain versus language models. We investigate this correspondence via a direct approach, in which we eliminate information related to specific linguistic properties in the language model representations and observe how this intervention affects the alignment with fMRI brain recordings obtained while participants listened to a story. We investigate a range of linguistic properties (surface, syntactic, and semantic) and find that the elimination of each one results in a significant decrease in brain alignment. Specifically, we find that syntactic properties (i.e. Top Constituents and Tree Depth) have the largest effect on the trend of brain alignment across model layers. These findings provide clear evidence for the role of specific linguistic information in the alignment between brain and language models, and open new avenues for mapping the joint information processing in both systems. We make the code publicly available [https://github.com/subbareddy248/linguistic-properties-brain-alignment].

摘要:

语言模型已被证明在预测经历复杂语言刺激的受试者的大脑记录方面非常有效。为了更深入地理解这种一致性，了解人脑与语言模型对语言信息的详细处理之间的对应关系非常重要。我们通过直接方法研究这种对应关系，在该方法中，我们消除了语言模型表示中与特定语言属性相关的信息，并观察这种干预如何影响与参与者听故事时获得的功能磁共振成像大脑记录的一致性。我们研究了一系列语言特性（表面、句法和语义），发现消除每一种特性都会导致大脑排列显着下降。具体来说，我们发现句法属性（即顶级成分和树深度）对跨模型层的大脑对齐趋势影响最大。这些发现为特定语言信息在大脑和语言模型之间的协调中的作用提供了明确的证据，并为绘制两个系统中的联合信息处理开辟了新的途径。我们公开提供代码 [https://github.com/subbareddy248/linguistic-properties-brain-alignment]。

## ToolkenGPT: Augmenting Frozen Language Models with Massive Tools via Tool Embeddings<sup>oral<sup>

Authors: Shibo Hao, Tianyang Liu, Zhen Wang, Zhiting Hu

Link: [https://neurips.cc/virtual/2023/poster/72492](https://neurips.cc/virtual/2023/poster/72492)

Abstract:

 Integrating large language models (LLMs) with various tools has led to increased attention in the field. Existing approaches either involve fine-tuning the LLM, which is both computationally costly and limited to a fixed set of tools, or prompting LLMs by in-context tool demonstrations. Although the latter method offers adaptability to new tools, it struggles with the inherent context length constraint of LLMs when many new tools are presented, and mastering a new set of tools with few-shot examples remains challenging, resulting in suboptimal performance. To address these limitations, we propose a novel solution, named ToolkenGPT, wherein LLMs effectively learn to master tools as predicting tokens through tool embeddings for solving complex tasks. In this framework, each tool is transformed into vector embeddings and plugged into the language model head. Once the function is triggered during text generation, the LLM enters a special function mode to execute the tool calls. Our experiments show that function embeddings effectively help LLMs understand tool use and improve on several tasks, including numerical reasoning, knowledge-based question answering and embodied decision-making.

摘要:

将大型语言模型（LLM）与各种工具集成已经引起了该领域的越来越多的关注。现有的方法要么涉及对法学硕士进行微调，这既需要计算成本高，又仅限于一组固定的工具，要么通过上下文工具演示来提示法学硕士。尽管后一种方法提供了对新工具的适应性，但当出现许多新工具时，它会受到法学硕士固有的上下文长度限制的困扰，并且通过少量示例掌握一组新工具仍然具有挑战性，从而导致性能不佳。为了解决这些限制，我们提出了一种名为 ToolkenGPT 的新颖解决方案，其中法学硕士可以有效地学习掌握工具，通过工具嵌入来预测令牌来解决复杂的任务。在这个框架中，每个工具都被转换为向量嵌入并插入到语言模型头中。一旦在文本生成过程中触发该函数，LLM 就会进入特殊函数模式来执行工具调用。我们的实验表明，函数嵌入有效地帮助法学硕士理解工具的使用并改进多项任务，包括数字推理、基于知识的问答和具体决策。

## LeanDojo: Theorem Proving with Retrieval-Augmented Language Models<sup>oral<sup>

Authors: Kaiyu Yang, Aidan Swope, Alex Gu, Rahul Chalamala, Peiyang Song, Shixing Yu, Saad Godil, Ryan J Prenger, Animashree Anandkumar

Link: [https://neurips.cc/virtual/2023/poster/73510](https://neurips.cc/virtual/2023/poster/73510)

Abstract:

 Large language models (LLMs) have shown promise in proving formal theorems using proof assistants such as Lean. However, existing methods are difficult to reproduce or build on, due to private code, data, and large compute requirements. This has created substantial barriers to research on machine learning methods for theorem proving. This paper removes these barriers by introducing LeanDojo: an open-source Lean playground consisting of toolkits, data, models, and benchmarks. LeanDojo extracts data from Lean and enables interaction with the proof environment programmatically. It contains fine-grained annotations of premises in proofs, providing valuable data for premise selection—a key bottleneck in theorem proving. Using this data, we develop ReProver (Retrieval-Augmented Prover): an LLM-based prover augmented with retrieval for selecting premises from a vast math library. It is inexpensive and needs only one GPU week of training. Our retriever leverages LeanDojo's program analysis capability to identify accessible premises and hard negative examples, which makes retrieval much more effective. Furthermore, we construct a new benchmark consisting of 98,734 theorems and proofs extracted from Lean's math library. It features challenging data split requiring the prover to generalize to theorems relying on novel premises that are never used in training. We use this benchmark for training and evaluation, and experimental results demonstrate the effectiveness of ReProver over non-retrieval baselines and GPT-4. We thus provide the first set of open-source LLM-based theorem provers without any proprietary datasets and release it under a permissive MIT license to facilitate further research.

摘要:

大型语言模型 (LLM) 在使用 Lean 等证明助手证明形式定理方面表现出了良好的前景。然而，由于私有代码、数据和大量计算需求，现有方法很难重现或构建。这给定理证明的机器学习方法的研究造成了巨大的障碍。本文通过介绍 LeanDojo 消除了这些障碍：一个由工具包、数据、模型和基准组成的开源精益游乐场。 LeanDojo 从 Lean 中提取数据，并以编程方式与证明环境进行交互。它包含证明中前提的细粒度注释，为前提选择（定理证明中的关键瓶颈）提供有价值的数据。使用这些数据，我们开发了 ReProver（检索增强证明器）：一种基于 LLM 的证明器，增强了检索功能，用于从庞大的数学库中选择前提。它价格低廉，并且只需要一周的 GPU 训练。我们的检索器利用 LeanDojo 的程序分析功能来识别可访问的前提和困难的负面示例，这使得检索更加有效。此外，我们构建了一个新的基准，其中包含从 Lean 数学库中提取的 98,734 个定理和证明。它具有挑战性的数据分割，要求证明者依赖于训练中从未使用过的新颖前提来推广到定理。我们使用这个基准进行训练和评估，实验结果证明了 ReProver 相对于非检索基线和 GPT-4 的有效性。因此，我们提供了第一套基于开源 LLM 的定理证明器，无需任何专有数据集，并在 MIT 许可下发布，以促进进一步的研究。

## Language Is Not All You Need: Aligning Perception with Language Models<sup>poster<sup>

Authors: Shaohan Huang, Li Dong, Wenhui Wang, Yaru Hao, Saksham Singhal, Shuming Ma, Tengchao Lv, Lei Cui, Owais Khan Mohammed, Barun Patra, Qiang Liu, Kriti Aggarwal, Zewen Chi, Nils Bjorck, Vishrav Chaudhary, Subhojit Som, XIA SONG, Furu Wei

Link: [https://neurips.cc/virtual/2023/poster/71488](https://neurips.cc/virtual/2023/poster/71488)

Abstract:

 A big convergence of language, multimodal perception, action, and world modeling is a key step toward artificial general intelligence. In this work, we introduce KOSMOS-1, a Multimodal Large Language Model (MLLM) that can perceive general modalities, learn in context (i.e., few-shot), and follow instructions (i.e., zero-shot). Specifically, we train KOSMOS-1 from scratch on web-scale multi-modal corpora, including arbitrarily interleaved text and images, image-caption pairs, and text data. We evaluate various settings, including zero-shot, few-shot, and multimodal chain-of-thought prompting, on a wide range of tasks without any gradient updates or finetuning. Experimental results show that KOSMOS-1 achieves impressive performance on (i) language understanding, generation, and even OCR-free NLP (directly fed with document images), (ii) perception-language tasks, including multimodal dialogue, image captioning, visual question answering, and (iii) vision tasks, such as image recognition with descriptions (specifying classification via text instructions). We also show that MLLMs can benefit from cross-modal transfer, i.e., transfer knowledge from language to multimodal, and from multimodal to language. In addition, we introduce a dataset of Raven IQ test, which diagnoses the nonverbal reasoning capability of MLLMs.

摘要:

语言、多模态感知、行动和世界建模的大融合是迈向通用人工智能的关键一步。在这项工作中，我们介绍了 KOSMOS-1，一种多模态大型语言模型 (MLLM)，它可以感知一般模态、在上下文中学习（即少样本）并遵循指令（即零样本）。具体来说，我们在网络规模的多模态语料库上从头开始训练 KOSMOS-1，包括任意交错的文本和图像、图像标题对和文本数据。我们在没有任何梯度更新或微调的情况下，在广泛的任务中评估各种设置，包括零样本、少样本和多模式思维链提示。实验结果表明，KOSMOS-1 在以下方面取得了令人印象深刻的性能：(i) 语言理解、生成，甚至无需 OCR 的 NLP（直接输入文档图像），(ii) 感知语言任务，包括多模态对话、图像字幕、视觉问题回答，以及（iii）视觉任务，例如带有描述的图像识别（通过文本指令指定分类）。我们还表明，MLLM 可以从跨模式转移中受益，即将知识从语言转移到多模式，以及从多模式转移到语言。此外，我们还引入了 Raven IQ 测试数据集，用于诊断 MLLM 的非语言推理能力。

## Is Your Code Generated by ChatGPT Really Correct? Rigorous Evaluation of Large Language Models for Code Generation<sup>poster<sup>

Authors: Jiawei Liu, Chunqiu Steven Xia, Yuyao Wang, LINGMING ZHANG

Link: [https://neurips.cc/virtual/2023/poster/72990](https://neurips.cc/virtual/2023/poster/72990)

Abstract:

 Program synthesis has been long studied with recent approaches focused on directly using the power of Large Language Models (LLMs) to generate code. Programming benchmarks, with curated synthesis problems and test-cases, are used to measure the performance of various LLMs on code synthesis. However, these test-cases can be limited in both quantity and quality for fully assessing the functional correctness of the generated code. Such limitation in the existing benchmarks begs the following question: In the era of LLMs, is the code generated really correct? To answer this, we propose EvalPlus – a code synthesis evaluation framework to rigorously benchmark the functional correctness of LLM-synthesized code. EvalPlus augments a given evaluation dataset with large amounts of test-cases newly produced by an automatic test input generator, powered by both LLM- and mutation-based strategies. While EvalPlus is general, we extend the test-cases of the popular HumanEval benchmark by 80x to build HumanEval+. Our extensive evaluation across 26 popular LLMs (e.g., GPT-4 and ChatGPT) demonstrates that HumanEval+ is able to catch significant amounts of previously undetected wrong code synthesized by LLMs, reducing the pass@k by up-to 19.3-28.9%. We also surprisingly found that test insufficiency can lead to mis-ranking. For example, both WizardCoder-CodeLlama and Phind-CodeLlama now outperform ChatGPT on HumanEval+, while none of them could on HumanEval. Our work not only indicates that prior popular code synthesis evaluation results do not accurately reflect the true performance of LLMs for code synthesis, but also opens up a new direction to improve such programming benchmarks through automated testing. We have open-sourced our tools, enhanced datasets as well as all LLM-generated code at https://github.com/evalplus/evalplus to facilitate and accelerate future LLM-for-code research.

摘要:

程序综合已经被研究了很长时间，最近的方法主要集中于直接使用大型语言模型（LLM）的功能来生成代码。编程基准以及精选的综合问题和测试用例用于衡量各种法学硕士在代码综合方面的表现。然而，这些测试用例在数量和质量上都受到限制，无法充分评估生成代码的功能正确性。现有基准测试中的这种限制引出了以下问题：在LLM时代，生成的代码真的正确吗？为了回答这个问题，我们提出了 EvalPlus——一个代码综合评估框架，用于严格基准测试 LLM 综合代码的功能正确性。 EvalPlus 使用自动测试输入生成器新生成的大量测试用例来增强给定的评估数据集，并由基于 LLM 和基于突变的策略提供支持。虽然 EvalPlus 很通用，但我们将流行的 HumanEval 基准测试用例扩展了 80 倍来构建 HumanEval+。我们对 26 个流行的 LLM（例如 GPT-4 和 ChatGPT）进行的广泛评估表明，HumanEval+ 能够捕获 LLM 合成的大量以前未检测到的错误代码，将 pass@k 减少高达 19.3-28.9%。我们还令人惊讶地发现测试不充分可能导致排名错误。例如，WizardCoder-CodeLlama 和 Phind-CodeLlama 现在在 HumanEval+ 上的性能都优于 ChatGPT，而在 HumanEval 上它们都无法做到。我们的工作不仅表明之前流行的代码综合评估结果并不能准确反映LLM在代码综合方面的真实性能，而且还为通过自动化测试改进此类编程基准开辟了新的方向。我们在 https://github.com/evalplus/evalplus 上开源了我们的工具、增强的数据集以及所有 LLM 生成的代码，以促进和加速未来的 LLM-for-code 研究。

## Aligning Language Models with Human Preferences via a Bayesian Approach<sup>poster<sup>

Authors: Jiashuo WANG, Haozhao Wang, Shichao Sun, Wenjie Li

Link: [https://neurips.cc/virtual/2023/poster/72170](https://neurips.cc/virtual/2023/poster/72170)

Abstract:

 In the quest to advance human-centric natural language generation (NLG) systems, ensuring alignment between NLG models and human preferences is crucial. For this alignment, current popular methods leverage a reinforcement learning (RL) approach with a reward model trained on feedback from humans. However, inherent disagreements due to the subjective nature of human preferences pose a significant challenge for training the reward model, resulting in a deterioration of the NLG performance. To tackle this issue, previous approaches typically rely on majority voting or averaging to consolidate multiple inconsistent preferences into a merged one. Although straightforward to understand and execute, such methods suffer from an inability to capture the nuanced degrees of disaggregation among humans and may only represent a specialized subset of individuals, thereby lacking the ability to quantitatively disclose the universality of human preferences. To address this challenge, this paper proposes a novel approach, which employs a Bayesian framework to account for the distribution of disagreements among human preferences as training a preference model, and names it as $\textbf{d-PM}$. Besides, considering the RL strategy's inefficient and complex training process over the training efficiency, we further propose utilizing the contrastive learning strategy to train the NLG model with the preference scores derived from the d-PM model. Extensive experiments on two human-centric NLG tasks, i.e., emotional support conversation and integrity ``Rule-of-Thumb'' generation, show that our method consistently exceeds previous SOTA models in both automatic and human evaluations.

摘要:

在寻求推进以人类为中心的自然语言生成（NLG）系统时，确保 NLG 模型与人类偏好之间的一致性至关重要。为了实现这种一致性，当前流行的方法利用强化学习（RL）方法和根据人类反馈进行训练的奖励模型。然而，由于人类偏好的主观性质而产生的固有分歧给奖励模型的训练带来了重大挑战，导致 NLG 性能恶化。为了解决这个问题，以前的方法通常依靠多数投票或平均来将多个不一致的偏好合并为一个合并的偏好。尽管易于理解和执行，但此类方法无法捕捉人类之间的细微差别，并且可能仅代表个体的特定子集，因此缺乏定量揭示人类偏好的普遍性的能力。为了应对这一挑战，本文提出了一种新颖的方法，采用贝叶斯框架来解释人类偏好之间的分歧分布，并训练偏好模型，并将其命名为 $\textbf{d-PM}$。此外，考虑到强化学习策略的训练过程效率低下且复杂，我们进一步建议利用对比学习策略利用从 d-PM 模型得出的偏好分数来训练 NLG 模型。对两个以人为中心的 NLG 任务（即情感支持对话和完整性“经验法则”生成）进行的广泛实验表明，我们的方法在自动评估和人类评估方面始终优于以前的 SOTA 模型。

## ChessGPT: Bridging Policy Learning and Language Modeling<sup>poster<sup>

Authors: Xidong Feng, Yicheng Luo, Ziyan Wang, Hongrui Tang, Mengyue Yang, Kun Shao, David Mguni, Yali Du, Jun Wang

Link: [https://neurips.cc/virtual/2023/poster/73461](https://neurips.cc/virtual/2023/poster/73461)

Abstract:

 When solving decision-making tasks, humans typically depend on information from two key sources: (1) Historical policy data, which provides interaction replay from the environment, and (2) Analytical insights in natural language form, exposing the invaluable thought process or strategic considerations. Despite this, the majority of preceding research focuses on only one source: they either use historical replay exclusively to directly learn policy or value functions, or engaged in language model training utilizing mere language corpus. In this paper, we argue that a powerful autonomous agent should cover both sources. Thus, we propose ChessGPT, a GPT model bridging policy learning and language modeling by integrating data from these two sources in Chess games. Specifically, we build a large-scale game and language dataset related to chess. Leveraging the dataset, we showcase two model examples ChessCLIP and ChessGPT, integrating policy learning and language modeling. Finally, we propose a full evaluation framework for evaluating language model's chess ability. Experimental results validate our model and dataset's effectiveness. We open source our code, model, and dataset at https://github.com/waterhorse1/ChessGPT.

摘要:

在解决决策任务时，人类通常依赖于两个关键来源的信息：（1）历史政策数据，提供来自环境的交互回放；（2）自然语言形式的分析见解，揭示宝贵的思维过程或战略考虑。尽管如此，大多数先前的研究只关注一个来源：他们要么专门使用历史重播来直接学习政策或价值函数，要么仅利用语言语料库进行语言模型训练。在本文中，我们认为强大的自主代理应该涵盖这两个来源。因此，我们提出了 ChessGPT，这是一种通过集成国际象棋游戏中这两个来源的数据来桥接策略学习和语言建模的 GPT 模型。具体来说，我们构建了一个与国际象棋相关的大型游戏和语言数据集。利用该数据集，我们展示了两个模型示例 ChessCLIP 和 ChessGPT，集成了策略学习和语言建模。最后，我们提出了一个完整的评估框架来评估语言模型的国际象棋能力。实验结果验证了我们的模型和数据集的有效性。我们在 https://github.com/waterhorse1/ChessGPT 开源我们的代码、模型和数据集。

## Using Imperfect Surrogates for Downstream Inference: Design-based Supervised Learning for Social Science Applications of Large Language Models<sup>poster<sup>

Authors: Naoki Egami, Musashi Hinck, Brandon Stewart, Hanying Wei

Link: [https://neurips.cc/virtual/2023/poster/70979](https://neurips.cc/virtual/2023/poster/70979)

Abstract:

 In computational social science (CSS), researchers analyze documents to explain social and political phenomena. In most scenarios, CSS researchers first obtain labels for documents and then explain labels using interpretable regression analyses in the second step. One increasingly common way to annotate documents cheaply at scale is through large language models (LLMs). However, like other scalable ways of producing annotations, such surrogate labels are often imperfect and biased. We present a new algorithm for using imperfect annotation surrogates for downstream statistical analyses while guaranteeing statistical properties—like asymptotic unbiasedness and proper uncertainty quantification—which are fundamental to CSS research. We show that direct use of surrogate labels in downstream statistical analyses leads to substantial bias and invalid confidence intervals, even with high surrogate accuracy of 80-90\%. To address this, we build on debiased machine learning to propose the design-based supervised learning (DSL) estimator. DSL employs a doubly-robust procedure to combine surrogate labels with a smaller number of high-quality, gold-standard labels. Our approach guarantees valid inference for downstream statistical analyses, even when surrogates are arbitrarily biased and without requiring stringent assumptions, by controlling the probability of sampling documents for gold-standard labeling. Both our theoretical analysis and experimental results show that DSL provides valid statistical inference while achieving root mean squared errors comparable to existing alternatives that focus only on prediction without inferential guarantees.

摘要:

在计算社会科学（CSS）中，研究人员分析文档来解释社会和政治现象。在大多数情况下，CSS 研究人员首先获取文档的标签，然后在第二步中使用可解释的回归分析来解释标签。一种日益常见的大规模廉价注释文档的方法是通过大型语言模型 (LLM)。然而，与其他生成注释的可扩展方式一样，此类替代标签通常是不完美且有偏见的。我们提出了一种新算法，使用不完美的注释替代项进行下游统计分析，同时保证统计特性（例如渐近无偏性和适当的不确定性量化），这些特性是 CSS 研究的基础。我们表明，在下游统计分析中直接使用替代标签会导致很大的偏差和无效的置信区间，即使替代准确度高达 80-90%。为了解决这个问题，我们在去偏机器学习的基础上提出了基于设计的监督学习（DSL）估计器。 DSL 采用双重鲁棒程序将代理标签与少量高质量、黄金标准标签相结合。我们的方法通过控制黄金标准标签的抽样文档的概率，保证下游统计分析的有效推断，即使替代者有任意偏见并且不需要严格的假设。我们的理论分析和实验结果都表明，DSL 提供了有效的统计推断，同时实现了与仅注重预测而没有推断保证的现有替代方案相当的均方根误差。

## Extensible Prompts for Language Models on Zero-shot Language Style Customization<sup>poster<sup>

Authors: Tao Ge, Hu Jing, Li Dong, Shaoguang Mao, Yan Xia, Xun Wang, Si-Qing Chen, Furu Wei

Link: [https://neurips.cc/virtual/2023/poster/70594](https://neurips.cc/virtual/2023/poster/70594)

Abstract:

 We propose eXtensible Prompt (X-Prompt) for prompting a large language model (LLM) beyond natural language (NL). X-Prompt instructs an LLM with not only NL but also an extensible vocabulary of imaginary words. Registering new imaginary words allows us to instruct the LLM to comprehend concepts that are difficult to describe with NL words, thereby making a prompt more descriptive. Also, these imaginary words are designed to be out-of-distribution (OOD) robust so that they can be (re)used like NL words in various prompts, distinguishing X-Prompt from soft prompt that is for fitting in-distribution data. We propose context-augmented learning (CAL) to learn imaginary words for general usability, enabling them to work properly in OOD (unseen) prompts. We experiment X-Prompt for zero-shot language style customization as a case study. The promising results of X-Prompt demonstrate its potential to facilitate advanced interaction beyond the natural language interface, bridging the communication gap between humans and LLMs.

摘要:

我们提出了可扩展提示（X-Prompt），用于提示超越自然语言（NL）的大型语言模型（LLM）。 X-Prompt 不仅教授法学硕士 NL，还教授可扩展的想象词汇词汇。注册新的虚构单词使我们能够指导法学硕士理解难以用 NL 单词描述的概念，从而使提示更具描述性。此外，这些虚构单词被设计为分布外 (OOD) 鲁棒性，以便它们可以在各种提示中像 NL 单词一样（重新）使用，从而将 X-Prompt 与用于拟合分布内数据的软提示区分开来。我们提出上下文增强学习（CAL）来学习虚构单词以实现一般可用性，使它们能够在 OOD（看不见的）提示中正常工作。我们将 X-Prompt 进行零样本语言风格定制实验作为案例研究。 X-Prompt 令人鼓舞的结果证明了其促进超越自然语言界面的高级交互的潜力，弥合了人类和法学硕士之间的沟通差距。

## LLM-Pruner: On the Structural Pruning of Large Language Models<sup>poster<sup>

Authors: Xinyin Ma, Gongfan Fang, Xinchao Wang

Link: [https://neurips.cc/virtual/2023/poster/72074](https://neurips.cc/virtual/2023/poster/72074)

Abstract:

 Large language models (LLMs) have shown remarkable capabilities in language understanding and generation. However, such impressive capability typically comes with a substantial model size, which presents significant challenges in both the deployment, inference, and training stages. With LLM being a general-purpose task solver, we explore its compression in a task-agnostic manner, which aims to preserve the multi-task solving and language generation ability of the original LLM. One challenge to achieving this is the enormous size of the training corpus of LLM, which makes both data transfer and model post-training over-burdensome. Thus, we tackle the compression of LLMs within the bound of two constraints: being task-agnostic and minimizing the reliance on the original training dataset. Our method, named LLM-pruner, adopts structural pruning that selectively removes non-critical coupled structures based on gradient information, maximally preserving the majority of the LLM's functionality. To this end, the performance of pruned models can be efficiently recovered through tuning techniques, LoRA, in merely 3 hours, requiring only 50K data. We validate the LLM-Pruner on three LLMs, including LLaMA, Vicuna, and ChatGLM, and demonstrate that the compressed models still exhibit satisfactory capabilities in zero-shot classification and generation. The code will be made public.

摘要:

大型语言模型（LLM）在语言理解和生成方面表现出了卓越的能力。然而，如此令人印象深刻的能力通常伴随着巨大的模型大小，这在部署、推理和训练阶段都带来了巨大的挑战。由于LLM是通用任务求解器，我们以任务无关的方式探索其压缩，旨在保留原始LLM的多任务求解和语言生成能力。实现这一目标的一个挑战是法学硕士的训练语料库规模巨大，这使得数据传输和模型后训练都变得过于繁重。因此，我们在两个约束的范围内解决法学硕士的压缩问题：与任务无关并最大限度地减少对原始训练数据集的依赖。我们的方法名为LLM-pruner，采用结构剪枝，根据梯度信息选择性地去除非关键耦合结构，最大限度地保留LLM的大部分功能。为此，通过调优技术LoRA，仅需3小时，仅需要50K数据，即可有效恢复剪枝模型的性能。我们在 LLaMA、Vicuna 和 ChatGLM 等三个 LLM 上验证了 LLM-Pruner，并证明压缩模型在零样本分类和生成方面仍然表现出令人满意的能力。该代码将被公开。

## Large Language Models Are Zero-Shot Time Series Forecasters<sup>poster<sup>

Authors: Nate Gruver, Marc Finzi, Shikai Qiu, Andrew Wilson

Link: [https://neurips.cc/virtual/2023/poster/70543](https://neurips.cc/virtual/2023/poster/70543)

Abstract:

 By encoding time series as a string of numerical digits, we can frame time series forecasting as next-token prediction in text. Developing this approach, we find that large language models (LLMs) such as GPT-3 and LLaMA-2 can surprisingly zero-shot extrapolate time series at a level comparable to or exceeding the performance of purpose-built time series models trained on the downstream tasks. To facilitate this performance, we propose procedures for effectively tokenizing time series data and converting discrete distributions over tokens into highly flexible densities over continuous values. We argue the success of LLMs for time series stems from their ability to naturally represent multimodal distributions, in conjunction with biases for simplicity, and repetition, which align with the salient features in many time series, such as repeated seasonal trends. We also show how LLMs can naturally handle missing data without imputation through non-numerical text, accommodate textual side information, and answer questions to help explain predictions.  While we find that increasing model size generally improves performance on time series, we show GPT-4 can perform worse than GPT-3 because of how it tokenizes numbers, and poor uncertainty calibration, which is likely the result of alignment interventions such as RLHF.

摘要:

通过将时间序列编码为一串数字，我们可以将时间序列预测框架为文本中的下一个标记预测。通过开发这种方法，我们发现 GPT-3 和 LLaMA-2 等大型语言模型 (LLM) 可以令人惊讶地以零样本推断时间序列，其水平相当于或超过在下游训练的专用时间序列模型的性能任务。为了促进这种性能，我们提出了有效标记时间序列数据并将标记上的离散分布转换为连续值上的高度灵活的密度的程序。我们认为时间序列法学硕士的成功源于它们自然地表示多模态分布的能力，再加上简单性和重复性的偏差，这与许多时间序列中的显着特征相一致，例如重复的季节性趋势。我们还展示了法学硕士如何自然地处理缺失数据，而无需通过非数字文本进行插补，容纳文本辅助信息，并回答问题以帮助解释预测。虽然我们发现增加模型大小通常会提高时间序列的性能，但我们表明 GPT-4 的性能可能比 GPT-3 差，因为它对数字进行标记的方式以及较差的不确定性校准，这可能是 RLHF 等对齐干预的结果。

## Meta-Adapter: An Online Few-shot Learner for Vision-Language Model<sup>poster<sup>

Authors: cheng cheng, Lin Song, Ruoyi Xue, Hang Wang, Hongbin Sun, Yixiao Ge, Ying Shan

Link: [https://neurips.cc/virtual/2023/poster/71536](https://neurips.cc/virtual/2023/poster/71536)

Abstract:

 The contrastive vision-language pre-training, known as CLIP, demonstrates remarkable potential in perceiving open-world visual concepts, enabling effective zero-shot image recognition.  Nevertheless, few-shot learning methods based on CLIP typically require offline fine-tuning of the parameters on few-shot samples, resulting in longer inference time and the risk of overfitting in certain domains.  To tackle these challenges, we propose the Meta-Adapter, a lightweight residual-style adapter, to refine the CLIP features guided by the few-shot samples in an online manner.  With a few training samples, our method can enable effective few-shot learning capabilities and generalize to unseen data or tasks without additional fine-tuning, achieving competitive performance and high efficiency.  Without bells and whistles, our approach outperforms the state-of-the-art online few-shot learning method by an average of 3.6\% on eight image classification datasets with higher inference speed.  Furthermore, our model is simple and flexible, serving as a plug-and-play module directly applicable to downstream tasks.  Without further fine-tuning, Meta-Adapter obtains notable performance improvements in open-vocabulary object detection and segmentation tasks.

摘要:

对比视觉语言预训练（称为 CLIP）在感知开放世界视觉概念、实现有效的零样本图像识别方面表现出巨大的潜力。然而，基于CLIP的少样本学习方法通常需要对少样本样本上的参数进行离线微调，导致推理时间更长，并且在某些领域存在过拟合的风险。为了应对这些挑战，我们提出了 Meta-Adapter，一种轻量级残差式适配器，以在线方式细化由少量样本引导的 CLIP 特征。通过一些训练样本，我们的方法可以实现有效的小样本学习能力，并泛化到未见过的数据或任务，而无需额外的微调，从而实现有竞争力的性能和高效率。没有花里胡哨的东西，我们的方法在八个图像分类数据集上以更高的推理速度平均优于最先进的在线少样本学习方法 3.6%。此外，我们的模型简单灵活，作为即插即用模块直接适用于下游任务。无需进一步微调，Meta-Adapter 在开放词汇对象检测和分割任务中获得显着的性能改进。

## AdaPlanner: Adaptive Planning from Feedback with Language Models<sup>poster<sup>

Authors: Haotian Sun, Yuchen Zhuang, Lingkai Kong, Bo Dai, Chao Zhang

Link: [https://neurips.cc/virtual/2023/poster/70298](https://neurips.cc/virtual/2023/poster/70298)

Abstract:

 Large language models (LLMs) have recently demonstrated the potential in acting as autonomous agents for sequential decision-making tasks. However, most existing methods either take actions greedily without planning or rely on static plans that are not adaptable to environmental feedback. Consequently, the sequential decision-making performance of LLM agents degenerates with problem complexity and plan horizons increase. We propose a closed-loop approach, AdaPlanner, which allows the LLM agent to refine its self-generated plan adaptively in response to environmental feedback. In AdaPlanner, the LLM agent adaptively refines its plan from feedback with both in-plan and out-of-plan refinement strategies. To mitigate hallucination, we develop a code-style LLM prompt structure that facilitates plan generation across a variety of tasks, environments, and agent capabilities. Furthermore, we propose a skill discovery mechanism that leverages successful plans as few-shot exemplars, enabling the agent to plan and refine with fewer task demonstrations. Our experiments in the ALFWorld and MiniWoB++ environments demonstrate that AdaPlanner outperforms state-of-the-art baselines by 3.73% and 4.11% while utilizing 2x and 600x fewer samples, respectively. The implementation of AdaPlanner is available at https://github.com/haotiansun14/AdaPlanner.

摘要:

大型语言模型（LLM）最近证明了作为顺序决策任务的自主代理的潜力。然而，大多数现有方法要么在没有计划的情况下贪婪地采取行动，要么依赖于不适应环境反馈的静态计划。因此，LLM 代理的顺序决策性能随着问题复杂性和计划范围的增加而退化。我们提出了一种闭环方法 AdaPlanner，它允许 LLM 代理根据环境反馈自适应地完善其自行生成的计划。在 AdaPlanner 中，LLM 代理通过计划内和计划外细化策略根据反馈自适应地细化其计划。为了减轻幻觉，我们开发了一种代码式的 LLM 提示结构，有助于跨各种任务、环境和代理功能生成计划。此外，我们提出了一种技能发现机制，利用成功的计划作为少数样本，使代理能够通过更少的任务演示来计划和完善。我们在 ALFWorld 和 MiniWoB++ 环境中的实验表明，AdaPlanner 的性能比最先进的基线高出 3.73% 和 4.11%，同时使用的样本数量分别减少了 2 倍和 600 倍。 AdaPlanner 的实现可以在 https://github.com/haotiansun14/AdaPlanner 获取。

## Evaluating Cognitive Maps and Planning in Large Language Models with CogEval<sup>poster<sup>

Authors: Ida Momennejad, Hosein Hasanbeig, Felipe Vieira Frujeri, Hiteshi Sharma, Nebojsa Jojic, Hamid Palangi, Robert Ness, Jonathan Larson

Link: [https://neurips.cc/virtual/2023/poster/71431](https://neurips.cc/virtual/2023/poster/71431)

Abstract:

 Recently an influx of studies claims emergent cognitive abilities in large language models (LLMs). Yet, most rely on anecdotes, overlook contamination of training sets, or lack systematic Evaluation involving multiple tasks, control conditions, multiple iterations, and statistical robustness tests. Here we make two major contributions. First, we propose CogEval, a cognitive science-inspired protocol for the systematic evaluation of cognitive capacities in LLMs. The CogEval protocol can be followed for the evaluation of various abilities. Second, here we follow CogEval to systematically evaluate cognitive maps and planning ability across eight LLMs (OpenAI GPT-4, GPT-3.5-turbo-175B, davinci-003-175B, Google Bard, Cohere-xlarge-52.4B, Anthropic Claude-1-52B, LLaMA-13B, and Alpaca-7B). We base our task prompts on human experiments, which offer both established construct validity for evaluating planning, and are absent from LLM training sets. We find that, while LLMs show apparent competence in a few planning tasks with simpler structures, systematic evaluation reveals striking failure modes in planning tasks, including hallucinations of invalid trajectories and falling in loops. These findings do not support the idea of emergent out-of-the-box planning ability in LLMs. This could be because LLMs do not understand the latent relational structures underlying planning problems, known as cognitive maps, and fail at unrolling goal-directed trajectories based on the underlying structure. Implications for application and future directions are discussed.

摘要:

最近大量研究声称大语言模型（LLM）具有新兴的认知能力。然而，大多数依赖于轶事，忽视了训练集的污染，或者缺乏涉及多个任务、控制条件、多次迭代和统计稳健性测试的系统评估。在这里我们做出了两个主要贡献。首先，我们提出 CogEval，这是一种受认知科学启发的协议，用于系统评估法学硕士的认知能力。可以遵循CogEval协议来评估各种能力。其次，在这里我们按照 CogEval 系统地评估八个 LLM 的认知图和规划能力（OpenAI GPT-4、GPT-3.5-turbo-175B、davinci-003-175B、Google Bard、Cohere-xlarge-52.4B、Anthropic Claude- 1-52B、LLaMA-13B 和 Alpaca-7B）。我们的任务提示基于人体实验，这既提供了评估计划的既定结构有效性，又不存在于法学硕士培训集中。我们发现，虽然法学硕士在一些结构较简单的规划任务中表现出明显的能力，但系统评估揭示了规划任务中惊人的失败模式，包括无效轨迹的幻觉和陷入循环。这些发现并不支持法学硕士具有现成的计划能力的想法。这可能是因为法学硕士不理解规划问题背后的潜在关系结构（称为认知图），并且无法根据底层结构展开目标导向的轨迹。讨论了应用的影响和未来的方向。

## Symbol-LLM: Leverage Language Models for Symbolic System in Visual Human Activity Reasoning<sup>poster<sup>

Authors: Xiaoqian Wu, Yong-Lu Li, Jianhua Sun, Cewu Lu

Link: [https://neurips.cc/virtual/2023/poster/71665](https://neurips.cc/virtual/2023/poster/71665)

Abstract:

 Human reasoning can be understood as a cooperation between the intuitive, associative "System-1'' and the deliberative, logical "System-2''. For existing System-1-like methods in visual activity understanding, it is crucial to integrate System-2 processing to improve explainability, generalization, and data efficiency. One possible path of activity reasoning is building a symbolic system composed of symbols and rules, where one rule connects multiple symbols, implying human knowledge and reasoning abilities.Previous methods have made progress, but are defective with limited symbols from handcraft and limited rules from visual-based annotations, failing to cover the complex patterns of activities and lacking compositional generalization. To overcome the defects, we propose a new symbolic system with two ideal important properties: broad-coverage symbols and rational rules. Collecting massive human knowledge via manual annotations is expensive to instantiate this symbolic system. Instead, we leverage the recent advancement of LLMs (Large Language Models) as an approximation of the two ideal properties, i.e., Symbols from Large Language Models (Symbol-LLM). Then, given an image, visual contents from the images are extracted andchecked as symbols and activity semantics are reasoned out based on rules via fuzzy logic calculation.Our method shows superiority in extensive activity understanding tasks. Code and data are available at https://mvig-rhos.com/symbol_llm.

摘要:

人类推理可以理解为直觉的、联想的“系统 1”和深思熟虑的、逻辑的“系统 2”之间的合作。对于视觉活动理解中现有的类似 System-1 的方法，集成 System-2 处理以提高可解释性、泛化性和数据效率至关重要。活动推理的一种可能路径是建立一个由符号和规则组成的符号系统，一个规则连接多个符号，暗示着人类的知识和推理能力。以前的方法已经取得了进展，但存在缺陷，手工制作的符号有限，视觉的规则有限。基于注释，未能涵盖复杂的活动模式并且缺乏组合概括。为了克服这些缺陷，我们提出了一种新的符号系统，它具有两个理想的重要属性：广泛覆盖的符号和理性的规则。通过手动注释收集大量人类知识来实例化这个符号系统的成本很高。相反，我们利用 LLM（大型语言模型）的最新进展作为两个理想属性的近似，即来自大型语言模型的符号（Symbol-LLM）。然后，给定图像，从图像中提取视觉内容并进行检查，并通过模糊逻辑计算根据规则推理出活动语义。我们的方法在广泛的活动理解任务中显示出优越性。代码和数据可在 https://mvig-rhos.com/symbol_llm 获取。

## Lexinvariant Language Models<sup>poster<sup>

Authors: Qian Huang, Eric Zelikman, Sarah Chen, Yuhuai Wu, Gregory Valiant, Percy Liang

Link: [https://neurips.cc/virtual/2023/poster/71847](https://neurips.cc/virtual/2023/poster/71847)

Abstract:

 Token embeddings, a mapping from discrete lexical symbols to continuous vectors, are at the heart of any language model (LM). However, lexical symbol meanings can also be determined and even redefined by their structural role in a long context. In this paper, we ask: is it possible for a language model to be performant without \emph{any} fixed token embeddings? Such a language model would have to rely entirely on the co-occurence and repetition of tokens in the context rather than the \textit{a priori} identity of any token. To answer this, we study \textit{lexinvariant}language models that are invariant to lexical symbols and therefore do not need fixed token embeddings in practice. First, we prove that we can construct a lexinvariant LM to converge to the true language model at a uniform rate that is polynomial in terms of the context length, with a constant factor that is sublinear in the vocabulary size. Second, to build a lexinvariant LM, we simply encode tokens using random Gaussian vectors, such that each token maps to the same representation within each sequence but different representations across sequences. Empirically, we demonstrate that it can indeed attain perplexity comparable to that of a standard language model, given a sufficiently long context. We further explore two properties of the lexinvariant language models: First, given text generated from a substitution cipher of English, it implicitly implements Bayesian in-context deciphering and infers the mapping to the underlying real tokens with high accuracy. Second, it has on average 4X better accuracy over synthetic in-context reasoning tasks. Finally, we discuss regularizing standard language models towards lexinvariance and potential practical applications.

摘要:

标记嵌入是从离散词汇符号到连续向量的映射，是任何语言模型 (LM) 的核心。然而，词汇符号的含义也可以通过它们在长上下文中的结构作用来确定甚至重新定义。在本文中，我们问：语言模型是否有可能在没有 \emph{any} 固定标记嵌入的情况下保持高性能？这样的语言模型必须完全依赖于上下文中标记的共现和重复，而不是任何标记的 \textit{先验} 身份。为了回答这个问题，我们研究了 \textit{lexinvariant} 语言模型，这些模型对于词汇符号是不变的，因此在实践中不需要固定的标记嵌入。首先，我们证明我们可以构造一个词法变量 LM，以上下文长度的多项式统一速率收敛到真实的语言模型，常数因子在词汇大小上呈次线性。其次，为了构建词法变量 LM，我们只需使用随机高斯向量对标记进行编码，以便每个标记映射到每个序列内的相同表示，但映射到序列之间的不同表示。根据经验，我们证明，在足够长的上下文中，它确实可以达到与标准语言模型相当的复杂性。我们进一步探索词法变量语言模型的两个属性：首先，给定从英语替换密码生成的文本，它隐式实现贝叶斯上下文解密，并高精度地推断到底层真实标记的映射。其次，它的准确度平均比综合上下文推理任务高出 4 倍。最后，我们讨论针对词法变化和潜在的实际应用正则化标准语言模型。

## InstructBLIP: Towards General-purpose Vision-Language Models with Instruction Tuning<sup>poster<sup>

Authors: Wenliang Dai, Junnan Li, DONGXU LI, Anthony Meng Huat Tiong, Junqi Zhao, Weisheng Wang, Boyang Li, Pascale N Fung, Steven Hoi

Link: [https://neurips.cc/virtual/2023/poster/70085](https://neurips.cc/virtual/2023/poster/70085)

Abstract:

 Large-scale pre-training and instruction tuning have been successful at creating general-purpose language models with broad competence. However, building general-purpose vision-language models is challenging due to the rich input distributions and task diversity resulting from the additional visual input. Although vision-language pretraining has been widely studied, vision-language instruction tuning remains under-explored. In this paper, we conduct a systematic and comprehensive study on vision-language instruction tuning based on the pretrained BLIP-2 models. We gather 26 publicly available datasets, covering a wide variety of tasks and capabilities, and transform them into instruction tuning format. Additionally, we introduce an instruction-aware Query Transformer, which extracts informative features tailored to the given instruction. Trained on 13 held-in datasets, InstructBLIP attains state-of-the-art zero-shot performance across all 13 held-out datasets, substantially outperforming BLIP-2 and larger Flamingo models. Our models also lead to state-of-the-art performance when finetuned on individual downstream tasks (e.g., 90.7% accuracy on ScienceQA questions with image contexts). Furthermore, we qualitatively demonstrate the advantages of InstructBLIP over concurrent multimodal models. All InstructBLIP models are open-source.

摘要:

大规模预训练和指令调整已成功创建具有广泛能力的通用语言模型。然而，由于额外的视觉输入导致丰富的输入分布和任务多样性，构建通用视觉语言模型具有挑战性。尽管视觉语言预训练已被广泛研究，但视觉语言指令调整仍待探索。在本文中，我们基于预训练的 BLIP-2 模型对视觉语言指令调优进行了系统、全面的研究。我们收集了 26 个公开可用的数据集，涵盖各种任务和功能，并将它们转换为指令调优格式。此外，我们引入了一个指令感知查询转换器，它提取适合给定指令的信息特征。 InstructBLIP 在 13 个保留数据集上进行训练，在所有 13 个保留数据集上实现了最先进的零样本性能，大大优于 BLIP-2 和更大的 Flamingo 模型。当对各个下游任务进行微调时，我们的模型也能带来最先进的性能（例如，带有图像上下文的 ScienceQA 问题的准确率为 90.7%）。此外，我们定性地证明了 InstructBLIP 相对于并发多模态模型的优势。所有 InstructBLIP 模型都是开源的。

## LayoutPrompter: Awaken the Design Ability of Large Language Models<sup>poster<sup>

Authors: Jiawei Lin, Jiaqi Guo, Shizhao Sun, Zijiang Yang, Jian-Guang Lou, Dongmei Zhang

Link: [https://neurips.cc/virtual/2023/poster/72326](https://neurips.cc/virtual/2023/poster/72326)

Abstract:

 Conditional graphic layout generation, which automatically maps user constraints to high-quality layouts, has attracted widespread attention today. Although recent works have achieved promising performance, the lack of versatility and data efficiency hinders their practical applications. In this work, we propose LayoutPrompter, which leverages large language models (LLMs) to address the above problems through in-context learning. LayoutPrompter is made up of three key components, namely input-output serialization, dynamic exemplar selection and layout ranking. Specifically, the input-output serialization component meticulously designs the input and output formats for each layout generation task. Dynamic exemplar selection is responsible for selecting the most helpful prompting exemplars for a given input. And a layout ranker is used to pick the highest quality layout from multiple outputs of LLMs. We conduct experiments on all existing layout generation tasks using four public datasets. Despite the simplicity of our approach, experimental results show that LayoutPrompter can compete with or even outperform state-of-the-art approaches on these tasks without any model training or fine-tuning. This demonstrates the effectiveness of this versatile and training-free approach. In addition, the ablation studies show that LayoutPrompter is significantly superior to the training-based baseline in a low-data regime, further indicating the data efficiency of LayoutPrompter. Our project is available at https://github.com/microsoft/LayoutGeneration/tree/main/LayoutPrompter.

摘要:

条件图形布局生成，可自动将用户约束映射到高质量布局，如今引起了广泛关注。尽管最近的工作取得了有希望的性能，但通用性和数据效率的缺乏阻碍了它们的实际应用。在这项工作中，我们提出了 LayoutPrompter，它利用大型语言模型（LLM）通过上下文学习来解决上述问题。 LayoutPrompter由三个关键组件组成，即输入输出序列化、动态示例选择和布局排序。具体来说，输入输出序列化组件为每个布局生成任务精心设计输入和输出格式。动态样本选择负责为给定输入选择最有帮助的提示样本。布局排序器用于从法学硕士的多个输出中挑选最高质量的布局。我们使用四个公共数据集对所有现有布局生成任务进行实验。尽管我们的方法很简单，但实验结果表明，在这些任务上，LayoutPrompter 可以与最先进的方法竞争甚至超越，而无需任何模型训练或微调。这证明了这种多功能且无需培训的方法的有效性。此外，消融研究表明，在低数据情况下，LayoutPrompter 显着优于基于训练的基线，进一步表明 LayoutPrompter 的数据效率。我们的项目位于 https://github.com/microsoft/LayoutGeneration/tree/main/LayoutPrompter。

## Memory-Efficient Fine-Tuning of Compressed Large Language Models via sub-4-bit Integer Quantization<sup>poster<sup>

Authors: Jeonghoon Kim, Jung Hyun Lee, Sungdong Kim, Joonsuk Park, Kang Min Yoo, Se Jung Kwon, Dongsoo Lee

Link: [https://neurips.cc/virtual/2023/poster/72931](https://neurips.cc/virtual/2023/poster/72931)

Abstract:

 Large language models (LLMs) face the challenges in fine-tuning and deployment due to their high memory demands and computational costs. While parameter-efficient fine-tuning (PEFT) methods aim to reduce the memory usage of the optimizer state during fine-tuning, the inherent size of pre-trained LLM weights continues to be a pressing concern.  Even though quantization techniques are widely proposed to ease memory demands and accelerate LLM inference, most of these techniques are geared towards the deployment phase.To bridge this gap, this paper presents Parameter-Efficient and Quantization-aware Adaptation (PEQA) – a simple yet effective method that combines the advantages of PEFT with quantized LLMs. By updating solely the quantization scales, PEQA can be directly applied to quantized LLMs, ensuring seamless task transitions. Parallel to existing PEFT methods, PEQA significantly reduces the memory overhead associated with the optimizer state. Furthermore, it leverages the advantages of quantization to substantially reduce model sizes. Even after fine-tuning, the quantization structure of a PEQA-tuned LLM remains intact, allowing for accelerated inference on the deployment stage.We employ PEQA-tuning for task-specific adaptation on LLMs with up to $65$ billion parameters. To assess the logical reasoning and language comprehension of PEQA-tuned LLMs, we fine-tune low-bit quantized LLMs using a instruction dataset. Our results show that even when LLMs are quantized to below 4-bit precision, their capabilities in language modeling, few-shot in-context learning, and comprehension can be resiliently restored to (or even improved over) their full-precision original performances with PEQA.

摘要:

大型语言模型（LLM）由于其高内存需求和计算成本而面临着微调和部署的挑战。虽然参数高效微调 (PEFT) 方法旨在减少微调期间优化器状态的内存使用量，但预训练的 LLM 权重的固有大小仍然是一个紧迫的问题。尽管量化技术被广泛提出来缓解内存需求并加速 LLM 推理，但这些技术大多数都是针对部署阶段的。为了弥补这一差距，本文提出了参数高效和量化感知适应（PEQA）——一种简单但结合了 PEFT 与量化 LLM 优点的有效方法。通过仅更新量化尺度，PEQA 可以直接应用于量化的 LLM，确保无缝任务转换。与现有 PEFT 方法并行，PEQA 显着减少了与优化器状态相关的内存开销。此外，它利用量化的优势来大幅减小模型大小。即使在微调之后，PEQA 调整的 LLM 的量化结构仍然完好无损，从而可以在部署阶段加速推理。我们采用 PEQA 调整对 LLM 进行特定于任务的适应，参数高达 65 亿美元。为了评估 PEQA 调整的 LLM 的逻辑推理和语言理解能力，我们使用指令数据集微调低位量化 LLM。我们的结果表明，即使 LLM 被量化到低于 4 位精度，它们在语言建模、小样本上下文学习和理解方面的能力也可以通过以下方式弹性恢复（甚至改进）其全精度原始性能： PEQA。

## Fairness-guided Few-shot Prompting for Large Language Models<sup>poster<sup>

Authors: Huan Ma, Changqing Zhang, Yatao Bian, Lemao Liu, Zhirui Zhang, Peilin Zhao, Shu Zhang, Huazhu Fu, Qinghua Hu, Bingzhe Wu

Link: [https://neurips.cc/virtual/2023/poster/72392](https://neurips.cc/virtual/2023/poster/72392)

Abstract:

 Large language models have demonstrated surprising ability to perform in-context learning, i.e., these models can be directly applied to solve numerous downstream tasks by conditioning on a prompt constructed by a few input-output examples. However, prior research has shown that in-context learning can suffer from high instability due to variations in training examples, example order, and prompt formats. Therefore, the construction of an appropriate prompt is essential for improving the performance of in-context learning. In this paper,  we revisit this problem from the view of predictive bias. Specifically, we introduce a metric to evaluate the predictive bias of a fixed prompt against labels or a given attributes. Then we empirically show that prompts with higher bias always lead to unsatisfactory predictive quality. Based on this observation, we propose a novel search strategy based on the greedy search to identify the near-optimal prompt for improving the performance of in-context learning. We perform comprehensive experiments with state-of-the-art mainstream models such as GPT-3 on various downstream tasks. Our results indicate that our method can enhance the model's in-context learning performance in an effective and interpretable manner.

摘要:

大型语言模型已经表现出令人惊讶的执行上下文学习的能力，即，这些模型可以通过以几个输入输出示例构建的提示为条件，直接应用于解决大量下游任务。然而，先前的研究表明，由于训练示例、示例顺序和提示格式的变化，上下文学习可能会遭受高度不稳定的影响。因此，构建适当的提示对于提高情境学习的绩效至关重要。在本文中，我们从预测偏差的角度重新审视这个问题。具体来说，我们引入了一个指标来评估固定提示相对于标签或给定属性的预测偏差。然后我们凭经验表明，具有较高偏差的提示总是会导致预测质量不令人满意。基于这一观察，我们提出了一种基于贪婪搜索的新颖搜索策略，以识别近乎最佳的提示，以提高上下文学习的性能。我们使用 GPT-3 等最先进的主流模型在各种下游任务上进行全面的实验。我们的结果表明，我们的方法可以以有效且可解释的方式增强模型的上下文学习性能。

## Self-Chained Image-Language Model for Video Localization and Question Answering<sup>poster<sup>

Authors: Shoubin Yu, Jaemin Cho, Prateek Yadav, Mohit Bansal

Link: [https://neurips.cc/virtual/2023/poster/71124](https://neurips.cc/virtual/2023/poster/71124)

Abstract:

 Recent studies have shown promising results on utilizing large pre-trained image-language models for video question answering. While these image-language models can efficiently bootstrap the representation learning of video-language models, they typically concatenate uniformly sampled video frames as visual inputs without explicit language-aware, temporal modeling. When only a portion of a video input is relevant to the language query, such uniform frame sampling can often lead to missing important visual cues. Although humans often find a video moment to focus on and rewind the moment to answer questions, training a query-aware video moment localizer often requires expensive annotations and high computational costs. To address this issue, we propose Self-Chained Video Localization-Answering (SeViLA), a novel framework that leverages a single image-language model (BLIP- 2) to tackle both temporal keyframe localization and question answering on videos. SeViLA framework consists of two modules: Localizer and Answerer, where both are parameter-efficiently fine-tuned from BLIP-2. We propose two ways of chaining these modules for cascaded inference and self-refinement. First, in the forward chain, the Localizer finds multiple language-aware keyframes in a video, which the Answerer uses to predict the answer. Second, in the reverse chain, the Answerer generates keyframe pseudo-labels to refine the Localizer, alleviating the need for expensive video moment localization annotations. Our SeViLA framework outperforms several strong baselines/previous works on five challenging video question answering and event prediction benchmarks, and achieves the state-of-the-art in both fine-tuning (NExT-QA and STAR) and zero-shot (NExT-QA, STAR, How2QA, and VLEP) settings. We show a comprehensive analysis of our framework, including the impact of Localizer, comparisons of Localizer with other temporal localization models, pre-training/self-refinement of Localizer, and varying the number of keyframes.

摘要:

最近的研究表明，利用大型预训练图像语言模型进行视频问答具有良好的效果。虽然这些图像语言模型可以有效地引导视频语言模型的表示学习，但它们通常将统一采样的视频帧连接为视觉输入，而无需显式的语言感知、时间建模。当视频输入中只有一部分与语言查询相关时，这种统一的帧采样通常会导致丢失重要的视觉线索。尽管人类经常找到一个视频时刻来关注并倒回该时刻来回答问题，但训练具有查询感知的视频时刻定位器通常需要昂贵的注释和高计算成本。为了解决这个问题，我们提出了自链视频定位回答（SeViLA），这是一种利用单一图像语言模型（BLIP-2）来解决视频上的时间关键帧定位和问题回答的新颖框架。 SeViLA 框架由两个模块组成：Localizer 和 Answerer，这两个模块都是从 BLIP-2 进行参数高效微调的。我们提出了两种链接这些模块以进行级联推理和自我优化的方法。首先，在前向链中，定位器在视频中找到多个语言感知关键帧，应答器使用这些关键帧来预测答案。其次，在反向链中，应答器生成关键帧伪标签来细化定位器，从而减轻对昂贵的视频时刻定位注释的需求。我们的 SeViLA 框架在五个具有挑战性的视频问答和事件预测基准上优于几个强大的基线/之前的工作，并在微调（NExT-QA 和 STAR）和零样本（NExT- QA、STAR、How2QA 和 VLEP）设置。我们展示了对我们的框架的全面分析，包括 Localizer 的影响、Localizer 与其他时间定位模型的比较、Localizer 的预训练/自我细化以及改变关键帧的数量。

## Kiki or Bouba? Sound Symbolism in Vision-and-Language Models<sup>poster<sup>

Authors: Morris Alper, Hadar Averbuch-Elor

Link: [https://neurips.cc/virtual/2023/poster/71134](https://neurips.cc/virtual/2023/poster/71134)

Abstract:

 Although the mapping between sound and meaning in human language is assumed to be largely arbitrary, research in cognitive science has shown that there are non-trivial correlations between particular sounds and meanings across languages and demographic groups, a phenomenon known as sound symbolism. Among the many dimensions of meaning, sound symbolism is particularly salient and well-demonstrated with regards to cross-modal associations between language and the visual domain. In this work, we address the question of whether sound symbolism is reflected in vision-and-language models such as CLIP and Stable Diffusion. Using zero-shot knowledge probing to investigate the inherent knowledge of these models, we find strong evidence that they do show this pattern, paralleling the well-known kiki-bouba effect in psycholinguistics. Our work provides a novel method for demonstrating sound symbolism and understanding its nature using computational tools. Our code will be made publicly available.

摘要:

虽然人类语言中声音和意义之间的映射被认为在很大程度上是任意的，但认知科学研究表明，跨语言和人口群体的特定声音和意义之间存在着重要的相关性，这种现象被称为声音象征主义。在意义的许多维度中，声音象征尤其突出，并且在语言和视觉领域之间的跨模式关联方面得到了充分证明。在这项工作中，我们解决了声音象征主义是否反映在视觉和语言模型（例如 CLIP 和稳定扩散）中的问题。使用零样本知识探测来研究这些模型的固有知识，我们发现强有力的证据表明它们确实表现出这种模式，与心理语言学中众所周知的 kiki-bouba 效应相似。我们的工作提供了一种利用计算工具展示声音象征意义并理解其本质的新颖方法。我们的代码将公开。

## EvoPrompting: Language Models for Code-Level Neural Architecture Search<sup>poster<sup>

Authors: Angelica Chen, David Dohan, David So

Link: [https://neurips.cc/virtual/2023/poster/70729](https://neurips.cc/virtual/2023/poster/70729)

Abstract:

 Given the recent impressive accomplishments of language models (LMs) for code generation, we explore the use of LMs as general adaptive mutation and crossover operators for an evolutionary neural architecture search (NAS) algorithm.While NAS still proves too difficult a task for LMs to succeed at solely through prompting, we find that the combination of evolutionary prompt engineering with soft prompt-tuning, a method we term EvoPrompting, consistently finds diverse and high performing models. We first demonstrate that EvoPrompting is effective on the computationally efficient MNIST-1D dataset, where EvoPrompting produces convolutional architecture variants that outperform both those designed by human experts and naive few-shot prompting in terms of accuracy and model size. We then apply our method to searching for graph neural networks on the CLRS Algorithmic Reasoning Benchmark, where EvoPrompting is able to design novel architectures that outperform current state-of-the-art models on 21 out of 30 algorithmic reasoning tasks while maintaining similar model size. EvoPrompting is successful at designing accurate and efficient neural network architectures across a variety of machine learning tasks, while also being general enough for easy adaptation to other tasks beyond neural network design.

摘要:

鉴于语言模型 (LM) 最近在代码生成方面取得了令人印象深刻的成就，我们探索使用 LM 作为进化神经架构搜索 (NAS) 算法的通用自适应变异和交叉算子。仅通过提示就能成功的语言模型，我们发现进化提示工程与软提示调整（我们称之为 EvoPrompting 的方法）的结合，始终能找到多样化且高性能的模型。我们首先证明 EvoPrompting 在计算效率高的 MNIST-1D 数据集上是有效的，其中 EvoPrompting 产生的卷积架构变体在准确性和模型大小方面优于人类专家设计的架构和简单的少样本提示。然后，我们应用我们的方法在 CLRS 算法推理基准上搜索图神经网络，其中 EvoPrompting 能够设计新颖的架构，在 30 个算法推理任务中的 21 个上优于当前最先进的模型，同时保持相似的模型大小。 EvoPrompting 成功地在各种机器学习任务中设计了准确、高效的神经网络架构，同时也具有足够的通用性，可以轻松适应神经网络设计之外的其他任务。

## Stable and low-precision training for large-scale vision-language models<sup>poster<sup>

Authors: Mitchell Wortsman, Tim Dettmers, Luke Zettlemoyer, Ari Morcos, Ali Farhadi, Ludwig Schmidt

Link: [https://neurips.cc/virtual/2023/poster/70245](https://neurips.cc/virtual/2023/poster/70245)

Abstract:

 We introduce new methods for 1) accelerating and 2) stabilizing training for large language-vision models. 1) For acceleration, we introduce SwitchBack, a linear layer for int8 quantized training which provides a speed-up of 13-25% while matching the performance of bfloat16 training within 0.1 percentage points for the 1B parameter CLIP ViT-Huge---the largest int8 training to date. Our main focus is int8 as GPU support for float8 is rare, though we also analyze float8 training through simulation. While SwitchBack proves effective for float8, we show that standard techniques are also successful if the network is trained and initialized so that large feature magnitudes are discouraged, which we accomplish via layer-scale initialized with zeros. 2) For stability, we analyze loss spikes and find they consistently occur 1-8 iterations after the squared gradients become under-estimated by their AdamW second moment estimator. As a result, we recommend an AdamW-Adafactor hybrid which avoids loss spikes when training a CLIP ViT-Huge model and outperforms gradient clipping at the scales we test.

摘要:

我们引入了 1）加速和 2）稳定大型语言视觉模型训练的新方法。 1) 为了加速，我们引入了 SwitchBack，一个用于 int8 量化训练的线性层，它提供了 13-25% 的加速，同时在 1B 参数 CLIP ViT-Huge 上与 bfloat16 训练的性能匹配在 0.1 个百分点以内——迄今为止最大的 int8 训练。我们的主要关注点是 int8，因为 GPU 对 float8 的支持很少，尽管我们也通过模拟分析 float8 的训练。虽然 SwitchBack 证明对 float8 有效，但我们表明，如果网络经过训练和初始化，不鼓励使用大的特征量，那么标准技术也是成功的，我们通过用零初始化的层规模来实现这一点。 2) 为了稳定性，我们分析了损失峰值，发现在 AdamW 二阶矩估计器低估平方梯度后，它们始终出现 1-8 次迭代。因此，我们推荐 AdamW-Adafactor 混合体，它可以在训练 CLIP ViT-Huge 模型时避免损失尖峰，并且在我们测试的尺度上优于梯度裁剪。

## Preference-grounded Token-level Guidance for Language Model Fine-tuning<sup>poster<sup>

Authors: Shentao Yang, Shujian Zhang, Congying Xia, Yihao Feng, Caiming Xiong, Mingyuan Zhou

Link: [https://neurips.cc/virtual/2023/poster/72756](https://neurips.cc/virtual/2023/poster/72756)

Abstract:

 Aligning language models (LMs) with preferences is an important problem in natural language generation. A key challenge is that preferences are typically provided at the sequence level while LM training and generation both occur at the token level. There is, therefore, a granularity mismatch between the preference and the LM training losses, which may complicate the learning problem. In this paper, we address this issue by developing an alternate training process, where we iterate between grounding the sequence-level preference into token-level training guidance, and improving the LM with the learned guidance. For guidance learning, we design a framework that extends the pairwise-preference learning in imitation learning to both variable-length LM generation and the utilization of the preference among multiple generations. For LM training, based on the amount of supervised data, we present two minimalist learning objectives that utilize the learned guidance. In experiments, our method performs competitively on two distinct representative LM tasks --- discrete-prompt generation and text summarization.

摘要:

将语言模型（LM）与偏好保持一致是自然语言生成中的一个重要问题。一个关键的挑战是偏好通常是在序列级别提供的，而 LM 训练和生成都发生在令牌级别。因此，偏好和 LM 训练损失之间存在粒度不匹配，这可能会使学习问题变得复杂。在本文中，我们通过开发替代训练过程来解决这个问题，在该过程中，我们在将序列级偏好融入到标记级训练指导中，并利用学习到的指导来改进 LM 之间进行迭代。对于引导学习，我们设计了一个框架，将模仿学习中的成对偏好学习扩展到可变长度的 LM 生成和多代之间偏好的利用。对于 LM 训练，根据监督数据量，我们提出了两个利用学习指导的极简学习目标。在实验中，我们的方法在两个不同的代表性 LM 任务上表现出竞争力——离散提示生成和文本摘要。

## MarioGPT: Open-Ended Text2Level Generation through Large Language Models<sup>poster<sup>

Authors: Shyam Sudhakaran, Miguel González-Duque, Matthias Freiberger, Claire Glanois, Elias Najarro, Sebastian Risi

Link: [https://neurips.cc/virtual/2023/poster/71191](https://neurips.cc/virtual/2023/poster/71191)

Abstract:

 Procedural Content Generation (PCG) is a technique to generate complex and diverse environments in an automated way. However, while generating content with PCG methods is often straightforward, generating meaningful content that reflects specific  intentions and constraints remains challenging. Furthermore, many PCG algorithms lack the ability to generate content in an open-ended manner. Recently, Large Language Models (LLMs) have  shown to be incredibly effective in many diverse domains. These trained LLMs can be fine-tuned, re-using information and accelerating training for new tasks. Here, we introduce MarioGPT, a fine-tuned GPT2 model trained to generate tile-based game levels, in our case Super Mario Bros levels. MarioGPT can not only generate diverse levels, but can be  text-prompted for controllable level generation, addressing one of the key challenges of current PCG techniques.  As far as we know, MarioGPT is the first text-to-level model and combined with novelty search it enables the  generation of diverse levels with varying play-style dynamics (i.e. player paths) and the open-ended discovery of an increasingly diverse range of content. Code available at https://github.com/shyamsn97/mario-gpt.

摘要:

程序内容生成（PCG）是一种以自动化方式生成复杂多样环境的技术。然而，虽然使用 PCG 方法生成内容通常很简单，但生成反映特定意图和约束的有意义的内容仍然具有挑战性。此外，许多 PCG 算法缺乏以开放式方式生成内容的能力。最近，大型语言模型 (LLM) 在许多不同的领域都显示出极其有效的效果。这些经过培训的法学硕士可以进行微调，重复使用信息并加速新任务的培训。在这里，我们介绍 MarioGPT，这是一种经过微调的 GPT2 模型，经过训练可以生成基于图块的游戏关卡，在我们的例子中是《超级马里奥兄弟》关卡。 MarioGPT不仅可以生成多样化的关卡，还可以通过文本提示进行可控关卡生成，解决了当前PCG技术的关键挑战之一。据我们所知，MarioGPT 是第一个文本到关卡模型，与新颖性搜索相结合，它能够生成具有不同游戏风格动态（即玩家路径）的不同关卡，以及日益多样化的范围的开放式发现的内容。代码可在 https://github.com/shyamsn97/mario-gpt 获取。

## GPT4Tools: Teaching Large Language Model to Use Tools via Self-instruction<sup>poster<sup>

Authors: Rui Yang, Lin Song, Yanwei Li, Sijie Zhao, Yixiao Ge, Xiu Li, Ying Shan

Link: [https://neurips.cc/virtual/2023/poster/71060](https://neurips.cc/virtual/2023/poster/71060)

Abstract:

 This paper aims to efficiently enable Large Language Models (LLMs) to use multi-modal tools.The advanced proprietary LLMs, such as ChatGPT and GPT-4, have shown great potential for tool usage through sophisticated prompt engineering.Nevertheless, these models typically rely on prohibitive computational costs and publicly inaccessible data.To address these challenges, we propose the GPT4Tools based on self-instruct to enable open-source LLMs, such as LLaMA and OPT, to use tools.It generates an instruction-following dataset by prompting an advanced teacher with various multi-modal contexts.By using the Low-Rank Adaptation (LoRA) optimization, our approach facilitates the open-source LLMs to solve a range of visual problems, including visual comprehension and image generation.Moreover, we provide a benchmark to evaluate the ability of LLMs to use tools, which is performed in both zero-shot and fine-tuning ways.Extensive experiments demonstrate the effectiveness of our method on various language models, which not only significantly improves the accuracy of invoking seen tools, but also enables the zero-shot capacity for unseen tools.

摘要:

本文旨在有效地使大型语言模型（LLM）能够使用多模态工具。ChatGPT 和 GPT-4 等先进的专有 LLM 通过复杂的提示工程显示出工具使用的巨大潜力。然而，这些模型通常依赖于高昂的计算成本和公开不可访问的数据。为了解决这些挑战，我们提出了基于自指令的 GPT4Tools，以使开源 LLM（例如 LLaMA 和 OPT）能够使用工具。它通过以下方式生成遵循指令的数据集：通过使用低阶适应（LoRA）优化，我们的方法有助于开源法学硕士解决一系列视觉问题，包括视觉理解和图像生成。此外，我们提供评估LLM使用工具能力的基准，以零样本和微调的方式进行。大量的实验证明了我们的方法在各种语言模型上的有效性，这不仅显着提高了调用所见工具的准确性，而且还能实现看不见的工具的零射击能力。

## Leveraging Pre-trained Large Language Models to Construct and Utilize World Models for Model-based Task Planning<sup>poster<sup>

Authors: Lin Guan, Karthik Valmeekam, Sarath Sreedharan, Subbarao Kambhampati

Link: [https://neurips.cc/virtual/2023/poster/69907](https://neurips.cc/virtual/2023/poster/69907)

Abstract:

 There is a growing interest in applying pre-trained large language models (LLMs) to planning problems. However, methods that use LLMs directly as planners are currently impractical due to several factors, including limited correctness of plans, strong reliance on feedback from interactions with simulators or even the actual environment, and the inefficiency in utilizing human feedback. In this work, we introduce a novel alternative paradigm that constructs an explicit world (domain) model in planning domain definition language (PDDL) and then uses it to plan with sound domain-independent planners. To address the fact that LLMs may not generate a fully functional PDDL model initially, we employ LLMs as an interface between PDDL and sources of corrective feedback, such as PDDL validators and humans. For users who lack a background in PDDL, we show that LLMs can translate PDDL into natural language and effectively encode corrective feedback back to the underlying domain model. Our framework not only enjoys the correctness guarantee offered by the external planners but also reduces human involvement by allowing users to correct domain models at the beginning, rather than inspecting and correcting (through interactive prompting) every generated plan as in previous work. On two IPC domains and a Household domain that is more complicated than commonly used benchmarks such as ALFWorld, we demonstrate that GPT-4 can be leveraged to produce high-quality PDDL models for over 40 actions, and the corrected PDDL models are then used to successfully solve 48 challenging planning tasks. Resources, including the source code, are released at: https://guansuns.github.io/pages/llm-dm.

摘要:

人们越来越有兴趣将预训练的大型语言模型（LLM）应用于规划问题。然而，由于多种因素，直接使用法学硕士作为规划者的方法目前是不切实际的，包括计划的正确性有限、强烈依赖与模拟器甚至实际环境交互的反馈，以及利用人类反馈的效率低下。在这项工作中，我们引入了一种新颖的替代范式，该范式在规划领域定义语言（PDDL）中构建显式世界（领域）模型，然后使用它与健全的领域无关规划器进行规划。为了解决 LLM 最初可能无法生成功能齐全的 PDDL 模型的事实，我们采用 LLM 作为 PDDL 和纠正反馈源（例如 PDDL 验证者和人类）之间的接口。对于缺乏 PDDL 背景的用户，我们表明法学硕士可以将 PDDL 翻译成自然语言，并有效地将纠正反馈编码回底层领域模型。我们的框架不仅享有外部规划者提供的正确性保证，而且还允许用户在开始时纠正域模型，而不是像以前的工作那样检查和纠正（通过交互式提示）每个生成的计划，从而减少了人为参与。在两个 IPC 域和一个比 ALFWorld 等常用基准更复杂的 Household 域上，我们证明可以利用 GPT-4 为 40 多个动作生成高质量的 PDDL 模型，然后使用校正后的 PDDL 模型成功解决 48 项具有挑战性的规划任务。包括源代码在内的资源发布于：https://guansuns.github.io/pages/llm-dm。

## From Cloze to Comprehension: Retrofitting Pre-trained Masked Language Models to Pre-trained Machine Reader<sup>poster<sup>

Authors: Weiwen Xu, Xin Li, Wenxuan Zhang, Meng Zhou, Wai Lam, Luo Si, Lidong Bing

Link: [https://neurips.cc/virtual/2023/poster/72478](https://neurips.cc/virtual/2023/poster/72478)

Abstract:

 We present Pre-trained Machine Reader (PMR), a novel method for retrofitting pre-trained masked language models (MLMs) to pre-trained machine reading comprehension (MRC) models without acquiring labeled data.PMR can resolve the discrepancy between model pre-training and downstream fine-tuning of existing MLMs.To build the proposed PMR, we constructed a large volume of general-purpose and high-quality MRC-style training data by using Wikipedia hyperlinks and designed a Wiki Anchor Extraction task to guide the MRC-style pre-training.Apart from its simplicity, PMR effectively solves extraction tasks, such as Extractive Question Answering and Named Entity Recognition. PMR shows tremendous improvements over existing approaches, especially in low-resource scenarios.When applied to the sequence classification task in the MRC formulation, PMR enables the extraction of high-quality rationales to explain the classification process, thereby providing greater prediction explainability. PMR also has the potential to serve as a unified model for tackling various extraction and classification tasks in the MRC formulation.

摘要:

我们提出了预训练机器阅读器（PMR），这是一种无需获取标记数据即可将预训练掩码语言模型（MLM）改造为预训练机器阅读理解（MRC）模型的新方法。PMR 可以解决模型之间的差异现有 MLM 的预训练和下游微调。为了构建所提出的 PMR，我们使用维基百科超链接构建了大量通用且高质量的 MRC 式训练数据，并设计了一个 Wiki Anchor Extraction 任务来指导MRC式的预训练。除了简单性之外，PMR还有效地解决了提取任务，例如提取问答和命名实体识别。 PMR 比现有方法显示出巨大的改进，特别是在资源匮乏的场景中。当应用于 MRC 公式中的序列分类任务时，PMR 能够提取高质量的基本原理来解释分类过程，从而提供更好的预测可解释性。 PMR 还有潜力作为统一模型来处理 MRC 公式中的各种提取和分类任务。

## No Train No Gain: Revisiting Efficient Training Algorithms For Transformer-based Language Models<sup>poster<sup>

Authors: Jean Kaddour, Oscar Key, Piotr Nawrot, Pasquale Minervini, Matt Kusner

Link: [https://neurips.cc/virtual/2023/poster/70190](https://neurips.cc/virtual/2023/poster/70190)

Abstract:

 The computation necessary for training Transformer-based language models has skyrocketed in recent years.This trend has motivated research on efficient training algorithms designed to improve training, validation, and downstream performance faster than standard training. In this work, we revisit three categories of such algorithms: dynamic architectures (layer stacking, layer dropping), batch selection (selective backprop., RHO-loss), and efficient optimizers (Lion, Sophia). When pre-training BERT and T5 with a fixed computation budget using such methods, we find that their training, validation, and downstream gains vanish compared to a baseline with a fully-decayed learning rate. We define an evaluation protocol that enables computation to be done on arbitrary machines by mapping all computation time to a reference machine which we call reference system time. We discuss the limitations of our proposed protocol and release our code to encourage rigorous research in efficient training procedures: https://github.com/JeanKaddour/NoTrainNoGain.

摘要:

近年来，训练基于 Transformer 的语言模型所需的计算量猛增。这一趋势推动了对高效训练算法的研究，这些算法旨在比标准训练更快地提高训练、验证和下游性能。在这项工作中，我们重新审视了三类此类算法：动态架构（层堆叠、层丢弃）、批量选择（选择性反向传播、RHO 损失）和高效优化器（Lion、Sophia）。当使用此类方法以固定计算预算预训练 BERT 和 T5 时，我们发现与学习率完全衰减的基线相比，它们的训练、验证和下游增益消失了。我们定义了一个评估协议，通过将所有计算时间映射到我们称为参考系统时间的参考机器，可以在任意机器上进行计算。我们讨论了我们提出的协议的局限性，并发布了我们的代码，以鼓励对高效训练程序进行严格研究：https://github.com/JeanKaddour/NoTrainNoGain。

## AVIS: Autonomous Visual Information Seeking with Large Language Model Agent<sup>poster<sup>

Authors: Ziniu Hu, Ahmet Iscen, Chen Sun, Kai-Wei Chang, Yizhou Sun, David Ross, Cordelia Schmid, Alireza Fathi

Link: [https://neurips.cc/virtual/2023/poster/72718](https://neurips.cc/virtual/2023/poster/72718)

Abstract:

 In this paper, we propose an autonomous information seeking visual question answering framework, AVIS. Our method leverages a Large Language Model (LLM) to dynamically strategize the utilization of external tools and to investigate their outputs via tree search, thereby acquiring the indispensable knowledge needed to provide answers to the posed questions. Responding to visual questions that necessitate external knowledge, such as "What event is commemorated by the building depicted in this image?", is a complex task. This task presents a combinatorial search space that demands a sequence of actions, including invoking APIs, analyzing their responses, and making informed decisions. We conduct a user study to collect a variety of instances of human decision-making when faced with this task. This data is then used to design a system comprised of three components: an LLM-powered planner that dynamically determines which tool to use next, an LLM-powered reasoner that analyzes and extracts key information from the tool outputs, and a working memory component that retains the acquired information throughout the process. The collected user behavior serves as a guide for our system in two key ways. First, we create a transition graph by analyzing the sequence of decisions made by users. This graph delineates distinct states and confines the set of actions available at each state. Second, we use examples of user decision-making to provide our LLM-powered planner and reasoner with relevant contextual instances, enhancing their capacity to make informed decisions. We show that AVIS achieves state-of-the-art results on knowledge-based visual question answering benchmarks such as Infoseek and OK-VQA.

摘要:

在本文中，我们提出了一种自主信息寻求视觉问答框架 AVIS。我们的方法利用大型语言模型（LLM）来动态制定外部工具的使用策略，并通过树搜索调查其输出，从而获取为所提出的问题提供答案所需的不可或缺的知识。回答需要外部知识的视觉问题，例如“该图像中描绘的建筑物是为了纪念什么事件？”，是一项复杂的任务。此任务提供了一个组合搜索空间，需要一系列操作，包括调用 API、分析其响应以及做出明智的决策。我们进行了一项用户研究，以收集人类在面临此任务时做出决策的各种实例。然后，这些数据被用来设计一个由三个组件组成的系统：一个由 LLM 驱动的规划器，动态确定下一步要使用哪个工具；一个由 LLM 驱动的推理器，用于分析并从工具输出中提取关键信息；以及一个工作记忆组件，在整个过程中保留所获取的信息。收集到的用户行为通过两个关键方式为我们的系统提供指导。首先，我们通过分析用户做出的决策顺序来创建一个转换图。该图描绘了不同的状态并限制了每个状态下可用的操作集。其次，我们使用用户决策的示例为我们由 LLM 支持的规划器和推理器提供相关的上下文实例，从而增强他们做出明智决策的能力。我们表明，AVIS 在基于知识的视觉问答基准（例如 Infoseek 和 OK-VQA）上取得了最先进的结果。

## Does Localization Inform Editing? Surprising Differences in Causality-Based Localization vs. Knowledge Editing in Language Models<sup>poster<sup>

Authors: Peter Hase, Mohit Bansal, Been Kim, Asma Ghandeharioun

Link: [https://neurips.cc/virtual/2023/poster/72296](https://neurips.cc/virtual/2023/poster/72296)

Abstract:

 Language models learn a great quantity of factual information during pretraining, and recent work localizes this information to specific model weights like mid-layer MLP weights. In this paper, we find that we can change how a fact is stored in a model by editing weights that are in a different location than where existing methods suggest that the fact is stored. This is surprising because we would expect that localizing facts to specific model parameters would tell us where to manipulate knowledge in models, and this assumption has motivated past work on model editing methods. Specifically, we show that localization conclusions from representation denoising (also known as Causal Tracing) do not provide any insight into which model MLP layer would be best to edit in order to override an existing stored fact with a new one. This finding raises questions about how past work relies on Causal Tracing to select which model layers to edit. Next, we consider several variants of the editing problem, including erasing and amplifying facts. For one of our editing problems, editing performance does relate to localization results from representation denoising, but we find that which layer we edit is a far better predictor of performance. Our results suggest, counterintuitively, that better mechanistic understanding of how pretrained language models work may not always translate to insights about how to best change their behavior.

摘要:

语言模型在预训练过程中学习大量事实信息，最近的工作将这些信息定位到特定的模型权重，例如中间层 MLP 权重。在本文中，我们发现我们可以通过编辑与现有方法建议事实存储位置不同的位置的权重来更改事实在模型中的存储方式。这是令人惊讶的，因为我们期望将事实本地化到特定的模型参数会告诉我们在哪里操纵模型中的知识，并且这种假设激发了过去对模型编辑方法的研究。具体来说，我们表明，表示去噪（也称为因果追踪）的定位结论并没有提供任何关于哪个模型 MLP 层最适合编辑以便用新事实覆盖现有存储事实的见解。这一发现提出了关于过去的工作如何依赖因果追踪来选择要编辑的模型层的问题。接下来，我们考虑编辑问题的几种变体，包括删除和放大事实。对于我们的一个编辑问题，编辑性能确实与表示去噪的本地化结果有关，但我们发现我们编辑的图层可以更好地预测性能。与直觉相反，我们的结果表明，对预训练语言模型如何工作的更好的机械理解可能并不总是转化为关于如何最好地改变其行为的见解。

## LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models<sup>poster<sup>

Authors: Neel Guha, Julian Nyarko, Daniel Ho, Christopher Ré, Adam Chilton, Aditya K, Alex Chohlas-Wood, Austin Peters, Brandon Waldon, Daniel Rockmore, Diego Zambrano, Dmitry Talisman, Enam Hoque, Faiz Surani, Frank Fagan, Galit Sarfaty, Gregory Dickinson, Haggai Porat, Jason Hegland, Jessica Wu, Joe Nudell, Joel Niklaus, John Nay, Jonathan Choi, Kevin Tobia, Margaret Hagan, Megan Ma, Michael Livermore, Nikon Rasumov-Rahe, Nils Holzenberger, Noam Kolt, Peter Henderson, Sean Rehaag, Sharad Goel, Shang Gao, Spencer Williams, Sunny Gandhi, Tom Zur, Varun Iyer, Zehua Li

Link: [https://neurips.cc/virtual/2023/poster/73565](https://neurips.cc/virtual/2023/poster/73565)

Abstract:

 The advent of large language models (LLMs) and their adoption by the legal community has given rise to the question: what types of legal reasoning can LLMs perform? To enable greater study of this question, we present LegalBench: a collaboratively constructed legal reasoning benchmark consisting of 162 tasks covering six different types of legal reasoning. LegalBench was built through an interdisciplinary process, in which we collected tasks designed and hand-crafted by legal professionals. Because these subject matter experts took a leading role in construction, tasks either measure legal reasoning capabilities that are practically useful, or measure reasoning skills that lawyers find interesting. To enable cross-disciplinary conversations about LLMs in the law, we additionally show how popular legal frameworks for describing legal reasoning—which distinguish between its many forms—correspond to LegalBench tasks, thus giving lawyers and LLM developers a common vocabulary. This paper describes LegalBench, presents an empirical evaluation of 20 open-source and commercial LLMs, and illustrates the types of research explorations LegalBench enables.

摘要:

大语言模型（LLM）的出现及其被法律界的采用引发了一个问题：LLM 可以执行哪些类型的法律推理？为了更好地研究这个问题，我们提出了 LegalBench：一个协作构建的法律推理基准，由涵盖六种不同类型的法律推理的 162 项任务组成。 LegalBench 是通过跨学科过程构建的，其中我们收集了由法律专业人士设计和手工制作的任务。由于这些主题专家在构建中发挥主导作用，因此任务要么衡量实际有用的法律推理能力，要么衡量律师感兴趣的推理技能。为了能够就法律中的法学硕士进行跨学科对话，我们还展示了描述法律推理的流行法律框架（区分其多种形式）如何与 LegalBench 任务相对应，从而为律师和法学硕士开发人员提供了通用词汇。本文介绍了 LegalBench，对 20 个开源和商业法学硕士进行了实证评估，并说明了 LegalBench 所支持的研究探索类型。

## Large Language Models as Commonsense Knowledge for Large-Scale Task Planning<sup>poster<sup>

Authors: Zirui Zhao, Wee Sun Lee, David Hsu

Link: [https://neurips.cc/virtual/2023/poster/71394](https://neurips.cc/virtual/2023/poster/71394)

Abstract:

 Large-scale task planning is a major challenge.  Recent work exploits large  language models (LLMs) directly as a policy and shows surprisingly  interesting results.  This paper shows that LLMs provide a  commonsense model of the world in addition to a policy that acts on it.  The world model and the policy can be combined in a search  algorithm, such as Monte Carlo Tree Search (MCTS), to scale up task  planning.  In our new LLM-MCTS algorithm, the LLM-induced world model  provides a commonsense prior belief for MCTS to achieve effective reasoning;  the LLM-induced policy acts as a heuristic to guide the search, vastly  improving search efficiency. Experiments show that LLM-MCTS outperforms  both MCTS alone and policies induced by LLMs (GPT2 and GPT3.5) by a wide  margin, for complex, novel tasks.   Further experiments and analyses on multiple tasks --  multiplication, travel planning, object rearrangement --  suggest minimum description length (MDL)  as a general guiding principle: if the  description length of the world model is substantially smaller than that of  the  policy, using LLM as a world model for model-based planning is likely better  than using LLM solely as a policy.

摘要:

大规模任务规划是一个重大挑战。最近的工作直接利用大型语言模型（LLM）作为一种策略，并显示出令人惊讶的有趣结果。本文表明，法学硕士提供了一个关于世界的常识模型以及对其采取行动的政策。世界模型和策略可以结合在搜索算法中，例如蒙特卡罗树搜索（MCTS），以扩大任务规划规模。在我们新的LLM-MCTS算法中，LLM引发的世界模型为MCTS提供了常识性先验信念，以实现有效推理； LLM 引发的策略作为启发式指导搜索，极大地提高了搜索效率。实验表明，对于复杂、新颖的任务，LLM-MCTS 远远优于单独的 MCTS 和 LLM（GPT2 和 GPT3.5）诱导的策略。对多项任务（乘法、旅行规划、对象重新排列）的进一步实验和分析建议将最小描述长度（MDL）作为一般指导原则：如果世界模型的描述长度远小于策略的描述长度，则使用 LLM作为基于模型的规划的世界模型可能比仅将法学硕士用作政策更好。

## Benchmarking Large Language Models on CMExam - A comprehensive Chinese Medical Exam Dataset<sup>poster<sup>

Authors: Junling Liu, Peilin Zhou, Yining Hua, Dading Chong, Zhongyu Tian, Andrew Liu, Helin Wang, Chenyu You, Zhenhua Guo, LEI ZHU, Michael Li

Link: [https://neurips.cc/virtual/2023/poster/73638](https://neurips.cc/virtual/2023/poster/73638)

Abstract:

 Recent advancements in large language models (LLMs) have transformed the field of question answering (QA). However, evaluating LLMs in the medical field is challenging due to the lack of standardized and comprehensive datasets. To address this gap, we introduce CMExam, sourced from the Chinese National Medical Licensing Examination. CMExam consists of 60K+ multiple-choice questions for standardized and objective evaluations, as well as solution explanations for model reasoning evaluation in an open-ended manner. For in-depth analyses of LLMs, we invited medical professionals to label five additional question-wise annotations, including disease groups, clinical departments, medical disciplines, areas of competency, and question difficulty levels. Alongside the dataset, we further conducted thorough experiments with representative LLMs and QA algorithms on CMExam. The results show that GPT-4 had the best accuracy of 61.6% and a weighted F1 score of 0.617. These results highlight a great disparity when compared to human accuracy, which stood at 71.6%. For explanation tasks, while LLMs could generate relevant reasoning and demonstrate improved performance after finetuning, they fall short of a desired standard, indicating ample room for improvement. To the best of our knowledge, CMExam is the first Chinese medical exam dataset to provide comprehensive medical annotations. The experiments and findings of LLM evaluation also provide valuable insights into the challenges and potential solutions in developing Chinese medical QA systems and LLM evaluation pipelines.

摘要:

大型语言模型（LLM）的最新进展已经改变了问答（QA）领域。然而，由于缺乏标准化和全面的数据集，评估医学领域的法学硕士具有挑战性。为了弥补这一差距，我们引入了源自中国国家医师资格考试的 CMExam。 CMExam包含60K+多项选择题，用于标准化和客观的评估，以及开放式模型推理评估的解决方案解释。为了对法学硕士进行深入分析，我们邀请医学专业人士额外标注了五个问题注释，包括疾病组、临床科室、医学学科、能力领域和问题难度级别。除了数据集之外，我们还在 CMExam 上使用代表性的 LLM 和 QA 算法进行了彻底的实验。结果显示，GPT-4 的准确率最好，为 61.6%，加权 F1 得分为 0.617。这些结果突显了与人类准确率（71.6%）相比的巨大差距。对于解释任务，虽然法学硕士可以生成相关推理并在微调后表现出改进的性能，但它们没有达到预期的标准，这表明有很大的改进空间。据我们所知，CMExam 是第一个提供全面医学注释的中国医学检查数据集。法学硕士评估的实验和结果也为开发中国医学质量保证系统和法学硕士评估管道的挑战和潜在解决方案提供了宝贵的见解。

## Large Language Models of Code Fail at Completing Code with Potential Bugs<sup>poster<sup>

Authors: Tuan Dinh, Jinman Zhao, Samson Tan, Renato Negrinho, Leonard Lausen, Sheng Zha, George Karypis

Link: [https://neurips.cc/virtual/2023/poster/70988](https://neurips.cc/virtual/2023/poster/70988)

Abstract:

 Large language models of code (Code-LLMs) have recently brought tremendous advances to code completion, a fundamental feature of programming assistance and code intelligence. However, most existing works ignore the possible presence of bugs in the code context for generation, which are inevitable in software development. Therefore, we introduce and study the buggy-code completion problem, inspired by the realistic scenario of real-time code suggestion where the code context contains potential bugs – anti-patterns that can become bugs in the completed program. To systematically study the task, we introduce two datasets: one with synthetic bugs derived from semantics-altering operator changes (buggy-HumanEval) and one with realistic bugs derived from user submissions to coding problems (buggy-FixEval). We find that the presence of potential bugs significantly degrades the generation performance of the high-performing Code-LLMs. For instance, the passing rates of CODEGEN-2B-MONO on test cases of buggy-HumanEval drop more than 50% given a single potential bug in the context. Finally, we investigate several post-hoc methods for mitigating the adverse effect of potential bugs and find that there remains a large gap in post-mitigation performance.

摘要:

大型代码语言模型（Code-LLM）最近在代码补全方面带来了巨大进步，这是编程辅助和代码智能的基本特征。然而，大多数现有的工作都忽略了生成代码上下文中可能存在的错误，这在软件开发中是不可避免的。因此，我们引入并研究了错误代码完成问题，受到实时代码建议的现实场景的启发，其中代码上下文包含潜在的错误 - 可能成为已完成程序中的错误的反模式。为了系统地研究该任务，我们引入了两个数据集：一个数据集包含源自语义改变操作符更改的合成错误 (buggy-HumanEval)，另一个数据集包含源自用户提交的编码问题的实际错误 (buggy-FixEval)。我们发现潜在错误的存在会显着降低高性能 Code-LLM 的生成性能。例如，考虑到上下文中存在单个潜在错误，CODEGEN-2B-MONO 在 buggy-HumanEval 测试用例上的通过率下降了 50% 以上。最后，我们研究了几种减轻潜在错误不利影响的事后方法，发现缓解后的性能仍然存在很大差距。

## Winner-Take-All Column Row Sampling for Memory Efficient Adaptation of Language Model<sup>poster<sup>

Authors: Zirui Liu, Guanchu Wang, Shaochen (Henry) Zhong, Zhaozhuo Xu, Daochen Zha, Ruixiang Tang, Zhimeng Jiang, Kaixiong Zhou, Vipin Chaudhary, Shuai Xu, Xia Hu

Link: [https://neurips.cc/virtual/2023/poster/71585](https://neurips.cc/virtual/2023/poster/71585)

Abstract:

 As the model size grows rapidly, fine-tuning the large pre-trained language model has become increasingly difficult due to its extensive memory usage. Previous works usually focus on reducing the number of trainable parameters in the network. While the model parameters do contribute to memory usage, the primary memory bottleneck during training arises from storing feature maps, also known as activations, as they are crucial for gradient calculation. Notably, machine learning models are typically trained using stochastic gradient descent.We argue that in stochastic optimization, models can handle noisy gradients as long as the gradient estimator is unbiased with reasonable variance.Following this motivation, we propose a new family of unbiased estimators called \sas, for matrix production with reduced variance, which only requires storing the sub-sampled activations for calculating the gradient.Our work provides both theoretical and experimental evidence that, in the context of tuning transformers, our proposed estimators exhibit lower variance compared to existing ones.By replacing the linear operation with our approximated one in transformers, we can achieve up to 2.7X peak memory reduction with almost no accuracy drop and enables up to $6.4\times$ larger batch size.Under the same hardware, \sas enables better down-streaming task performance by applying larger models and/or faster training speed with larger batch sizes.The code is available at https://anonymous.4open.science/r/WTACRS-A5C5/.

摘要:

随着模型大小的快速增长，由于其大量的内存使用，对大型预训练语言模型进行微调变得越来越困难。以前的工作通常侧重于减少网络中可训练参数的数量。虽然模型参数确实会影响内存使用，但训练期间的主要内存瓶颈来自于存储特征图（也称为激活），因为它们对于梯度计算至关重要。值得注意的是，机器学习模型通常使用随机梯度下降进行训练。我们认为，在随机优化中，只要梯度估计器无偏且具有合理的方差，模型就可以处理噪声梯度。遵循这一动机，我们提出了一个新的无偏估计器系列，称为\sas，对于方差减少的矩阵生成，只需要存储子采样激活来计算梯度。我们的工作提供了理论和实验证据，表明在调整变压器的背景下，我们提出的估计器与现有的相比表现出更低的方差通过用 Transformer 中的近似线性运算替换线性运算，我们可以在几乎没有精度下降的情况下实现高达 2.7 倍的峰值内存减少，并可实现高达 $6.4\times$ 的更大批量大小。在相同的硬件下，\sas 可以实现更好的性能通过应用更大的模型和/或更大批量大小的更快训练速度来降低下游任务性能。代码可在 https://anonymous.4open.science/r/WTACRS-A5C5/ 上获取。

## ProPILE: Probing Privacy Leakage in Large Language Models<sup>poster<sup>

Authors: Siwon Kim, Sangdoo Yun, Hwaran Lee, Martin Gubri, Sungroh Yoon, Seong Joon Oh

Link: [https://neurips.cc/virtual/2023/poster/71697](https://neurips.cc/virtual/2023/poster/71697)

Abstract:

 The rapid advancement and widespread use of large language models (LLMs) have raised significant concerns regarding the potential leakage of personally identifiable information (PII). These models are often trained on vast quantities of web-collected data, which may inadvertently include sensitive personal data. This paper presents ProPILE, a novel probing tool designed to empower data subjects, or the owners of the PII, with awareness of potential PII leakage in LLM-based services. ProPILE lets data subjects formulate prompts based on their own PII to evaluate the level of privacy intrusion in LLMs. We demonstrate its application on the OPT-1.3B model trained on the publicly available Pile dataset. We show how hypothetical data subjects may assess the likelihood of their PII being included in the Pile dataset being revealed. ProPILE can also be leveraged by LLM service providers to effectively evaluate their own levels of PII leakage with more powerful prompts specifically tuned for their in-house models. This tool represents a pioneering step towards empowering the data subjects for their awareness and control over their own data on the web.

摘要:

大型语言模型（LLM）的快速发展和广泛使用引起了人们对个人身份信息（PII）潜在泄露的严重担忧。这些模型通常是根据大量网络收集的数据进行训练的，其中可能会无意中包含敏感的个人数据。本文介绍了 ProPILE，这是一种新颖的探测工具，旨在使数据主体或 PII 所有者能够意识到基于 LLM 的服务中潜在的 PII 泄漏。 ProPILE让数据主体根据自己的PII制定提示，以评估法学硕士的隐私侵犯程度。我们在公开可用的 Pile 数据集上训练的 OPT-1.3B 模型上演示了其应用。我们展示了假设的数据主体如何评估其 PII 被包含在所揭示的 Pile 数据集中的可能性。 LLM 服务提供商还可以利用 ProPILE 来有效评估自己的 PII 泄漏水平，并提供专门针对其内部模型调整的更强大的提示。该工具代表着向数据主体增强其对网络上自己数据的认识和控制权迈出的开创性一步。

## M3Exam: A Multilingual, Multimodal, Multilevel Benchmark for Examining Large Language Models<sup>poster<sup>

Authors: Wenxuan Zhang, Mahani Aljunied, Chang Gao, Yew Ken Chia, Lidong Bing

Link: [https://neurips.cc/virtual/2023/poster/73506](https://neurips.cc/virtual/2023/poster/73506)

Abstract:

 Despite the existence of various benchmarks for evaluating natural language processing models, we argue that human exams are a more suitable means of evaluating general intelligence for large language models (LLMs), as they inherently demand a much wider range of abilities such as language understanding, domain knowledge, and problem-solving skills. To this end, we introduce M3Exam, a novel benchmark sourced from real and official human exam questions for evaluating LLMs in a multilingual, multimodal, and multilevel context. M3Exam exhibits three unique characteristics: (1) multilingualism, encompassing questions from multiple countries that require strong multilingual proficiency and cultural knowledge; (2) multimodality, accounting for the multimodal nature of many exam questions to test the model's multimodal understanding capability; and (3) multilevel structure, featuring exams from three critical educational periods to comprehensively assess a model's proficiency at different levels. In total, M3Exam contains 12,317 questions in 9 diverse languages with three educational levels, where about 23\% of the questions require processing images for successful solving. We assess the performance of top-performing LLMs on M3Exam and find that current models, including GPT-4, still struggle with multilingual text, particularly in low-resource and non-Latin script languages. Multimodal LLMs also perform poorly with complex multimodal questions. We believe that M3Exam can be a valuable resource for comprehensively evaluating LLMs by examining their multilingual and multimodal abilities and tracking their development. Data and evaluation code is available at \url{https://github.com/DAMO-NLP-SG/M3Exam}.

摘要:

尽管存在各种评估自然语言处理模型的基准，但我们认为，人类考试是评估大语言模型（LLM）一般智力的更合适的方法，因为它们本质上需要更广泛的能力，例如语言理解、领域知识和解决问题的能力。为此，我们推出了 M3Exam，这是一种新颖的基准，源自真实和官方的真人考试问题，用于在多语言、多模式和多层次的背景下评估法学硕士。 M3Exam呈现出三个独特的特点：（1）多语言性，涵盖多个国家的问题，需要很强的多语言能力和文化知识； （2）多模态，考虑很多试题的多模态性质，测试模型的多模态理解能力； （3）多层次结构，以三个关键教育时期的考试为特色，综合评估模型在不同层次的熟练程度。 M3Exam 总共包含 9 种不同语言、三个教育级别的 12,317 个问题，其中约 23% 的问题需要处理图像才能成功解决。我们评估了 M3Exam 上表现最好的法学硕士的表现，发现当前模型（包括 GPT-4）仍然难以处理多语言文本，特别是在资源匮乏和非拉丁文字语言中。多模式法学硕士在处理复杂的多模式问题时也表现不佳。我们相信，M3Exam 可以通过检查法学硕士的多语言和多模式能力并跟踪他们的发展，成为全面评估法学硕士的宝贵资源。数据和评估代码可在 \url{https://github.com/DAMO-NLP-SG/M3Exam} 获取。

## BenchCLAMP: A Benchmark for Evaluating Language Models on Syntactic and Semantic Parsing<sup>poster<sup>

Authors: Subhro Roy, Samuel Thomson, Tongfei Chen, Richard Shin, Adam Pauls, Jason Eisner, Benjamin Van Durme

Link: [https://neurips.cc/virtual/2023/poster/73488](https://neurips.cc/virtual/2023/poster/73488)

Abstract:

 Recent work has shown that generation from a prompted or fine-tuned language model can perform well at semantic parsing when the output is constrained to be a valid semantic representation. We introduce BenchCLAMP, a Benchmark to evaluate Constrained LAnguage Model Parsing, that includes context-free grammars for seven semantic parsing datasets and two syntactic parsing datasets with varied output meaning representations, as well as a constrained decoding interface to generate only valid outputs covered by these grammars. We provide low, medium, and high resource splits for each dataset, allowing accurate comparison of various language models under different data regimes. Our benchmark supports evaluation of language models using prompt-based learning as well as fine-tuning. We benchmark seven language models, including two GPT-3 variants available only through an API. Our experiments show that encoder-decoder pretrained language models can achieve similar performance or even surpass state-of-the-art methods for both syntactic and semantic parsing when the model output is constrained to be valid.

摘要:

最近的工作表明，当输出被限制为有效的语义表示时，从提示或微调的语言模型生成可以在语义解析中表现良好。我们引入了 BenchCLAMP，一个评估约束语言模型解析的基准，其中包括七个语义解析数据集的上下文无关语法和两个具有不同输出含义表示的句法解析数据集，以及一个约束解码接口，用于仅生成这些数据覆盖的有效输出语法。我们为每个数据集提供低、中、高资源划分，允许在不同数据体系下准确比较各种语言模型。我们的基准测试支持使用基于提示的学习和微调来评估语言模型。我们对七种语言模型进行了基准测试，其中包括两种仅通过 API 提供的 GPT-3 变体。我们的实验表明，当模型输出被限制为有效时，编码器-解码器预训练语言模型可以实现类似的性能，甚至超越句法和语义解析的最先进方法。

## UP-DP: Unsupervised Prompt Learning for Data Pre-Selection with Vision-Language Models<sup>poster<sup>

Authors: Xin Li, Sima Behpour, Thang Long Doan, Wenbin He, Liang Gou, Liu Ren

Link: [https://neurips.cc/virtual/2023/poster/71462](https://neurips.cc/virtual/2023/poster/71462)

Abstract:

 In this study, we investigate the task of data pre-selection, which aims to select instances for labeling from an unlabeled dataset through a single pass, thereby optimizing performance for undefined downstream tasks with a limited annotation budget. Previous approaches to data pre-selection relied solely on visual features extracted from foundation models, such as CLIP and BLIP-2, but largely ignored the powerfulness of text features. In this work, we argue that, with proper design, the joint feature space of both vision and text can yield a better representation for data pre-selection. To this end, we introduce UP-DP, a simple yet effective unsupervised prompt learning approach that adapts vision-language models, like BLIP-2, for data pre-selection. Specifically, with the BLIP-2 parameters frozen, we train text prompts to extract the joint features with improved representation, ensuring a diverse cluster structure that covers the entire dataset. We extensively compare our method with the state-of-the-art using seven benchmark datasets in different settings, achieving up to a performance gain of 20\%. Interestingly, the prompts learned from one dataset demonstrate significant generalizability and can be applied directly to enhance the feature extraction of BLIP-2 from other datasets. To the best of our knowledge, UP-DP is the first work to incorporate unsupervised prompt learning in a vision-language model for data pre-selection.

摘要:

在本研究中，我们研究了数据预选择的任务，其目的是通过单次从未标记的数据集中选择用于标记的实例，从而在有限的注释预算下优化未定义的下游任务的性能。以前的数据预选方法仅依赖于从基础模型（例如 CLIP 和 BLIP-2）中提取的视觉特征，而很大程度上忽略了文本特征的强大功能。在这项工作中，我们认为，通过适当的设计，视觉和文本的联合特征空间可以为数据预选择提供更好的表示。为此，我们引入了 UP-DP，一种简单而有效的无监督即时学习方法，它采用视觉语言模型（如 BLIP-2）进行数据预选择。具体来说，在冻结 BLIP-2 参数的情况下，我们训练文本提示来提取具有改进表示的联合特征，确保覆盖整个数据集的多样化集群结构。我们在不同设置下使用七个基准数据集将我们的方法与最先进的方法进行了广泛比较，实现了高达 20% 的性能增益。有趣的是，从一个数据集学到的提示表现出显着的通用性，可以直接应用于增强 BLIP-2 从其他数据集的特征提取。据我们所知，UP-DP 是第一个将无监督即时学习纳入视觉语言模型以进行数据预选的工作。

