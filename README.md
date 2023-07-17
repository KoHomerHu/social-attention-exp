# Social Attention Experiment

An implementation of the paper [Social Attention for Autonomous Decision-Making in Dense Traffic](https://arxiv.org/pdf/1911.12250.pdf) with custom modification (experiments with SAC and GAIL).

We use the low-level continuous action so that it might be harder for the agent to learn from scratch (RGB rendering shows that the agent goes crazy and few other vehicles appeared in the view, probably the attention module is not working at all), perhaps next step is to try out SAC over discrete action space (with the DiscreteMetaAction type).

Simply install the requirements and run the following command, enjoy (though most likely not)~~ 

```
python train.py
```

## To-do List

1, Try out [DiscreteMetaAction](http://highway-env.farama.org/actions/#discrete-meta-actions)

2, Treat a trained agent as expert (or maybe collect manual control data) and try out [GAIL](https://arxiv.org/pdf/1606.03476.pdf) 

3, Incorporate DRQN to enhance performance (maybe refer to this [Playing FPS Games with Deep Reinforcement Learning](https://arxiv.org/pdf/1609.05521.pdf))

## Results

### 300 episodes Continuous Action (rewards scale x10)

![image](./result01.png)


