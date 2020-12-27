# Amazing AI
notes on paper and news I have read

[Distilling the Knowledge in a Neural Network](https://arxiv.org/pdf/1503.02531.pdf)

（Globally and Locally Consistent Image Completion）[http://iizuka.cs.tsukuba.ac.jp/projects/completion/data/completion_sig2017.pdf]
解决了传统CV方法无法修补背景中不存在相似像素的情况，同时也可以修补比较大的空缺区域。
实现方法是：1. 借鉴图像数据库搜索相似patch的做法，同时GAN网络学习图像分布；2.采用空洞卷积扩大CNN的感知范围，从而可以生成更大的语义像素；3.采用局部和全局两个鉴别器，来监督生成器提供语义合理同时过度自然的填充像素。

[deepfill v1](https://arxiv.org/abs/1801.07892)
借鉴了Globally and Locally Consistent Image Completion的local and global critic思路，也借鉴了patch match的局部填充思路来提高边缘的平滑效果。
提出contexture attention的layers,并加入到local critic分支中，使得模型兼顾了DL方法的语义理解又兼顾了传统方法的平滑边缘过渡。

[deepfill v2](https://arxiv.org/abs/1806.03589)
使用Gating卷积神经网络来做图片缺失区域的修补。输入数据有图片、自动mask图片和sketch图片.mask用于图片区域擦除，而sketch则是用于图像编辑。

