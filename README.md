# WaLiCode - 小傅哥出品，研发自己人的 AI IDE Coding !

作者：小傅哥
<br/>官网：[https://walicode.xiaofuge.cn](https://walicode.xiaofuge.cn/)

> 沉淀、分享、成长，让自己和他人都能有所收获！😄

大家好，我是技术UP主小傅哥！

得益于 Claude Code 的被动开源 😂 （~~怀疑是故意的~~），市面上出现了非常多的 Claude Code 源码架构设计分析，这也让我们看到了非常精彩的
AI Agent 运行时设计技巧。按照剧本套路，我们使用的 AI IDE 将迎来一大波迭代升级。**嘿嘿，但这次，我先下手啦！**

<div align="center">
	<img src="https://bugstack.cn/images/article/project/ai-rag-knowledge/ai-rag-knowledge-0-00.png" width="150px"/>
</div>

**小傅哥的 WaLiCode，AI IDE Coding v0.1.0 发布！**

市面上优秀的 AI IDE 非常多，但论最好用的还得是 Claude Code。所以借助于这些的“源码”学习，小傅哥基于 Tauri（Rust）桥接 Claude
Code 能力（这个设计也可以桥接其他的，如 OpenCode），在上层做一套 AI IDE 应用服务实现。通过工程、工程、代码块（含图片）对话的方式，驱动代码开发辅助提效处理。
`也让大家可以通过 WaLiCode 感受到 Claude Code 的巴士体验！`

<div align="center">
	<img src="https://bugstack.cn/images/article/product/software/product-walicode-00.png" width="350px"/>
</div>

> WaLiCode 产品功能还在快速迭代中，可以扫码加入群聊，关注最新动态和讨论使用！

## 一、产品介绍

**产品官网**：[https://walicode.xiaofuge.cn/](https://walicode.xiaofuge.cn/)  - 提供了下载安装包（
`如果遇到什么bug，可以群里交流`）。

WaLiCode，本地运行的 AI 编程助手。基于 Tauri + Claude Code 底层能力桥接，深度集成文件系统与终端，让 AI 真正帮你写代码，而不只是给建议。更为重要的是你可以，你可以直接本地安装 WaLiCode 就能体验到 Claude Code 的编码能力！

在辅助编码中，可以直接把代码块、文件、图片放入对话框作为上下文，AI 会结合项目结构与依赖关系给出更准确的修改建议，并可通过
Diff 预览后安全应用到本地代码。

但当然，我还是一个配角，小配角！我还有很多功能需要迭代，让研发伙伴使用这款工具，可以在学习源码、了解项目、深入功能、俯瞰架构等方面，都能有所帮助。
**好吧，让我们一起期待，WaLiCode 的迭代！**

## 二、使用演示

### 1. 模型配置

<div align="center">
	<img src="https://bugstack.cn/images/article/product/software/product-walicode-06.png" width="850px"/>
</div>

- 多厂家模型灵活配置，支持自定义 OpenAI 格式的各类大模型接口，无论是智谱、火山引擎还是本地部署的模型，均可一键接入，满足不同场景的开发需求。
- 各类的 token/coding plan，支持 OpenAI 格式就可以配置使用。

### 2. 产品首页

<div align="center">
	<img src="https://bugstack.cn/images/article/product/software/product-walicode-01.png" width="850px"/>
</div>

- 首先，安装软件后，打开 WaliCode 在初次使用会引导你配置 apikey，可以添加你需要的模型。得益于 Claude Code 和 WaliCode
  的扩展，上下文的使用会非常准确和节省，也就让你的模型消耗也会很低。
- 之后，你可以打开文件夹选择自己的工程，进行对话框对话，以及智能终端对话。在对话中，你可以把模块、文件、代码以及图片，都放到对话框中，之后进行诉求描述。

### 3. 添加技能（Skills）

<div align="center">
	<img src="https://bugstack.cn/images/article/product/software/product-walicode-02.png" width="850px"/>
</div>

- 在设置中可以添加你需要扩展的 Skills 技能，支持zip包上传、git地址直接拉取，可以非常方便的扩展 Skills。
- 同时还为你提供了 SkillMP、ClawHub 官网 Skills 地址，随时去找你需要的技能扩展到工程里。

### 4. 添加服务（MCP）

<div align="center">
	<img src="https://bugstack.cn/images/article/product/software/product-walicode-03.png" width="850px"/>
</div>

- 在设置中可以添加 MCP 服务能力，支持 stdio、sse、json 多种配置方式。极大的方便用户扩展自己的功能使用场景。

### 5. 智能终端

<div align="center">
	<img src="https://bugstack.cn/images/article/product/software/product-walicode-04.png" width="850px"/>
</div>

- 这是一个附属功能，方便用户可以在终端直接使用 Claude Code 能力。属于原生的扩展支持。

### 6. Git 能力

<div align="center">
	<img src="https://bugstack.cn/images/article/product/software/product-walicode-07.png" width="850px"/>
</div>

- 内置 Git 操作面板，支持分支切换、代码提交与状态查看。结合 AI 能力，还能自动分析变更并生成规范的提交信息。

> 好嘞，欢迎下载体验 [https://walicode.xiaofuge.cn/](https://walicode.xiaofuge.cn/) 遇到问题可以群里交流 😄

## 三、扩展学习（AI Agent）

如果你希望自己不只是一个业务开发工程师，也具备 AI Agent 开发能力，让自己在这个 AI
时代做点什么，那么下面的教程你可以学习下。小傅哥也是在这些项目中积累的经验，可以一次次在 AI 快速迭代中，做一些有意思的事情。

<div align="center">
	<img src="https://bugstack.cn/images/article/project/ai-agent-scaffold/part-1/1-1/images/ai-agent-scaffold-1-1-10.png" width="650px"/>
</div>

小傅哥的社群星球「码农会锁」，现已经有20个实战项目，6个AI、5个业务、8个组件 + 1套源码（MyBatis），这6个AI项目，你可以按需选择学习。[项目地址 Go!](https://bugstack.cn/md/project/ai-agent-scaffold/ai-agent-scaffold.html)



