# 机器学习月考实战项目

基于 Python + scikit-learn 的机器学习分类实战，包含 **3 个独立实验**，覆盖数据清洗、特征工程、模型训练、网格搜索调参与多指标评估的完整流程。

## 📚 三个实验

### 实验1：金融欺诈检测（`first_exam.ipynb`）
- **任务**：二分类，预测信用卡交易是否欺诈
- **数据**：信用卡交易训练数据 / 测试数据（1000 条训练样本，5 个特征）
- **模型**：逻辑回归 + 随机森林，网格搜索（GridSearchCV）调参
- **评估**：准确率、F1 分数、ROC 曲线与 AUC
- **亮点**：特征重要性 / 逻辑回归斜率系数分析

### 实验2：苹果品质预测（`second_exam.ipynb`）
- **任务**：分类，预测苹果品质等级
- **模型**：决策树（DecisionTreeClassifier）
- **调参**：3 折交叉验证 + 网格搜索
- **评估**：调优前后准确率对比、多个指标评估、ROC 曲线

### 实验3：餐饮客户满意度预测（`third_exam.ipynb`）
- **任务**：分类，预测餐饮客户满意度
- **数据**：餐饮客户满意度.csv
- **模型**：XGBoost + GBDT，网格搜索调参
- **评估**：模型性能评估，保存最优模型 `best_satisfaction_model.pkl`

## 🛠 技术栈

Python | Pandas | NumPy | Scikit-learn | Matplotlib | XGBoost

## 📁 目录结构

```
ml-month3-exam/
├── first_exam.ipynb              # 实验1：金融欺诈检测
├── second_exam.ipynb             # 实验2：苹果品质预测
├── third_exam.ipynb              # 实验3：餐饮客户满意度预测
├── best_satisfaction_model.pkl   # 实验3训练的最优模型
├── 数据/
│   ├── 信用卡交易训练数据.xlsx
│   ├── 信用卡交易测试数据.xlsx
│   └── 餐饮客户满意度.csv
├── requirements.txt
└── README.md
```

## 🚀 运行方式

```bash
# 1. 安装依赖
pip install -r requirements.txt

# 2. 用 Jupyter 打开实验文件逐个运行
jupyter notebook first_exam.ipynb
jupyter notebook second_exam.ipynb
jupyter notebook third_exam.ipynb
```

## 📌 说明

- 数据文件与 notebook 使用相对路径读取，克隆仓库后可直接运行
- `best_satisfaction_model.pkl` 为训练产物，体积较小，一并提交便于直接加载演示
- 模型仅用于学习演示，不涉及真实生产数据
