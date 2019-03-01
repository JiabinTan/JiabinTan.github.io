---
layout: post
title:  "矩阵相关分解专题开篇"
date:   2019-03-01
excerpt: "主要包括LU、Cholesky、QR等分解的一些条件和说明"
tags: [matrix,decomposition]
feature: https://JiabinTan.github.io/assets/img/post/math_3_1_2019.jpg
comments: true
---

### 说明

&emsp;&emsp;本文主要是矩阵分解这块知识的开篇，后面的文章会涉及的内容有：<br/>
- LU、LDL、Cholesky、SVD等分解的简单比较 
- 后面系列博文的安排

### 各个分解的比较
 
| 名称  |  形式 | 条件  |
| :------------: | :------------: | :------------: |
| LU分解  |  \\( A=LU \\)  | A顺序主子式不为零,L为下三角矩阵，U为上三角矩阵  |
| Cholesky 分解  | \\( A=GG^H\\) , \\(G^H\\)表示G的共轭转置 |  A为正定矩阵，G为下三角矩阵 |
| LDL分解  | \\( A=LDL^H\\)   |  A为正定矩阵，L为下三角矩阵，D为对角矩阵 |
|  特征值分解 | \\(Av={\lambda}v \\)  | A为方阵  |
|  SVD | \\( A=UΣV^H\\)  | A是m×n阶矩阵，U是m×m阶酉矩阵；Σ是半正定m×n阶对角矩阵；V是n×n阶酉矩阵|
|  QR | \\( A=QR\\)  | A为非奇异矩阵，Q为正交矩阵，R为上三角矩阵  |
|  schur |   \\( A=QUQ^{-1}\\) | Q是酉矩阵,U是上三角机矩阵  |

<br/>
### 后面安排
专题结构:
- 第一篇博文将会就LU、Cholesky、LDL进行展开
- 第二篇博文将会就奇异值分解、SVD、GSVD进行展开
- 第三篇博文将会就QR进行展开
- 第四篇博文将会就Schur、CS分解进行展开
专题主要列举比较常用的相关分解，如果有必要可以考虑系统的学习矩阵计算[1]
<br/>

### 参考

[1]Gene H. Golub.matrix computations


<br/>
<br/>
<br/>
## <label style="color:orange">重要！！！（Important）</label>

评论版块需要fan墙，如果需要请fan墙后操作。<br/>
游客评论无法接受回复提醒邮件。<br/>
之前也用了别的评论系统，但还是觉得这个比较好，功能比较全。<br/>
