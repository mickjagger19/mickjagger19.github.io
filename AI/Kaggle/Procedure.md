
# 数据处理 Feature Exploration, Engineering and Cleaning
省略默认步骤（读取，确认问题类型,， Data Quality Check, Data Type Check等）
1. Plot
	* 分布: histogram, `sns.distplot(hue)`, `.skew()`, `.kurt()`, `sns.FacetGrid`
	* Correlation:
		* 特征 - 特征关系： `d.plot.scatter`
		* 特征 - 特征关系(category): `sns.boxplot`
	* **Pearson Correlation Plot**:   `sns.heatmap(d.corr())`
	* 特征 - 标签关系：`sns.pairplot`
2. 处理异常值
	* na: `d.isnull().sum().sort_values(ascending=False)`
		* `missingno.matrix`
	* nan: Impute
	* outliers
		* **boxplot**
		* 判断方法：`StandardScaler`， 多变量 scatter 图
3. 处理数据
	* norm: `StandardScaler([[]]`
	* 降维和聚类 
		* scatter plot
		* 降维：PCA, LDA, t-SNE
	* subsample
1. 检查 Label 和 features 的关系
	* **Normality**： Histogram +  Normality Prob Plot, np.log()
	* **Homoscedasticity**
	* **Linearity**
	* **Absence of correlated errors**
2. 选择 features (生成新features)
	* 删除
             *  缺失比例大于 15%
             *  和其他变量相关性很大
             * 
3. 转换为 numeric
	* categorical:
		*  One-hot: OHE, `pd.get_dummies`
		*  Labeler
	* Time series: hour, day, week, month, quarter, year



# 建模

## 模型

* classifier
	* Ensemble
		* ensemble.AdaBoostClassifier()
		* ensemble.BaggingClassifier()
		* ensemble.ExtraTreesClassifier()
		* ensemble.GradientBoostingClassifier()
		* ensemble.RandomForestClassifier()
	* Gaussian Processes
		* GaussianProcessClassifier()
	* GLM
		* linear_model.LogisticRegressionCV()
		* linear_model.PassiveAggressiveClassifier()
		* linear_model.RidgeClassifierCV()
		* linear_model.SGDClassifier()
		* linear_model.Perceptron()
	* Navies Bayes
		* BernoulliNB()
		* GaussianNB()
	* Neighbor
		* KNeighborsClassifier()
	* SVM
		* svm.SVC(probability=True)
		* svm.NuSVC(probability=True)
		* svm.LinearSVC()
	* Trees
		* tree.DecisionTreeClassifier()
		* tree.ExtraTreeClassifier()
	* Discriminant Analysis
		* LinearDiscriminantAnalysis()
		* QuadraticDiscriminantAnalysis(),
	* Logistic Regressor
	* Grid Search CV
	* perceptron
	* GBM
	* 

* regressor
	* ensemble
		* GradientBoostingRegressor
	* linear model
		* ElasticNet
		* SGDRegressor
		* BayesianRidge
		* LinearRegression
	* svm
		* SVR
	* kernel_ridge
		* KernelRidge
	* XGBRegressor
	* lightgbm

ensembles
* averaging: 取平均值
* rank average: 
* bagging
* blending
* stacking: 底层模型的输出作为 feature，使用 XGBoost 作为二级
* stacked generalization: 使用分类器组合其他分类器的输出
* feature weighted linear stacking

1. 分类 or 回归？多分类器 or 单个？ Ensemble ?


## 验证 Validation
1. 



# 预测

1. ensemble 
2. feature importance
	* 删除 / 添加 features(mean?)

## Ensemble
ensemble from un-related models(Correlation of models output)
* Voting: 









=======
* Voting: