# Machine learning

> By Andrew NG

## General

### Supervised learning

#### Defination

- Learns from being given "right answers"

#### Regression

- Predict a number

- Infinitely many possible outputs

#### Classification

- Predict categories

- Small number of possible outputs

### Unsupervised learning

#### Defination

Find something interesting in unlabled data

#### Clustering

Group similar data points together.

![](https://raw.githubusercontent.com/0x3f3f3f3f3f3f3f3f3f3f3/UPIC/master/uPic/CleanShot 2024-08-05 at 13.54.39@2x.png?token=AZ7ARDGV246EQY4RXT654C3GWGXZI)

#### Anomaly detection

- Find unusual data points

#### Dimensionality reduction

- Compress data using fewer numbers.



## Linear regression

### Terminology

- Training set : data used to train the model
- $x$ :
   - "input" variable
   - Feature

- $y$ :
   - "output" variable
   - "target" variable

- $m$ : number of training examples
- ($x$ , $ y$) : single training example
- ($x^{(i)}$ , $y^{(i)}$) : $i^{th}$​ training example
- $\hat y$ : the estimate or the prediction for $y$​
- $w$​ : 
   - weight
   - parameters

- $b$​  : 
   - bias
   - parameters




### Model

$$
f_{w,b}(x)=wx+b
$$

### Cost function

#### Squared erro cost function

$$
J(w,b)=\frac{1}{2m}\sum_{i=1}^m(\hat y ^{(i)}-y^{(i)})^2\\
J(w,b)=\frac{1}{2m}\sum_{i=1}^m(f_{w,b}(x^{(i)})-y^{(i)})^2\\
$$

![](https://raw.githubusercontent.com/0x3f3f3f3f3f3f3f3f3f3f3/UPIC/master/uPic/CleanShot 2024-08-06 at 11.00.17@2x.png?token=AZ7ARDHKOJGY5CBOHC47O6LGWGJA2)

### Gradient descent

#### Rule

$$
w=w-\alpha\frac{\partial }{\partial w}J(w,b)\\
b=b-\alpha\frac{\partial }{\partial b}J(w,b)
$$

- $\alpha$​ : Learning rate

- $\frac{\partial }{\partial w}J(w,b)$​ : Derivative

#### Learning rate

- Too small
  - Slow
- Too big
  - Overshoot
  - Fail to converge, diverge

### Different version

#### Batch gradient descent

Each step of gradient descent uses all the training examples

#### Subsets

Use only subsets each step of gradient descent


