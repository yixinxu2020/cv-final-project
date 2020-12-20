# cv-final-projectData proprecess
## Data proprecess
### Ben Graham's preprocessing method & center crop（即在这里的scale radius）
2015年的类似比赛Diabetic Retinopathy Detection 第一名Ben的预处理方案。简单来说就是改善图片亮度不一致的情况，同时对图片做center crop，去除黑边，具体可参考如下kernel:
> https://www.kaggle.com/ratthachat/aptos-eye-preprocessing-in-diabetic-retinopathy#2.-Try-Ben-Graham's-preprocessing-method.
### Pseudo Labeling
> https://www.kaggle.com/cdeotte/pseudo-labeling-qda-0-969
> 伪标记是将可靠的预测测试数据添加到训练数据的过程。
5个步骤：
使用训练数据建立模型。
预测未知的测试数据集的标签。
在我们的训练数据中添加可信的预测测试观察结果。
使用组合数据构建新模型。
使用新模型预测测试数据。
## Extra data
2015 kaggle Diabetic Retinopathy (resized)
> https://www.kaggle.com/tanlikesmath/diabetic-retinopathy-resized
## 模型集成(Ensemble)
将所有的data分成5个folder，分别train得到5个basic model，再进行ensemble
