### 学习进度
Week 1
Video: VideoWhat is a Neural Network? ✔
. Duration: 7 minutes7 min

Video: VideoSupervised Learning with Neural Networks ✔
. Duration: 8 minutes8 min

Video: VideoWhy is Deep Learning taking off?
. Duration: 10 minutes10 min

Video: VideoAbout this Course
. Duration: 2 minutes2 min

Ungraded External Tool: Ungraded External ToolJoin us on Discourse!
. Duration: 1 hour1h

Reading: ReadingFrequently Asked Questions
. Duration: 10 minutes10 min

Lecture Notes (Optional)

Quiz

Heroes of Deep Learning (Optional)

# ML-notes

### 西瓜书 第三章 2022/03/22
本次学习了线性模型，线性模型拥有较好的可解释性，w矩阵中权值的大小，表达各个特征值的相对重要程度。线性模型也能有多种变式（对数线性回归模型、更一般地，广义线性模型）。线性模型的求参往往采用最小二乘法。线性回归模型的输出值是实数值，如果对输出值再套一层sigmoid函数，则该模型可用于分类问题，此时模型称为“对数几率回归”（logistic regression)（不要参考中文译名“逻辑回归”，十分具有误导性），这个模型的参数求解可以采用“极大似然法”。多分类学习问题，对数据集的拆分有大致三种方式：ovo,ovr,mvm。训练模型时，基本假设是不同类别的训练样例相当，否则训练出的模型泛化能力差。此问题的对策：欠采样、过采样、阈值移动。
