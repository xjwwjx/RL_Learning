# 马尔科夫决策过程（MDP）

对于MRP(Markov Reward Process)的几个公式：
![alt text](image-6.png)

Value Function还可以转化为下面这个式子：
![alt text](image-7.png)

现在的目标求解Value Function，有两种方法可以解决这个问题：

- 1. 矩阵乘法直接计算，算法复杂度$O(n_3)$：
![alt text](image-8.png)

- 2. 动态规划求解，算法复杂度$O(n_2)$:
![alt text](image-9.png)
**注意：k为迭代次数，而不是时间戳**

## MDP组成结构

![alt text](image-10.png)

MDP + Policy
![alt text](image-11.png)


![alt text](image-12.png)

举一个例子来更加理解贝尔曼方程的形式：
![alt text](image-13.png)
答案是2.5

## State-Action Function 
![alt text](image-15.png)
![alt text](image-14.png)

## Markov Policy Iteration
![alt text](image-17.png)

![alt text](image-16.png)
第二个公式的意思是：我在这一时间步使用的策略应该要比上一时间步策略使用的最优策略要更优。

![alt text](image-18.png)

## Value Iteration

![alt text](image-19.png)