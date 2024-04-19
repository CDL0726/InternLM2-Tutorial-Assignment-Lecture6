# InternLM2-Tutorial-Assignment-Lecture6
# Lagent & AgentLego 智能体应用搭建    
2024.4.17   Lagent&AgentLego 核心贡献者 樊奇   

[Lagent](https://github.com/InternLM/Lagent)    
[AgentLego](https://github.com/InternLM/AgentLego)   

[第6课 视频](https://www.bilibili.com/video/BV1Xt4217728/)    
[第6课 文档](https://github.com/InternLM/Tutorial/tree/camp2/agent)    
[第6课 作业](https://github.com/InternLM/Tutorial/blob/camp2/agent/homework.md)    


论文：    
[Agent-FLAN 技术报告](https://arxiv.org/abs/2403.12881)    
[Repo](https://github.com/InternLM/Agent-FLAN)    

# 第6课 笔记   

## 理论课程    

###  为什么要有智能体 

大语言模型存在局限性：
  - 幻觉: 模型可能会生成虚假信息、与现实严重不符或脱节。
  - 时效性： 模型训练数据过时，无法反映最新趋势和信息。
  - 可靠性问：面对复杂任务时，可能频发错误输出现象，影响信任度。

![](./Agent1.png)       

### 什么是智能体          

智能体概念的第一次提出： Hayes-Roth 1995, An Architecture for Adaptive Intelligent Systems.    
一个智能体需要满足以下3个条件：     

1. Perception of dynamic conditions in the environment
可以感知环境中的动态条件。

2. Action to affect conditions in the environment
能采取动作影响环境。

3. Reasoning to interpret perceptions, solve problems, draw inferences, and determine actions.    
能运用推理能力理解信息、解决问题，产生推断、决定动作。

![](./Agent2.png) 

智能体组成：    

  1. 大脑：作为控制器，承担记忆、思考和决策任务。接收来自感知和模块的信息，并采取相应动作。
     
  2. 感知：对外部环境的多模态信息进行感知和处理。包括但不限于图像、音频、视频、传感器等。
     
  3. 动作： 利用并执行工具以影响环境。工具可能包括文本的检索、调用相关API、操控机械臂等。

![](./Agent3.png)     

### 智能体范式     
- AutoGPT
- ReWoo
- ReAct

### Lagent & AgentLego   

1. Lagent  

Lagent 是一个轻量级开源智能体框架，旨在让用户可以高效地构建基于大语言模型的智能体。同时它也提供了一些典型工具以增强大语言模型的能力。

Lagent 目前已经支持了包括 AutoGPT、ReAct 等在内的多个经典智能体范式，也支持了如下工具：

 - Arxiv 搜索
 - Bing 地图
 - Google 学术搜索
 - Google 搜索
 - 交互式 IPython 解释器
 - IPython 解释器
 - PPT
 - Python 解释器

![](./Agent4.png) 

2. AgentLego   

AgentLego 是一个提供了多种开源工具 API 的多模态工具包，旨在像是乐高积木一样，让用户可以快速简便地拓展自定义工具，从而组装出自己的智能体。通过 AgentLego 算法库，不仅可以直接使用多种工具，也可以利用这些工具，在相关智能体框架（如 Lagent，Transformers Agent 等）的帮助下，快速构建可以增强大语言模型能力的智能体。    

AgentLego 目前提供了如下工具：    

![](./Agent5.png) 

![](./Agent6.png)    

3. Lagent 与 AgentLego 两者的关系

 Lagent 是一个智能体框架，而 AgentLego 与大模型智能体并不直接相关，而是作为工具包，在相关智能体的功能支持模块发挥作用。   

两者之间的关系可以用下图来表示：    

![](./Agent7.png)







# 第6课 作业        



