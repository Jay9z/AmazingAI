# Amazing AI
notes on paper and news I have read

[Distilling the Knowledge in a Neural Network](https://arxiv.org/pdf/1503.02531.pdf)

[deepfill v1](https://arxiv.org/abs/1801.07892)
借鉴了Globally and Locally Consistent Image Completion的local and global critic思路，也借鉴了patch match的局部填充思路来提高边缘的平滑效果。
提出contexture attention的layers,并加入到local critic分支中，使得模型兼顾了DL方法的语义理解又兼顾了传统方法的平滑边缘过渡。

[deepfill v2](https://arxiv.org/abs/1806.03589)
使用Gating卷积神经网络来做图片缺失区域的修补。输入数据有图片、自动mask图片和sketch图片.mask用于图片区域擦除，而sketch则是用于图像编辑。

