# 人工智能基础及应用 - 作业汇总

## 作业1: auto-diff
- **作业形式**: 个人作业
- **占成绩比例**: 5.00%
- **计分规则**: 最高得分
- **评分方式**: 教师评阅 (100.0%)

### 作业要求
1. Basic of neural networks and tensorflow (5 point)
   - Assuming y=(w1-1)^2 +(w2-2)^2+4, where w1,w2 is variable and their Initial value is 3 and 5 respectively. We want to minimize this function
   - Calculate the minimum value of this function (25%)
   - Use gradient descent to calculate: Draw computing graph and perform two iterations by hand (25%)
   - Write an iterate program using autodiff of tensorflow (25%)
   - For y=-(w1-1)^2 -(w2-2)^2+4, write program to maximize this function (25%)

---

## 作业2: Regression
- **作业形式**: 个人作业
- **占成绩比例**: 5.00%
- **计分规则**: 最高得分
- **评分方式**: 教师评阅 (100.0%)

### 作业要求
1. Get ComputerHardware Data Set from UCI, describe dataset, design goal, and performance metric (10%)
   - [Air Quality - UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/360/air+quality)
2. Preprocess data (10%)
   - Split into train (80%), valid (10%), test (10%)
   - Build pipeline: replace missing values, one-hot encode categorical features, scale numerical features
3. Build base model: build, compile, fit, visualize, evaluate, predict first 5 samples, plot loss curve (10%)
4. Improve model based on overfitting/underfitting analysis (30%)
5. Repeat improvements twice until slightly overfitted (20%)
6. Build random search for optimal hyperparameters and compare results (20%)

---

## 作业3: classification
- **作业形式**: 个人作业
- **占成绩比例**: 6.00%
- **计分规则**: 最高得分
- **评分方式**: 教师评阅 (100.0%)

### 作业要求
1. Get Adult Data Set from UCI, describe dataset, design goal, performance metric (10%)
   - [Adult - UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/2/adult)
2. Prepare dataset: split (80/20), write preprocessing pipeline (10%)
3. Build baseline model (10%)
4. Find the best learning rate (20%)
5. Improve model based on overfitting/underfitting analysis (20%)
6. Finetune with random search method (10%)
7. Compare models (10%)
8. Compute confusion matrix, precision, recall and F1 score (10%)

---

## 作业4: CNN
- **作业形式**: 个人作业
- **占成绩比例**: 5.00%
- **计分规则**: 最高得分
- **评分方式**: 教师评阅 (100.0%)

### 作业要求
1. Get CIFAR10 dataset and explore data "from tensorflow.keras.datasets import cifar10" (10%)
- Draw pictures, show shape, count samples in each class
2. Use ImageDataGenerator to scale, augment and load data (10%)
3. Train baseline model (10%)
4. Improve model by changing hyperparameters (20%)
- Number of layers
- Number of filters (10, 32, 64, 128)
- Epochs
- Learning rate
- Data augmentation parameters
5. Repeat until slightly overfitted, change at least 3 options (20%)
6. Compare models (10%)
7. Compute confusion matrix, precision, recall and F1 score (10%)
8. Make predictions on test set and visualize results (10%)

---

## 作业5: transfer learning
- **作业形式**: 个人作业
- **占成绩比例**: 0.00%
- **计分规则**: 最高得分
- **评分方式**: 教师评阅 (100.0%)

### 作业要求
1. Get 20% of data from CNN assignment and count distribution (10%)
2. Feature extraction with resnet_v2_50 (20%)
3. Feature extraction with EfficientNetB0 (20%)
4. Compare, select better model (model 3), train with full dataset (10%)
5. Fine-tune models with 20% data, create model 4 (20%)
6. Compare all models and find the best (10%)
7. Compute confusion matrix, precision, recall of best model (10%)

---

## 作业6: time series
- **作业形式**: 个人作业
- **占成绩比例**: 0.00%
- **计分规则**: 最高得分
- **评分方式**: 教师评阅 (100.0%)

### 作业要求
1. Get dataset from Kaggle: [TimeSeries starter dataset](https://www.kaggle.com/datasets/podsyp/time-series-starter-dataset?resource=download) (10%)
2. Visualize the time series (10%)
3. Window and split into train/test sets (10%)
4. Predict using following methods and evaluate on test set (60%)
- Naïve model (baseline)
- Dense network
- RNN
- LSTM
- Conv1D
- [N-BEATs Algorithm](https://arxiv.org/pdf/1905.10437.pdf)
- Ensemble (multiple models with different loss functions)
5. Compare methods, find best, visualize predictions vs true values (10%)

---

## 作业7: reinforcement learning
- **作业形式**: 个人作业
- **占成绩比例**: 0.00%
- **计分规则**: 最高得分
- **评分方式**: 教师评阅 (100.0%)

### 作业要求
1. Markov decision process (50%)
- 3×3 maze environment: agent starts at S, seeks path to G
- Rewards: -1 (blue grid), -10 (red X), +10 (goal G)
- Use Value Iteration to find Optimal Policy for each state
2. Programming practice (50%)
- Describe LunarLander-v2 environment: define state, action, reward
- Interact with environment manually
- Implement random policy and evaluate performance
- Implement deep reinforcement learning (e.g., DDQN) and compare with random policy

