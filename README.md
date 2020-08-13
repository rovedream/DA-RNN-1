# DA-RNN
根据 Seanny123 复现论文A Dual-Stage Attention-Based Recurrent Neural Network for Time Series Prediction的pytorch代码进行相关修改，适应pytorch1.2版本


1. 在原代码的基础上，进行了修改，使得其能够适应pytorch1.2版本，移除了Variable相关函数。
2. 在阅读了github上4篇关于这篇论文的复现之后，发现，bgithub1的数学公式推导部分与原文高度一致，而Seanny123等人的复现结果中，对公式8、12部分有所简化，（也可能是我才疏学浅，不知道这部分可以简化吧。。。）为了节省时间，我选择了Seanny123的公式部分的代码，如果有兴趣的同学，可以去bgithub1的相关代码下看看，相关的仓库我都已经start。
3. 在代码中，我发现Seanny123输入的inputdata，encoder模块中输入了前t-1个时间步的输入数据传入attention层中，但是在文章中的输入数据是前t个时间步的数据。为此，我在原代码的基础上，进行了相应的修改，修改部分的原代码均以注释的形式展现。
4. 我在文件中给出了两份代码数据，第一份NASDAQ_DARNN Seanny123 是根据Seanny123等人的相关工作进行的复现代码，加上了自己的注释便于去理解。在NASDAQ_DARNN是我对时间步进行了修改，以便于更好的实现原文。
5. 文章所有代码，均可在pytorch1.2环境下得以实现。Utils.utils_Pytorch包是本人的一些trick，可以直接去除不影响代码的整体运行。



### 最后，祝小米公司十周年快乐，也预祝8月17日的他生日快乐。
