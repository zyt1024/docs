## [ torch 参数更多 ]torch.special.psi
### [torch.special.psi](https://pytorch.org/docs/stable/special.html#torch.special.psi)
```python
torch.special.psi(input,
              *,
              out=None)
```

### [paddle.digamma](https://www.paddlepaddle.org.cn/documentation/docs/zh/develop/api/paddle/special.digamma_cn.html)
```python
paddle.digamma(x,
               name=None)
```

Pytorch 相比 Paddle 支持更多其他参数，具体如下：
### 参数映射
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
|  input  |  x  | 表示输入的 Tensor ，仅参数名不一致。  |
|  out  | -  | 表示输出的 Tensor ， Paddle 无此参数，需要转写。    |

### 转写示例
#### out：指定输出
```python
# Pytorch 写法
torch.special.psi(input, out=y)

# Paddle 写法
paddle.assign(paddle.digamma(input), y)
```
