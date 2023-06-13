# GAN
代码来自：https://blog.csdn.net/qq_39547794/article/details/125389000
我们对其做了一些改进，主要有：  
1. 增加了amp
2. 将日志保存到txt文件中
3. 原网络对generator的训练效果不是很好，我们在每次训练中额外增加了两次对generator的训练（所以现在discriminator的效果不是很好了
   - 而且因为discriminator的效果不好，反而降低了generator的训练效果
## TODO
1. 将discriminator与generator的训练比例维护为一个输入参数
2. 重新组织代码结构，使其易于维护
3. 当generator和discriminator训练次数为1：1时，结果生成出的数字大多为1.需要考虑如何生成更丰富的数字。(引入罚分机制)