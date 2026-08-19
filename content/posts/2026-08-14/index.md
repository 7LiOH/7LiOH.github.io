+++
date = '2026-08-14T23:37:15+08:00'
draft = false
math = true
title = '探究最佳抛射角问题'
tags = ["物理", "高中"]
+++

随着14世纪左右火炮在欧洲的登场，如何精确射击成为迫切需求，这直接催生了弹道学研究

以下为对起止点在同一水平面的探究（**不考虑空气阻力**）

> 可将**斜抛运动**分解为**水平方向的匀速直线运动**与**竖直方向的竖直上抛运动**进行分析

规定水平向右为 $x$ 轴正方向，竖直向上为 $y$ 轴正方向，设该物体向右抛出

设物体初速度为 $v$，与水平面夹角为 $\theta$，易得初速度 $v$ 的水平与竖直分量为
$$ v_x = v\cos\theta $$ 
$$ v_y = v\sin\theta $$

由于平抛运动具有**对称性**，所以当物体的竖直速度与物体初竖直速度矢量和为 $0$ 时，物体落地

由 $v = v_0 + at$ 得，
$$ -v_y = v_y - gt $$
$$ t = \dfrac{2v_y}{g} = \dfrac{2v\sin\theta}{g} $$

将 $t = \dfrac{2v\sin\theta}{g}$ 代入 $v = \dfrac{x}{t}$ 得
$$ v_x = \frac{x}{t} $$
$$ x = v_xt = v\cos\theta \cdot \dfrac{2v\sin\theta}{g} = \dfrac{2v^2\sin\theta\cos\theta}{g} $$

即转换为求关于 $x$ 与 $\theta$ 的函数的最大值

注意到 $\sin 2\theta = 2\sin\theta\cos\theta$

所以原函数可化为
$$ x = \dfrac{v^2\sin 2\theta}{g} $$

对正弦函数 $y = \sin x$，当 $x \in \{\dfrac{\lambda\pi}{2} | \lambda \in \{2k - 1\}, k \in \mathbb{Z}\}$ 时，$y$ 有最大值 $1$

所以当
$$ 2\theta = 90^\circ $$
$$ \theta = 45^\circ $$
时，$x$ 有最大值

$$ x_{\text{max}} = \dfrac{v^2\sin\dfrac{\pi}{2}}{g} = \dfrac{v^2}{g} $$

故
$$
    \begin{cases}
        x_{\text{max}} = \dfrac{v^2}{g} \\
        \theta = 45^\circ
        \tag*{$\square$}
    \end{cases}
$$

---