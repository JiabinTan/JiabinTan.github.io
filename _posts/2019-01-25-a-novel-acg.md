---
layout: post
title:  "论文摘要《A NOVEL AGC SCHEME FOR QAM DEMODULATOR APPLICATIONS》"
date:   2019-01-24
excerpt: "基于自适应均衡算法解决ISI与AGC"
tags: [AGC,equalizer,QAM,论文摘要]
feature: https://JiabinTan.github.io/assets/img/post/elec.jpg
comments: true
---

### 论文信息
<img src='https://JiabinTan.github.io/assets/img/post/201901251.png' alt='论文信息' align='center' title='论文信息'/>
### 主要内容
&emsp;&emsp;这边只涉及算法有关的内容，如果需要可获取原文详细阅读。<br/>
&emsp;&emsp;该论文主要思想是，使用均衡器输出来同时解决AGC与ISI问题。一般我们使用均衡器来处理ISI问题，文中使用的是自适应算法，详细过程如下：<br>
<img src='https://JiabinTan.github.io/assets/img/post/201901252.png' alt='公式1' align='center' title='公式1'/>
<p align='center' style='font-style:italic;font-size:12px'>公式1</p>
&emsp;&emsp;其中k表示时刻（下同），$C_k$为均衡器系数向量，$X_k$为输入数据向量。另均衡器错误为$e_{k-1}$，$\hat y_k$是决策值，$y_k$是均衡器输出值。则可以将三者表示为
<img src='https://JiabinTan.github.io/assets/img/post/201901253.png' alt='公式2' align='center' title='公式2'/>
<p align='center' style='font-style:italic;font-size:12px'>公式2</p>
&emsp;&emsp;带入公式1
<img src='https://JiabinTan.github.io/assets/img/post/201901254.png' alt='公式3' align='center' title='公式3'/>
<p align='center' style='font-style:italic;font-size:12px'>公式3</p>
&emsp;&emsp;之后，令AGC错误为（乘上$y_{k-1}$是为了产生凸优化解）
<img src='https://JiabinTan.github.io/assets/img/post/201901255.png' alt='公式4' align='center' title='公式4'/>
<p align='center' style='font-style:italic;font-size:12px'>公式4</p>
&emsp;&emsp;注意上面的公式实际上在分开考虑增益错误与均衡器错误。<br/>
&emsp;&emsp;最后就可以实现整个电路图了
<img src='https://JiabinTan.github.io/assets/img/post/201901257.png' alt='简易图' align='center' title='简易图'/>
<p align='center' style='font-style:italic;font-size:12px'>简易图</p>
<img src='https://JiabinTan.github.io/assets/img/post/201901256.png' alt='电路图' align='center' title='电路图'/>
<p align='center' style='font-style:italic;font-size:12px'>电路图</p>
&emsp;&emsp;这边的电路图将Vg整数部分与小数部分分开考虑，整数部分乘法体现为shift（二进制）。<br/>
&emsp;&emsp;大概就是这些。<br/>
<br/>
### 未涉及原文内容有
- 算法的稳定性分析
- 实验结果
- 以及一些详细的解释内容
有需要的同学请参看原文

### 参考
Deng Q , Wu J H , Shi L X , et al. A novel AGC scheme for QAM demodulator applications[M]. 2007.


<br/>
<br/>
<br/>
## <label style="color:orange">重要！！！（Important）</label>

评论版块需要fan墙，如果需要请fan墙后操作。<br/>
游客评论无法接受回复提醒邮件。<br/>
之前也用了别的评论系统，但还是觉得这个比较好，功能比较全。<br/>
