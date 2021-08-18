

## Adversarial Machine Learning

Takeru Miyato, Shin-ichi Maeda, Masanori Koyama, Shin Ishii:  
Virtual Adversarial Training: A Regularization Method for Supervised and Semi-Supervised Learning. IEEE Trans. Pattern Anal. Mach. Intell. 41(8): 1979-1993 (2019)  
https://arxiv.org/abs/1704.03976  
> They build a virtual adversarial loss induced by pesudo label to utilize unlabeled data.

Mathias Lécuyer, Vaggelis Atlidakis, Roxana Geambasu, Daniel Hsu, Suman Jana:  
Certified Robustness to Adversarial Examples with Differential Privacy. CoRR abs/1802.03471 (2018)  
https://arxiv.org/abs/1802.03471  
> They build the connection between roubstness and differential privacy. Certified robustness is a concept to design defense proactively against adversarial examples. Differentially private mechanism provide robustness on dataset-level. They add a noise layer to neural network which satisifes differential privacy to maintain the robust output when input changes slightly. This design can be used in various neural network.

Aditi Raghunathan, Jacob Steinhardt, Percy Liang:  
Certified Defenses against Adversarial Examples. ICLR 2018  
https://openreview.net/forum?id=Bys4ob-Rb  
> It provide a provable form of robustness against attack from norm-based adversarial example. Through adding adversarial loss, it trains a robust neural network. Specially, the neural network only contains a hidden-layer. For more complex model, this method doesn't work.  
> This paper point out a direction: we should be proactive against attack by model attacker's behavior and design defense.




## Generalization Error Analysis

Karthik Sridharan, Shai Shalev-Shwartz, Nathan Srebro:  
Fast Rates for Regularized Objectives. NIPS 2008: 1545-1552  
http://papers.nips.cc/paper/3400-fast-rates-for-regularized-objectives  
> Convergence properties of empirical minimization of a stochastic strongly convex objective, where the stochastic component is linear.(SVM/Logistic Regression)
  

Shai Shalev-Shwartz, Nathan Srebro:  
SVM optimization: inverse dependence on training set size. ICML 2008: 928-935  
http://ttic.uchicago.edu/~shai/papers/SSSICML08.pdf
>SVM的训练时间随数据量上升而增加，若果限定最终模型的近似精度范围，那么当一部分数据就足够支持模型达到这个近似精度时，利用其余数据来加速训练  
>文章中对于SVM泛化性能的分析方式在privateERM及其之后的工作中被广泛使用
