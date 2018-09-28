# DQN开发
我们在forex市场寻找圣杯
## 理论基础

bid为阴土，ask为阳土，买阴不买阳，卖阳不卖阴

### DQN 

## 开发笔记

### 第一天

我们以30S为周期，一周的数据是14400条，需要设置State和ForexEnv(继承gym.Env)

metadata = {'render.modes':['human']}

#### 预备

    强化学习基本知识：智能体agent与环境environment、状态states、动作actions、回报rewards等等，网上都有相关教程。
    
    gym安装：openai/gym 注意，直接调用pip install gym只会得到最小安装。如果需要使用完整安装模式，调用pip install gym[all],或者只安装gym[atari]。
    pytorch会用到。
    
    主流开源强化学习框架推荐如下。以下只有前三个原生支持gym的环境，其余的框架只能自行按照各自的格式编写环境，不能做到通用。
    并且前三者提供的强化学习算法较为全面，PyBrain提供了较基础的如Q-learning、Sarsa、Natural AC算法。
    Tensorlayer基于tensorflow开发，提供了更为基本的api。
 
     OpenAI提供的Baselines：openai/baselines 3.2k starsTensorforce：reinforceio/tensorforce 1.2k 
     starsIntel提供的Coach：NervanaSystems/coach 0.6k stars，pip安装可以使用pip install rl-coach，而不是pip install coachPyBrain：pybrain/pybrain 2.5k starsTensorlayer：tensorlayer/tensorlayer 3.1k stars
