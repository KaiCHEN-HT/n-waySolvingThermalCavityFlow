# 二维方腔自然对流的N种解法

## 1. 可计算建模
### 1.1 问题描述与数学物理模型

<div align="center">
  <img src="images/computational domain.png" alt="computational domain" width="400">
</div>

<div align="center">
    计算域与边界条件
</div>

<br>
如图所示，二维方腔的上下边界均为均为绝热边界，左边界为高温边界，右边界为低温边界。
当高温边界与低温边界温度差别较小（<15℃）时，可以采取Boussinesq假设：假设密度变化对流场没有影响，在计算时只需考虑产生浮力的情况。由此可以得到简化后的N-S方程：

- 连续方程:

$$ \frac{\partial u}{\partial x} +  \frac{\partial v}{\partial y}=0$$

- 动量方程:

`x`方向: 
$$ u\frac{\partial u}{\partial x} +  v\frac{\partial u}{\partial y}=-\frac{1}{\rho}\frac{\partial p}{\partial x}+ v(\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2})$$

`y`方向: 
$$ u\frac{\partial v}{\partial x} +  v\frac{\partial v}{\partial y}=-\frac{1}{\rho}\frac{\partial p}{\partial y}+ v(\frac{\partial^2 v}{\partial x^2} + \frac{\partial^2 v}{\partial y^2}) + g\beta(T-T_0)$$

- 能量方程：
$$ u\frac{\partial T}{\partial x} +  v\frac{\partial T}{\partial y}=a(\frac{\partial^2 T}{\partial x^2} + \frac{\partial^2 T}{\partial y^2})$$

### 1.2 方程无量纲化

为了更加直观的理解**相似原理**，展示流动的相似性，下面通过**量纲分析**对以上方程进行无量纲化，进而求解无量纲方程。一组无量数下无量纲方程得到的结果代表了整个相似组的解。


## 2. 算法
### 2.1 FVM商软求解



### 2.2 paddlesci求解（Python）


### 2.3 paddle求解（Python）


### 2.4 FEM求解（C++）



### 2.5 FVM求解（C++）



### 2.6 FEM求解（C++）



### 2.7 谱方法求解（C++）


### 2.8 LBM求解（C++）