# 2023-EXP-Frozen_Lake

## 代码运行指南

### 脱机模拟

代码存放在offline文件夹中

#### q_learning & Sarsa

环境配置：

新建conda环境：`python==3.7`，然后在conda环境中执行（pip也需要使用当前conda环境的pip）

```
pip install tensorflow==1.15
pip install gym==0.23.1
pip install pygame
pip install tqdm
pip install matplotlib
conda install -c conda-forge gcc  # 在无英伟达显卡的设备上运行的时候需要执行这一指令
```

<font color=red>在`q_learning+Sarsa`文件夹下</font>启动Terminal，`conda activate xxx`以后

执行以下代码开始训练或进行演示。

```
python -m q_learning.train
python -m q_learning.load
```

```
python -m Sarsa.train
python -m Sarsa.load
```



#### DQN

新建conda环境：`python==3.8`，然后在conda环境中执行（pip也需要使用当前conda环境的pip）。

```
pip install tensorflow==2.10
pip install gym==0.23.1
pip install pygame
pip install tqdm
pip install matplotlib
```

进入DQN文件夹中，激活环境后执行`python DQN.py`即可开始训练，训练结束以后自动进行仿真实验。
