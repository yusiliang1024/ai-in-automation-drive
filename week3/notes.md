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
     $$Q(s_t,a_t)\gets Q(s_t,a_t)+\alpha \overset{temperary\quad difference}{\overbrace{\left[ \underset{new\quad \quad value\quad \quad \left( temperol\quad difference\quad target \right)}{\underbrace{r_{t+1}+\gamma \max_a Q(s_{t+1},a)}}-Q(s_t,a_t) \right] }}$$
- 环境
  常被假设为 **马尔可夫决策过程** ，只关注于未来的状态影响
- 离线训练过程：
  - **MDP假设** 下，去逼近最优贝尔曼方程解的闭环反馈控制 $u=C(x|MDP)$
  - **Real World环境下** ,不满足MDP/“没见过”场景 $u=C(x|MDP)$ "开环"
- 常见的闭环控制：
  - 辨识
  - 电池
  - 通信
  - 定位
  - 游戏
