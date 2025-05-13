本篇介绍当前流行的分布式训练框架与通信协议。

## 什么是分布式训练？
通过多台设备共同完成模型训练任务。

## 数据并行 vs 模型并行
| 类型       | 说明 |
|------------|--------|
| 数据并行   | 多卡训练同一模型，每卡处理不同 batch |
| 模型并行   | 不同层分布在不同设备上 |

## AllReduce 算法
用于同步梯度更新，在 PyTorch 和 TensorFlow 中广泛应用。

```python
dist.all_reduce(tensor, op=dist.ReduceOp.SUM)