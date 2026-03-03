# Final projects

The final reports consists of the following three project, each with 20 points.

Popular open data repositories include

- http://archive.ics.uci.edu/ml/
- https://www.kaggle.com/datasets
- https://registry.opendata.aws/

## 1、project 1: CNN (20 point)

#### 1)   Problem Statement and Task Definition (5%): 

- Brief overview of your problem. 
- What does your system do (what is its input and output)? 
- What real-world problem does this system try to solve? 
- Why might this problem be important? 

#### 2)   Get image data and define task (20%)

a)    Select an image data set that interest you in Kaggle(or TFDS, sklearn) and get the data set. (You cannot use data set which have already analyzed in the class and in the textbook. Your data set cannot be less than 1000 samples)

b)    Write a code to select picture randomly, draw the selected picture and show its label. You need to show one sample for each label.

c)    Define your task: Is it regression, binary classification, muticlassification task? Evaluation Metric

d)    Write image preprocess code including data augmentation layer and shows it work

e)    Split the data set into train set and test if they do not existed. Show the shape of train and test set

#### 3)   Build a CNN architecture and improve it (30%)

a)    Build a traditional CNN architecture as baseline, finish a full train steps including:. build model, compile, fit, evaluate, visualize your model, plot training curve.

b)    Analyze training curve and prose improvement method.Build a improving model according your analyses.

c)    Repeat step b) until your model is slightly overfitted.

#### 4)   Transfer learning (20%)

a)    use feature extraction transfer learning method to train a model base on EfficientNetB0 and restnet respectively with full train step

b)    use fine tune transfer learning method to train a model base on EfficientNetB0 ,  , finish a full train step

#### 5)   Best model, its performance and usage (20%)

a)    compare above model and find your best model.

b)    Compute precision, racall, F1 Score of each category

c)    confusion matrix and discussed it

d)    Select 5 randomly picture from test set, make prediction, draw the pictures and show their predictions and labels. Does the prediction right?

#### 6)   Conclusion and review (5%)



## 2、project 2: Time series (20 point)

#### 1)   Problem Statement and Task Definition (5%): 

- Brief overview of your problem. 
- What does your system do (what is its input and output)? 
- What real-world problem does this system try to solve? 
- Why might this problem be important? 

#### 2)   Get and explore time series data (20%)

a)    Select a time series dataset that interests you in the Kaggle (or TFDS, sklearn) and get the data.

b)    Show a few data sample, visualize the time series, Split into tran/test set.

c)    What is your model input and output, define Evaluation Metric, Specifically , Prepare a function to calculate following metric given true label and prediction value: 'mae', 'mse', 'rmse', 'mape', 'mase'

d)    Naïve model (baseline, use value of current step to predict value of next step), evaluate it using your metric, visualize your prediction

#### 3)   Window the time series, show your windows works correctly, Split the data set into train set and test.(10%)

#### 4)   Build following model. (60%, each model 10%)

a)    Dense network, finish a full train step(Train, evaluate, visualize training process, improve model at least once)

b)    Conv1D, finish a full train step

c)    RNN/LSTM, finish a full train step

d)    [N-BEATs Algorithm](https://arxiv.org/pdf/1905.10437.pdf), finish a full train step

e)    ARIMA (Autoregression Integrated Moving Average), P719, [Hands-on Machine Learning with Scikit-Learn, Keras and TensorFlow (3rd edition)](https://homl.info/er3): Use ad test to check whether the time series is stationary. If it is not, difference the time series until it is stationary. Train Arima model, draw autocorrelation, adjust (p,q,d) accordingly.

f)     Esemble learning. Using different combination of loss function("mae", "mse", "mape") and layer number to create multiple neural networks(dense or RNN/LSTM)，and esemble them into one model, evaluate its performance.

#### 5)   Models comparation (5%)

a)    Compare above model, visualize the comparation, find the best model, discuss what you find

b)    Visualize the best model’s prediction against true value, discuss what you find

 

## 3、project 3: Reinforce learning (20 point)

#### 1)   Problem Statement and Task Definition (5%):

- Brief overview of your problem. 
- What does your system do (what is its input and output)? 
- What real-world problem does this system try to solve? 
- Why might this problem be important? 

#### 2)   Familiar with environment of reinforcing learning (10%)

a)    Select a enforcing learning env from gym( You can not use env that has been discussed in the class room)

b)    Describe state, reward, action space, design goal

#### 3)   Design random policy as baseline (10%)

a)    Implement a random policy, visualize episode_returns

#### 4)   Design Double DQN (35%)

a)    Implement Double DQN, visualize episode_returns, Can it beat random policy?

b)    Improve your model at least once: Use q_network to select best action and use target_network to calculate maximal Q value.

c)    Dueling Double DQN( principle see text book)

d)    Change size of play buffer or layer number of CNN, Can it impact performance?

#### 5)   Design A2C (35%)

a)    Implement A2C, visualize episode_returns, Can it beat random policy?

b)    Improve your model at least once by varying following parameter: number of environments to run in parallel, Number of steps to collect per environment before update, discount factor, value function coefficient for loss. Change one parameter at one time and discuss its impaction.

#### 6)   Summary: Compare above model and discuss (5%)

 

 

## **Project report requirements**

You should submit a final Report for each above project and each final report include 5-10 pages at least. 

Each sub-section of report should correspond to each requirement of final project. 

In Each sub-section, You need to say a few sentence what you are going to do, then shows your code, and your code outcome, Then analyze the code come outcome. 

For example, discuss it. Is it expect outcome? If it is loss curve or accuracy curve, What does it mean? Is your model overfitted or underfitted? What is your next step? 

**If discussion is missing, the item’s score will be halved**.

**You can not use any data set have been use in the classroom and homework.**

## Format

You should use **Word** to write an analysis report for each project, then convert the reports to PDF format. 

The **document** names should follow the format: **Student ID + English Name + Project Name.** 

You need to submit a compressed package (e.g., .zip or .rar) containing the following files:

- three analysis reports,
- three source code files
- the data files used by the source code. 

The **compressed package** should be named as: **Student ID + English Name.**

 If the dataset is large to upload, you have to state clearly source of code and submitted a subset of your data set.
