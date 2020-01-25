### About PLD-UAV
Power line detection plays an important role in an automated UAV-based electricity inspection system, which is crucial for real-time motion planning and navigation along power lines. Although previous approaches have achieved great improvements, they are mainly developed on top of several sample images or synthetic ones due to the lack of power line datasets, which may be inappropriate for learning-based methods. To overcome this, we introduce two power line detection datasets with pixel-wise annotations, power line dataset of urban scene (**PLDU**) and power line dataset of mountain scene (**PLDM**). The detailed information of the two datasets is listed below. These images contain complex backgrounds and power lines with different features. All images are manually annotated with boundary labels. Besides, standard data augmentation techniques, including rotation, flipping and resizing have been performed for optional use. We evaluate several state-of-the-art power line detection methods on the two datasets. Experimental results demonstrate that accurate power line detection on the two datasets is quite a challenging task. **PLDU and PLDM are publicly available, including the raw data and ground truth.** 



电力线检测在基于无人机的自动化电力检查系统中扮演着重要角色，这对于实时运动规划和沿电力线导航至关重要。尽管以前的方法已经取得了很大的进步，但是由于缺乏电力线数据集，它们主要在几个样本图像或合成图像的基础上开发，这可能不适用于基于学习的方法。为了克服这个问题，我们引入了两个带有像素注释的电源线检测数据集，即城市场景的电源线数据集（PLDU）和山地场景的电源线数据集（PLDM）。下面列出了这两个数据集的详细信息。这些图像包含复杂的背景和具有不同功能的电源线。所有图像均使用边界标签手动注释。此外，已经进行了包括旋转，翻转和调整大小在内的标准数据增强技术以供可选使用。我们评估了两个数据集上几种最新的电力线检测方法。实验结果表明，在两个数据集上进行准确的电力线检测是一项艰巨的任务。 PLDU和PLDM是公开可用的，包括原始数据和基本事实。

Dataset | Train | Test | Size | maxDist
------ | ------| ------| ------| ------
PLDU | 453 | 120 | 540X360 | 0.0075
PLDM | 237 | 50 | 540X360 | 0.0075


### PLDU
Here are some samples from PLDU. The dataset is available on [Google Drive](https://drive.google.com/open?id=1XjoWvHm2I8Y4RV_i9gEd93ZP-KryjJlm)

![sample1](PLDU.jpg)

### PLDM
Here are some samples from PLDM. The dataset is available [Google Drive](https://drive.google.com/open?id=1bKFEuXKHRsy0tnOnoEVW6oRi7hS5oekr)

![sample2](PLDM.jpg)

### Benchmark
For evaluation, we refer to the boundary detection benchmark developed in [BSDS500](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/resources.html) dataset.
The accuracy of power line detection is measured using four main criteria: F1-measure of optimal
dataset scale threshold (ODS), F1-measure of optimal image scale threshold (OIS), false positive rate and
precision-recall curve.


基准测试
为了进行评估，我们参考了BSDS500数据集中开发的边界检测基准。
电力线检测的准确性使用以下四个主要标准来衡量：
1.F1最佳数据集比例阈值（ODS）的度量
2.F1最佳图像比例阈值OIS的度量
3.误报率
4.精确调用曲线。
