# paper-list

privateERM

Kifer, D., Smith, A., & Thakurta, A. (2012). Private Convex Empirical Risk Minimization and High-dimensional Regression. Conference on Learning Theory.  
http://101.96.10.63/www.cse.psu.edu/~ads22/pubs/KST12/KST12-2012-06-07-Colt-camera.pdf  
>在目标扰动上引入高斯噪声，有更低的期望误差  
>证明了目标扰动的privateERM在带有非处处可微的正则项时依然满足dp  
>分析了对于稀疏回归场景的应用  

Chaudhuri, K., Monteleoni, C., & Sarwate, A. D. (2011). Differentially Private Empirical Risk Minimization. Journal of Machine Learning Research, 12, 1069–1109.  
https://dl.acm.org/citation.cfm?id=2021036  
>纠正了前一篇文章中的错误，正式提出了一类基于经验误差最小化方法的dp框架privateERM  
>对输出扰动和目标扰动两种方法的泛化误差进行了分析  
>应用于logistic回归和svm的性能分析  

Chaudhuri, K., & Monteleoni, C. (2008). Privacy-preserving logistic regression. In Advances in Neural Information Processing Systems 21 (pp. 289–296).  
http://www.cse.psu.edu/~ads22/privacy598/papers/cm08.pdf  
>分析了带正则逻辑回归输出的函数敏感度，提出了在输出上增加Laplace噪声达成dp的lr  
>在目标函数中增加随机向量b，由b的随机性导出优化求得解的随机性，称为目标扰动的lr  

---

dp optimization

Zhang, J., Xiao, X., Yang, Y., Zhang, Z., & Winslett, M. (2013). PrivGene: differentially private model fitting using genetic algorithms. In Proceedings of the 2013 ACM SIGMOD International Conference on Management of Data (pp. 665–676).  
http://davidyinyang.weebly.com/uploads/9/8/6/2/9862052/privgene_final.pdf
>将遗传算法的每一步作隐私化处理构建了满足差分隐私的参数求解方法  
>提出了EEM(增强的指数机制)用于隐私地选择，当候选参数随着迭代求解过程而趋于相同时，EEM较EM能提供更小的噪声  

---

dp histogram publishing

Dong Su, Jianneng Cao, Ninghui Li, Min Lyu: PrivPfC: differentially private data publication for classification. VLDB J. 27(2): 201-223 (2018).  
https://link.springer.com/article/10.1007%2Fs00778-017-0492-3

>PrivPfC，在DiffGen的基础上针对更多特征的数据集和二分类任务进行了优化，通过生成Generalization候选映射，然后直接选择的方式，略去了DiffGen中的迭代过程  
code:https://github.com/DongSuIBM/PrivPfC

Mohammed, N., Chen, R., Fung, B. C. M., & Yu, P. S. (2011). Differentially private data release for data mining. In Proceedings of the 17th ACM SIGKDD international conference on Knowledge discovery and data mining (pp. 493–501).  
https://dl.acm.org/citation.cfm?id=2020408.2020487  
>DiffGen,za在满足dp的框架下实现隐私保护中常用的Generalization方法发布匿名化数据集，赋予其可证的保护程度  
code:https://github.com/McGill-DMaS/DiffGen  

---


