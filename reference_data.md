###### 系列文章
1. 《Transformers快速入门》 https://transformers.run/  
**Abstract** TODO  
**阅读状态** doing  

2. 《探秘Transformer系列》 https://www.cnblogs.com/rossiXYZ/p/18785601  
    * 《注意力机制》https://www.cnblogs.com/rossiXYZ/p/18705809  
    **Abstract** 看完忘写了摘要了...  
    **阅读状态** 需要重看  

    * 《Transformer总体架构》 https://www.cnblogs.com/rossiXYZ/p/18706134  
    **Abstract** 介绍了Transformer中总体的结构，包括Encoder、Decoder中Attention的实现、FFN的实现。包含Transformer的实现代码，后面对Transformer多方面的解释感觉看起来有点费劲。  
    **阅读状态** done  

    * 《数据处理》、《编码器&解码器》 https://www.cnblogs.com/rossiXYZ/p/18722830、https://www.cnblogs.com/rossiXYZ/p/18727704  
    **Abstract** 《数据处理》介绍了加载数据的过程，包括padding，训练时候输入构建batch的方法，比较easy；《编码器&解码器》继续详解了两个模块里面的具体结构，并对encoder-decoder架构的模型进行了流程梳理；也提到了encoder-only和decoder-only架构的模型演进，随着bert带来最初的保障下增长后，encoder-only模型逐渐消失，目前仅剩encoder-decoder和decoder-only架构。并结合了相关文章，对这一现象进行了相关的解释。  
    **阅读状态** done  

    * 《训练&推理》https://www.cnblogs.com/rossiXYZ/p/18730583  
    **Abstract** 详细介绍了训练的代码实现，讲解了dropout、label_smooth正则化技术、noam learning rate（包含warmup和decay两部分，学习率先增后减）、  teacher forcing加速训练方法（通过给模型提供每一步的正确输出作为指导，来实现让自回归（逐字输出）的模型实现并行化的训练）等训练技术，同时给出了基本训练架构的代码；简要介绍了下推理和训练中的输入输出&流程中的区别。  
    **阅读状态** done  

    * 《token》、《embedding》、《位置编码》、《位置编码分类》、《自注意力》、《掩码》、《多头自注意力》
    **Abstract** 介绍了将原始query用分词器分词、获取embedding、给embedding增加位置编码，自注意力，掩码，MHA等（emmm，感觉我这abstract跟没写一样）
    **阅读状态** done（一次看的比较多，没及时记录详情。。）



###### 预训练技术  
1. 《从Word Embedding到Bert模型—自然语言处理中的预训练技术发展史》 https://zhuanlan.zhihu.com/p/49271699  
**Abstract** 介绍了自然语言处理中的预训练技术的发展，其中主要介绍了 Word2Vec（获取词向量）、ELMO（新增双向LSTM，给词向量新增上下文语义特征、句法特征，解决多义词相同embedding问题，双向语言模型）、GPT-1（预训练+下游任务Fine-tuning两阶段，使用Transformer特征抽取器，单向语言模型）、Bert（使用Transformer特征抽取、通过mask根据上下文猜词实现双向语义特征提取，双向语言模型）  
**阅读状态** done  

2. 《》