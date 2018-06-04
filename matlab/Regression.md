# 回归算法小结
这里的回归计算方法来自MATLAB的Statistics and Machine Learning Toolbox。包括数据的组织，模型的设定，和结果的简单分析。
## 回归数据类型-table
MATLAB回归分析可以使用普通的矩阵和向量作为输入条件，但为了更方便的进行模型设置和结果展示，使用table数据类型是一个更好的选择。此外，统计和机器学习工具箱定义了dataset数据类型，与table数据类型起到同样的作用，但可能在未来的版本中被取消，所以这里仅以table类型进行说明。

table类型数据可以通过整合工作空间现有变量的方式来生成。

>\>\> tbl1 = readtable('hospital.xls','ReadRowNames',true)

而当数据被导入以后，就可以使用fitlm函数来获得线性模型。

>\>\> mdl = fitlm(tbl1,'sys ~ 1 + sex+ age + smoke')

结果显示为：

>mdl = 
>
>
>Linear regression model:
>    sys ~ 1 + sex + age + smoke
>
>Estimated Coefficients:
>                   Estimate        SE         tStat        pValue  
>                   _________    ________    _________    __________
>
>    (Intercept)       116.19      2.7171       42.762     2.639e-64
>    sex_f          -0.050106     0.98364    -0.050939       0.95948
>    age             0.085276    0.066945       1.2738        0.2058
>    smoke               9.87      1.0346       9.5395    1.4516e-15
>
>
>Number of observations: 100, Error degrees of freedom: 96
>Root Mean Squared Error: 4.78
>R-squared: 0.507,  Adjusted R-Squared 0.492
>F-statistic vs. constant model: 33, p-value = 9.91e-15
