# The basic idea of policy gradient
之前介绍的deep Q-Learning是基于值函数的，而策略梯度方法则是直接根据策略来得到最优策略。<br>
与deep Q-Learning方法类似，策略梯度方法也可以使用梯度上升/下降方法优化。<br>
![alt text](../images/policy_gradient.png)
现在的问题是如何定义$J(\theta_t)$。

# Metric of define optimal policy

## Average Value
![alt text](../images/Average_Value.png)
其中，$d(s)$的定义为stationary distribution，在前面几节已经介绍过了。<br>

可以使用$\bar{v}(s)$来当作$J(\theta_t)$，神经网络的目标是最大化$J(\theta_t)$。
![alt text](../images/Average_Value_2.png)

## Average Reward
![alt text](../images/Average_Reward.png)

## 两种metric的对比
![alt text](../images/Average_Comparison.png)

## The implementation of policy gradient
![alt text](../images/Policy_Gradient_Implementation.png)
此外，还有一些对于$J(\theta_t)$的梯度求解方法以及相关分析，具体可以看ppt的解释。