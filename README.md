## 基于 TensorFlow 与 Keras 卷积神经网络的猫类图像识别

东北大学 2017 年数学建模第四次模拟题目。与 @lyx988、@Lee-faner 合力完成。

最终测试集准确率 90.0%，loss 0.29。

### 题目

You are given a dataset ("*.h5") containing:

- a training set of train_catvnoncat.h5 file labeled as cat (y=1) or non-cat (y=0)
- a test set of test_catvnoncat.h5 file labeled as cat or non-cat
- each image is of shape (height, width, 3) where 3 is for the 3 channels (RGB).

No.1-3 in the "images" directory are the test images.  Of course, you can also select the other cat or non-cat images freely. 

You will build a simple image-recognition model that can correctly classify pictures as cat or non-cat.

### 基本思路

卷积神经网络

-   四层卷积：输入层 3 层（RGB）、16、32、64、128，ReLU
-   一层前馈：1024 个神经元，ReLU
-   输出：sigmoid（二分类）