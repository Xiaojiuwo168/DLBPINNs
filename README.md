# [Dynamic Loss Balanced Physics-Informed Neural Networks](https://github.com/Xiaojiuwo168/DLBPINNs/)

近年来，物理信息神经网络 (Physics-Informed Neural Networks, PINNs) 在求解非线性偏微分方程 (Partial Differential Equations, PDEs) 中得到了大量应用. PINNs将物理信息作为一种正则化约束加入神经网络损失函数中，可以减少传统神经网络方法对数据的大量依赖. 然而，这种做法使得PINNs在训练中无法根据数据变化而动态调整损失函数中各个残差权重，导致PINNs在求解非线性PDEs中存在求解误差较大的局限. 为了解决该问题，本文提出了一种动态损失平衡的物理信息神经网络 (Dynamic Loss Balanced Physics-Informed Neural Networks, DLBPINNs) . 首先，DLBPINNs通过分别为PINNs损失函数的各个损失项设计了一种动态权重系数以解决不同损失项梯度下降速度的不平衡. 其次，DLBPINNs在动态权重系数的基础上为PNNNs损失函数的各个损失项之间建立了一种的损失平衡求和以降低误差. 本文选择了科学机器学习领域中四个经典的非线性PDEs对DLBPINNs进行数值验证和分析. 实验结果表明，DLBPINNs比PINNs在Schrodinger和Allen-Cahn方程上误差分别降低了46%、64%. DLBPINNs在求解Navier-Stokes方程时将系数 λ_1 的误差降低了1至2个数量级和系数 λ_2 的误差降低了约50%. DLBPINNs在KdV方程中能够在多项系数中将误差降低1个数量级. 最后，本文在多种形式的Burgers方程上进行大量消融实验以验证了DLBPINNs能够带来性能的提升、具有处理数据量小的能力以及能够拟合不同时间状态下的方程. DLBPINNs可以取代PINNs被应用于各种非线性PDEs的高精度求解，源代码见于https://github.com/Xiaojiuwo168/DLBPINNs/.

All codes will be release soon.
For more information, please refer to the following: (https://github.com/Xiaojiuwo168/DLBPINNs/).
