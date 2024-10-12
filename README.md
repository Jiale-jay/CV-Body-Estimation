# CV-Body-Estimation
姿态估计
姿态估计是在Object Detection基础上进一步发展而来的CV垂直领域应用，通常用于AR、影视行业动态捕捉追踪、安防动作识别、仿生机器人模仿学习等领域。并且在行业中还逐渐分化为头部姿态、手部姿态、身体姿态三个方向，分别应用于不同领域的需求。
在接下来的两周，我们要探索深度学习的Body Estimation方法。深度学习的姿态估计的算法某种意义上来说是Object Detection的变体，但在定位和跟踪上有更为复杂的处理。
在该环节之后的算法可能会涉及一些我们在Week1-2中没有提及过的基分类器，希望你能够自行简单了解，实习期间不再给出更多的reference。
任务1
Openpose
https://arxiv.org/pdf/1611.08050.pdf
https://github.com/CMU-Perceptual-Computing-Lab/openpose
https://blog.csdn.net/cjnewstar111/article/details/115284760
https://zhuanlan.zhihu.com/p/37526892
https://www.jianshu.com/p/98c11545d4fb
仪态识别我们不可能绕过的算法就是Openpose。
Openpose是业界第一个能够做到近实时能力的仪态识别系统，并且随着不断地维护迭代，Openpose已经支持了2D环境下的人体、面部、脚部、手部姿态估计，以及3D的人体姿态估计和重建。
Openpose的内容过于庞大，本次实习仅需要涉及2D的人体骨架识别。
任务1需要你在读完论文和参考链接并且本机跑通Openpose开箱即用的模型后，写一篇文章阐述你对Openpose的2D人体骨架识别的算法理解。
任务2
Openpose是近实时人体姿态赛估计算法的开山鼻祖，然而其算法非常重和复杂，因而导致在多数很强大的工作站上运行都无法达成实时（~30fps）能力。在Openpose面世后的数年来，业界一直有围绕它的迭代和优化方法产生。其中一个里程碑是Lightweight Openpose，它实现了真正的2D实时姿态估计能力：
Lightweight Openpose
https://arxiv.org/pdf/1811.12004.pdf
https://github.com/Daniil-Osokin/lightweight-human-pose-estimation.pytorch
https://zhuanlan.zhihu.com/p/478854529
https://aitechtogether.com/article/31642.html
在本任务，你需要实现TF2.0环境下的Lightweight openpose。@murdockhou已经有一个Tensorflow的实现，对TF2.0的支持仍处于实现性阶段。你可以以此为基础进行调试并找出问题。
https://github.com/murdockhou/lightweight_openpose/tree/tf2.0_version
