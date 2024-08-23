# AI

* [重磅 | 完备的 AI 学习路线，最详细的资源整理！ ](https://mp.weixin.qq.com/s?__biz=MzIyNjM2MzQyNg==&mid=2247484443&idx=1&sn=7110e42ef9e95a8c16064dde5b897960)
> from 微信公众号 Datawhale，作者：AIUnion

* [antlr4](https://github.com/antlr/antlr4)

## 神经网络
* [人人都能搞定的大模型原理 - 神经网络](https://mp.weixin.qq.com/s?__biz=MzUxNjI3NTg4Mg==&mid=2247483844&idx=1&sn=a63d5d5b825b96ad7b9b342ef7b8ad64)

## AI 算法
* [Stylized Neural Painting 为艺术而生的算法](https://github.com/jiupinjia/stylized-neural-painting)
  > [算法根据我们提供的图片，自动一笔一划地创作油画](https://mp.weixin.qq.com/s/qtNei4A7Zgr4qBDbKnnyXg)  
  > [paper](https://arxiv.org/abs/2011.08114)
* [中国山水画 alicex2020/Chinese-Landscape-Painting-Dataset](https://github.com/alicex2020/Chinese-Landscape-Painting-Dataset)

## NLP
* [Awesome-Chinese-NLP](https://github.com/crownpku/Awesome-Chinese-NLP)
* [【腾讯人工智能实验室】TexSmart: 文本理解工具与服务](https://ai.tencent.com/ailab/nlp/texsmart/zh/index.html#instructions)

## 推荐系统
* [推荐一个国人开源的推荐系统 gorse: Go Recommender System Engine](https://mp.weixin.qq.com/s/j_tNX6W4A-LKCmwM_Bc98g)
  > https://github.com/zhenghaoz/gorse

## 大模型 LLM
* [掌握Prompt写作技巧：写出完美Prompt的秘籍](https://mp.weixin.qq.com/s/NsRY_hEUSEZbubWYK1_1RQ)
* 上下文
  > 在AI大模型中，“上下文长度”指的是模型在一次输入中能够处理的最大字符或标记（tokens）数量。这个上下文包括输入的所有内容，例如问题、对话历史、文档文本等。
  > 模型的上下文长度决定了它在单次推理中能够考虑的最大信息量。
  > 
  > - 1. 上下文长度的含义  
  >   上下文长度 是模型在一次输入中可以处理的最大标记数量。标记可以是单个字母、词语，甚至是词的一部分，取决于具体的模型和语言处理方式。  
  >   比如，如果一个模型的上下文长度是 2048 tokens，那么它一次最多能处理 2048 个标记。如果输入超过了这个长度，模型将无法考虑超出的部分，或者需要对输入进行截断。  
  > 
  > - 2. 128K的上下文长度意味着什么？  
  >   128K 的上下文长度意味着模型在单次输入中可以处理 128,000 个 tokens。这是一个非常大的上下文长度，远超大多数传统模型的上下文限制（通常在 2K 到 4K tokens 左右）。  
  >   这个上下文长度的优势在于，模型可以在一次处理更多的信息，无需频繁地对话或文本进行分割。对于需要处理长文档、复杂对话历史或上下文信息密集的任务（如编程代码、法律文书分析等），这种上下文长度非常有用。  
  >
  > - 3. 上下文长度的实际应用  
  >   在实际应用中，更长的上下文长度意味着模型可以在处理复杂任务时更有效地保持上下文一致性。例如，分析一本书的内容时，模型可以理解并处理整个章节，甚至更长的段落，而无需逐段分析。  
  >   在多轮对话中，长上下文长度允许模型记住更多的对话历史，从而提供更相关和一致的回复。  
  >
  > - 4. 上下文长度的局限性  
  >   尽管更长的上下文长度提供了更多的处理能力，但它也需要更多的计算资源。处理大量的 tokens 可能会导致更高的计算开销和内存使用，这对于一些资源受限的环境可能是一个挑战。  
  >   总结来说，128K 的上下文长度意味着该 AI 模型可以在单次推理中处理非常大量的信息，这是在处理复杂任务时的一个重要优势。然而，使用长上下文长度也需要考虑计算资源的平衡。  
