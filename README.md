# paper-list

## dp learning  

Bassily, Raef, et al. “Private Empirical Risk Minimization: Efficient Algorithms and Tight Error Bounds.” 2014 IEEE 55th Annual Symposium on Foundations of Computer Science, 2014.  
https://arxiv.org/pdf/1405.7085.pdf  
>利用sgd采样随机性的dp实现  
>给出了dpERM的经验误差下界  
>基于Localization+EM的可实现的参数求解框架(相较之前的(Kifer,2012)框架，给出了一个可实现的解法)  
  
Kifer, Daniel, et al. “Private Convex Empirical Risk Minimization and High-Dimensional Regression.” Conference on Learning Theory, 2012.  
http://101.96.10.63/www.cse.psu.edu/~ads22/pubs/KST12/KST12-2012-06-07-Colt-camera.pdf  
>在目标扰动上引入高斯噪声，有更低的期望误差  
>证明了目标扰动的privateERM在带有非处处可微的正则项时依然满足dp  
>分析了对于稀疏回归场景的应用（在一个较优的候选区域求解）  

Chaudhuri, Kamalika, et al. “Differentially Private Empirical Risk Minimization.” Journal of Machine Learning Research, vol. 12, 2011.  
https://dl.acm.org/citation.cfm?id=2021036  
>纠正了前一篇文章(Chaudhuri, 2008)中的错误，正式提出了一类基于经验误差最小化方法的dp框架privateERM  
>对输出扰动和目标扰动两种方法的泛化误差进行了分析  
>应用于logistic回归和svm的性能分析  

Chaudhuri, Kamalika, and C. Monteleoni. "Privacy-preserving logistic regression." International Conference on Neural Information Processing Systems 2008.  
http://www.cse.psu.edu/~ads22/privacy598/papers/cm08.pdf  
>分析了带正则逻辑回归输出的函数敏感度，提出了在输出上增加Laplace噪声达成dp的lr  
>在目标函数中增加随机向量b，由b的随机性导出优化求得解的随机性，称为目标扰动的lr  

---

## dp optimization

Song, Shuang, et al. “Stochastic Gradient Descent with Differentially Private Updates.” 2013 IEEE Global Conference on Signal and Information Processing, 2013.  
https://ieeexplore.ieee.org/document/6736861  
>sgd的dp版本，基于一次梯度下降的函数敏感度对梯度加入噪声
>mini-batch版本获得梯度提升
>为了避免因迭代引起的privacy衰减，每个batch是不相交的，对整个数据集只能遍历一遍

Zhang, Jun, et al. “PrivGene: Differentially Private Model Fitting Using Genetic Algorithms.” Proceedings of the 2013 ACM SIGMOD International Conference on Management of Data, 2013.  
http://davidyinyang.weebly.com/uploads/9/8/6/2/9862052/privgene_final.pdf
>将遗传算法的每一步作隐私化处理构建了满足差分隐私的参数求解方法  
>提出了EEM(增强的指数机制)用于隐私地选择，当候选参数随着迭代求解过程而趋于相同时，EEM较EM能提供更小的噪声  

---

## dp histogram publishing

Dong Su, Jianneng Cao, Ninghui Li, Min Lyu: PrivPfC: differentially private data publication for classification. VLDB J. 27(2): 201-223 (2018).  
https://link.springer.com/article/10.1007%2Fs00778-017-0492-3  
>PrivPfC，在DiffGen的基础上针对更多特征的数据集和二分类任务进行了优化，通过生成Generalization候选映射，然后直接选择的方式，略去了DiffGen中的迭代过程  
code:https://github.com/DongSuIBM/PrivPfC

Mohammed, Noman, et al. “Differentially Private Data Release for Data Mining.” Proceedings of the 17th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, 2011.  
https://dl.acm.org/citation.cfm?id=2020408.2020487  
>DiffGen,za在满足dp的框架下实现隐私保护中常用的Generalization方法发布匿名化数据集，赋予其可证的保护程度  
code:https://github.com/McGill-DMaS/DiffGen  

---

## Generalization Error Analysis

Shalev-Shwartz, Shai, and Nathan Srebro. “SVM Optimization: Inverse Dependence on Training Set Size.” Proceedings of the 25th International Conference on Machine Learning, 2008.  
http://ttic.uchicago.edu/~shai/papers/SSSICML08.pdf
>SVM的训练时间随数据量上升而增加，若果限定最终模型的近似精度范围，那么当一部分数据就足够支持模型达到这个近似精度时，利用其余数据来加速训练  
>文章中对于SVM泛化性能的分析方式在privateERM及其之后的工作中被广泛使用

---

## OverView and Tutorials

Chaudhuri, K.     nips2017 tutorial  
Differentially Private Machine Learning: Theory, Algorithms, and Applications  
https://www.ece.rutgers.edu/~asarwate/nips2017/  


Li, Ninghui, et al. “Differential Privacy:From Theory to Practice.” Synthesis Lectures on Information Security, Privacy, and Trust, vol. 8, no. 4, 2016  
https://ieeexplore.ieee.org/document/7731575?bkn=7731575  


