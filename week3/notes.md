# Feedback is all you need
## feedback基本思想
期刊《cybernetics》
## 人类反馈强化学习 （RLHF）
- 第三种基本的机器学习方法（ *RL* ）（ **基本构成** ）
  - 策略
  - 值函数
  - 回报函数   
- **动态规划** 和 **MPC**
  MPC可以看作一个局部最优的动态规划， ""小范围""
- Q-learning
  通过当前值来更新当前状态下的最优控制
  $$ Q(s_t,a_t)\gets Q(s_t,a_t)+\alpha \overset{temperary\,\,difference}{\overbrace{\left[ \underset{new\,\,value\,\,\left( temperary\,\,difference\,\,target \right)}{\underbrace{r_{t+1}+\gamma \max_a Q(s_{t+1},a)}}-Q(s_t,a_t) \right] }}$$
