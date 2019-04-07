# paper-list

## Semi-Supervised Learning



Anh T. Pham, Jing Xi:  
Differentially Private Semi-Supervised Learning With Known Class Priors. BigData 2018: 801-810  
https://ieeexplore.ieee.org/document/8622071
> It presents a framework for semi-supervised learning, assuming known class priors, and provides the theoretical guarantee on the optimal risk. Under this setting, they give the differentially private learning on the framework. However, they make mistakes on addition of noise, which have been corrected in [[Kamalika Chaudhuri 2011](https://dl.acm.org/citation.cfm?id=2021036)].

Nicolas Papernot, Martín Abadi, Úlfar Erlingsson, Ian J. Goodfellow, Kunal Talwar:  
Semi-supervised Knowledge Transfer for Deep Learning from Private Training Data. ICLR 2017  
https://openreview.net/forum?id=HkwoSDP  
> The paper presents a general teacher-student approach for differentially-private learning in which the student learns to predict a noise vote among a set of teachers. The noise allows the student to be differentially private, whilst maintaining good classification accuracies on MNIST and SVHN. 
> It divides the dataset to some disjoint subsets and provide client-level dp, then use semi-supervised learning to utlize non-private unlabeled data and obtain a student model. Bscause aggregation is much easier to add noise than learning. Take notice of that this framework don't limit the teacher models and student model, which is different from ([Jihun Hamm ICML 2016](http://proceedings.mlr.press/v48/hamm16.html)).


Yu-Feng Li, Han-Wen Zha, Zhi-Hua Zhou:  
Learning Safe Prediction for Semi-Supervised Regression. AAAI 2017: 2217-2223  
https://aaai.org/ocs/index.php/AAAI/AAAI17/paper/view/14587  
> A safe prediction from multiple semi-supervised regressors, which is better than a supervised learner in the worset situation. To be detailed, the problem is transfromed to a projection.

## Federated Learning

Eugene Bagdasaryan, Andreas Veit, Yiqing Hua, Deborah Estrin, Vitaly Shmatikov:  
How To Backdoor Federated Learning. CoRR abs/1807.00459 (2018)  
https://arxiv.org/abs/1807.00459  
> It demonstrates that any participant in federated learning can introduce hidden backdoor functionality into the joint global model. By model replacement, the inside attacker can make the global model to behave a certain way on specific, attack-chosen backdoor inputs, while global model maintains good accuracy on main task.

Abhishek Bhowmick, John Duchi, Julien Freudiger, Gaurav Kapoor, Ryan Rogers:  
Protection Against Reconstruction and Its Applications in Private Federated Learning. CoRR abs/1812.00984 (2018)  
https://arxiv.org/abs/1812.00984  
> They devlop a new private mechanism for releasing high dimensional vectors to applied in federated learning. To be detailed, it separately privatize vector's direction and magnitude. As a result, they show the experiment in image classification and language models that is comparable to federated learning without these privacy restrictions.

Stacey Truex, Nathalie Baracaldo, Ali Anwar, Thomas Steinke, Heiko Ludwig, Rui Zhang:  
A Hybrid Approach to Privacy-Preserving Federated Learning. CoRR abs/1812.03224 (2018)  
https://arxiv.org/abs/1812.03224  
> Differentially private federated learning with secure multiparty computation(SMC)  
> It utilizes SMC to reduce the noise added on gradient.

Keith Bonawitz, Vladimir Ivanov, Ben Kreuter, Antonio Marcedone, H. Brendan McMahan, Sarvar Patel, Daniel Ramage, Aaron Segal, Karn Seth:  
Practical Secure Aggregation for Privacy-Preserving Machine Learning. ACM Conference on Computer and Communications Security 2017: 1175-1191  
https://dl.acm.org/citation.cfm?doid=3133956.3133982  
> A new efficient technology to handle multi-party computation for high dimension vectors.


Brendan McMahan, Eider Moore, Daniel Ramage, Seth Hampson, Blaise Agüera y Arcas:  
Communication-Efficient Learning of Deep Networks from Decentralized Data. AISTATS 2017: 1273-1282  
http://proceedings.mlr.press/v54/mcmahan17a.html  
> Federated Learning


Robin C. Geyer, Tassilo Klein, Moin Nabi:  
Differentially Private Federated Learning: A Client Level Perspective. CoRR abs/1712.07557 (2017)  
https://arxiv.org/abs/1712.07557  
> Client-level dp protection, the method is the same with the dp-sgd which regards the client's database as a bag.

---
## Distributed Learning

Bargav Jayaraman, Lingxiao Wang, David Evans, Quanquan Gu:  
Distributed Learning without Distress: Privacy-Preserving Empirical Risk Minimization. NeurIPS 2018: 6346-6357  
http://papers.nips.cc/paper/7871-distributed-learning-without-distress-privacy-preserving-empirical-risk-minimization  
Code:https://github.com/bargavj/distributedMachineLearning  
> It combines differential privacy and secure multi-party computation in the application of distributed learning. The output perturbation method is computationally more efficient and gradient perturbation method maintains high accuracy regardless of how the data is partitioned.
> ps: To be personally, the second method that iteratively compuate the gradient is the same as federated learning.

Jihun Hamm, Yingjun Cao, Mikhail Belkin:  
Learning privately from multiparty data. ICML 2016: 555-563  
http://proceedings.mlr.press/v48/hamm16.html  
> It use cheap auxiliary unlabeled data and local classifier ensemble to create fresh labeled data and then train a differentially private classifier. Notice that, the student model should be a private learning which be limited in convex and linear in differentially private scenario.

Manas A. Pathak, Shantanu Rane, Bhiksha Raj:  
Multiparty Differential Privacy via Aggregation of Locally Trained Classifiers. NIPS 2010: 1876-1884  
http://papers.nips.cc/paper/4034-multiparty-differential-privacy-via-aggregation-of-locally-trained-classifiers  
> It constructs SMC to average the multipary model parameters and add the noise to result, such that it provides client-level protection.

## Security Principles

Martín Abadi, Úlfar Erlingsson, Ian J. Goodfellow, H. Brendan McMahan, Ilya Mironov, Nicolas Papernot, Kunal Talwar, Li Zhang:  
On the Protection of Private Information in Machine Learning Systems: Two Recent Approches. CSF 2017: 1-6  
https://ieeexplore.ieee.org/document/8049647  
> It compares Noisy-SGD and PATE on some fundamental principles when designing a privacy-protection system.

---

## Local Differential Privacy


Differential Privacy Team, Apple:  
Learning with privacy at scale. 2017  
https://machinelearning.apple.com/docs/learning-with-privacy-at-scale/appledifferentialprivacysystem.pdf  
> Apple's LDP solution on Frequency Estimation  
> It combines Count Mean Sketch(a kind of hash method) and randomized response to realize local differential privacy. Besides, it uses Hadamard basis transform to reduce communcation between client and server.

Bolin Ding, Janardhan Kulkarni, Sergey Yekhanin:  
Collecting Telemetry Data Privately. NIPS 2017: 3574-3583  
http://papers.nips.cc/paper/6948-collecting-telemetry-data-privately  
> Microsoft's LDP solution to handle continous collection of data.  
> Compared the memoization in RAPPOR, it adds rounding to protect user's private numeric values with small but frequent changes.

Tianhao Wang, Jeremiah Blocki, Ninghui Li, Somesh Jha:  
Locally Differentially Private Protocols for Frequency Estimation. USENIX Security Symposium 2017: 729-745  
https://www.usenix.org/conference/usenixsecurity17/technical-sessions/presentation/wang-tianhao  
> - The survey about existing LDP protocols on frequency estimation.
> - Propose a pure framework and cast existing protocols(RAPPOR, Random Matrix Projection) into it.
> - It utilizes the framework to optimize Unary Encoding(Basic RAPPOR) and Binary Local Hashing(Random Matrix Projection) and comp up with Optimal UE and Optimal Local Hashing.

Kazuto Fukuchi, Quang Khai Tran, Jun Sakuma:  
Differentially Private Empirical Risk Minimization with Input Perturbation. DS 2017: 82-90  
https://link.springer.com/chapter/10.1007%2F978-3-319-67786-6_6  
> It propose a framework(input perturbation) for ERM, use the representation(p,q) replace the original data(feature,label) in loss function. However, there isn't efficient solution in this paper.

Thông T. Nguyên, Xiaokui Xiao, Yin Yang, Siu Cheung Hui, Hyejin Shin, Junbum Shin:  
Collecting and Analyzing Data from Smart Device Users with Local Differential Privacy. CoRR abs/1606.05053 (2016)  
https://arxiv.org/abs/1606.05053  
> - Harmony: a method to estimate mean and frequencies for multi-dimensional data containing both numerical and categorical attributes
> - Local differentially private ERM: distributed sgd


Giulia C. Fanti, Vasyl Pihur, Úlfar Erlingsson:  
Building a RAPPOR with the Unknown: Privacy-Preserving Learning of Associations and Data Dictionaries. PoPETs 2016(3): 41-61 (2016)  
https://content.sciendo.com/view/journals/popets/2016/3/article-p41.xml  
>Estimate the joint distribution of multi-attributes generated by RAPPOR.  
>Work on unknown dictionary where the domain of attributes is unknown, regard these as a special category 'others'.

Naoise Holohan, Douglas J. Leith, Oliver Mason:  
Optimal Differentially Private Mechanisms for Randomised Response. IEEE Trans. Information Forensics and Security 12(11): 2726-2735 (2017)  
https://ieeexplore.ieee.org/document/7967624  
> For binary output, this paper gives optimal differentially private mechanism for random response, includes strict and relaxed differential privacy

Yue Wang, Xintao Wu, Donghui Hu:  
Using Randomized Response for Differential Privacy Preserving Data Collection. EDBT/ICDT Workshops 2016  
http://ceur-ws.org/Vol-1558/paper35.pdf  
>For an attribute(binary/polychotomous), compare the utlity preservation between Randomized Response and Laplace Mechanism, and prove that Randomized Response outperforms the Laplace Mechanism.

Úlfar Erlingsson, Vasyl Pihur, Aleksandra Korolova:  
RAPPOR: Randomized Aggregatable Privacy-Preserving Ordinal Response. ACM Conference on Computer and Communications Security 2014: 1054-1067  
https://doi.org/10.1145/2660267.2660348  
code: https://github.com/google/rappor  
> Google's LDP solution to handle one-time and tracking attacker.  
> It constructs 2 levels's protection using Permanent randomized response and Instantaneous randomized response, the former is used to handle one-time collection and the later is used to handle windowed attacker who has access to multiple reports over time from the same user.

John C. Duchi, Michael I. Jordan, Martin J. Wainwright:  
Local Privacy and Statistical Minimax Rates. FOCS 2013: 429-438  
https://ieeexplore.ieee.org/document/6686179?arnumber=6686179&tag=1  
> - propose local differential privacy  
> - ~~prove something~~

---

## Machine Learning with Differential privacy

Jaewoo Lee, Daniel Kifer:  
Concentrated Differentially Private Gradient Descent with Adaptive per-Iteration Privacy Budget. KDD 2018: 1656-1665  
> The motivation is that we need more accurate gradients in later iteration. And this is the first private gradient-based algorithm in which the privacy budget and step size for each iteration is dynamically determined at runtime based on the quality of the noisy statistics obtained for the current iteration.

Jiaqi Zhang, Kai Zheng, Wenlong Mou, Liwei Wang:
Efficient Private ERM for Smooth Objectives. IJCAI 2017: 3922-3928  
https://www.ijcai.org/proceedings/2017/548  
>- Gradient descent method with output perturbation. Compared with previous work(Raef Bassily, 2014), they improve the running time and show better experimental results.  
>- Expand dp-GD to non-convex but smooth objectives. The method looks like that (Raef Bassily, 2014), the privacy and utility are been guaranteed in this paper.  
  
  
Beyza Ermis, Ali Taylan Cemgil:  
Differentially Private Dropout. CoRR abs/1712.01665 (2017)  
http://arxiv.org/abs/1712.01665  
>introduce a noise interpretation to dropout, and prove the noise on gradient satisfies dp  

Yining Wang, Yu-Xiang Wang, Aarti Singh:  
Differentially private subspace clustering. NIPS 2015: 1000-1008  
http://papers.nips.cc/paper/5991-differentially-private-subspace-clustering  
> It utilities local sensitivity and the assumption which dataset is well-separated in k-subspace clustering to realize the subspace clustering with differential privacy. More specially, it proposed two method that use sample and aggregate framework and exponential mechanism respectively.


Raef Bassily, Adam D. Smith, Abhradeep Thakurta:  
Private Empirical Risk Minimization: Efficient Algorithms and Tight Error Bounds. FOCS 2014: 464-473  
https://arxiv.org/pdf/1405.7085.pdf  
>利用sgd采样随机性的dp实现  
>给出了dpERM的经验误差下界  
>基于Localization+EM的可实现的参数求解框架(相较之前的(Kifer,2012)框架，给出了一个可实现的解法)  


Shuang Song, Kamalika Chaudhuri, Anand D. Sarwate:  
Stochastic gradient descent with differentially private updates. GlobalSIP 2013: 245-248  
https://ieeexplore.ieee.org/document/6736861  
>sgd的dp版本，基于一次梯度下降的函数敏感度对梯度加入噪声
>mini-batch版本获得梯度提升
>为了避免因迭代引起的privacy衰减，每个batch是不相交的，对整个数据集只能遍历一遍


Jun Zhang, Xiaokui Xiao, Yin Yang, Zhenjie Zhang, Marianne Winslett:  
PrivGene: differentially private model fitting using genetic algorithms. SIGMOD Conference 2013: 665-676  
http://davidyinyang.weebly.com/uploads/9/8/6/2/9862052/privgene_final.pdf
>将遗传算法的每一步作隐私化处理构建了满足差分隐私的参数求解方法  
>提出了EEM(增强的指数机制)用于隐私地选择，当候选参数随着迭代求解过程而趋于相同时，EEM较EM能提供更小的噪声  

  
Daniel Kifer, Adam D. Smith, Abhradeep Thakurta:  
Private Convex Optimization for Empirical Risk Minimization with Applications to High-dimensional Regression. COLT 2012: 25.1-25.40  
http://101.96.10.63/www.cse.psu.edu/~ads22/pubs/KST12/KST12-2012-06-07-Colt-camera.pdf  
>在目标扰动上引入高斯噪声，有更低的期望误差  
>证明了目标扰动的privateERM在带有非处处可微的正则项时依然满足dp  
>分析了对于稀疏回归场景的应用（在一个较优的候选区域求解）  


Kamalika Chaudhuri, Claire Monteleoni, Anand D. Sarwate:  
Differentially Private Empirical Risk Minimization. Journal of Machine Learning Research 12: 1069-1109 (2011)  
https://dl.acm.org/citation.cfm?id=2021036  
>纠正了前一篇文章(Chaudhuri, 2008)中的错误，正式提出了一类基于经验误差最小化方法的dp框架privateERM  
>对输出扰动和目标扰动两种方法的泛化误差进行了分析  
>应用于logistic回归和svm的性能分析  


Kamalika Chaudhuri, Claire Monteleoni:  
Privacy-preserving logistic regression. NIPS 2008: 289-296  
http://www.cse.psu.edu/~ads22/privacy598/papers/cm08.pdf  
>分析了带正则逻辑回归输出的函数敏感度，提出了在输出上增加Laplace噪声达成dp的lr  
>在目标函数中增加随机向量b，由b的随机性导出优化求得解的随机性，称为目标扰动的lr  

Kobbi Nissim, Sofya Raskhodnikova, Adam D. Smith:  
Smooth sensitivity and sampling in private data analysis. STOC 2007: 75-84  
https://doi.org/10.1145/1250790.1250803  
> It proposed the concept of local sensitivity, that can be considered to add noise and make the protection. In some cases, the local sensitivity is much smaller than the global sensitivity and to maintain the uility of algorithm. However, the local computation of local sensitivity is difficult. To handle it, it provides the sample and aggregate framework to approximate the local sensitivity.


---

## Composition of differential privacy


Martín Abadi, Andy Chu, Ian J. Goodfellow, H. Brendan McMahan, Ilya Mironov, Kunal Talwar, Li Zhang:  
Deep Learning with Differential Privacy. ACM Conference on Computer and Communications Security 2016: 308-318  
https://arxiv.org/pdf/1607.00133.pdf  
>Moments accountant with tighter estimates on the overall privacy loss  
>Apply the accountant to neural networks  

Cynthia Dwork, Guy N. Rothblum, Salil P. Vadhan:  
Boosting and Differential Privacy. FOCS 2010: 51-60  
https://ieeexplore.ieee.org/document/5670947  
>"Strong Composition"  
>Boosting for Queries  

---

## dp histogram publishing

Dong Su, Jianneng Cao, Ninghui Li, Min Lyu:  
PrivPfC: differentially private data publication for classification. VLDB J. 27(2): 201-223 (2018)  
https://link.springer.com/article/10.1007%2Fs00778-017-0492-3  
>PrivPfC，在DiffGen的基础上针对更多特征的数据集和二分类任务进行了优化，通过生成Generalization候选映射，然后直接选择的方式，略去了DiffGen中的迭代过程  
code:https://github.com/DongSuIBM/PrivPfC


Noman Mohammed, Rui Chen, Benjamin C. M. Fung, Philip S. Yu:  
Differentially private data release for data mining. KDD 2011: 493-501  
https://dl.acm.org/citation.cfm?id=2020408.2020487  
>DiffGen,在满足dp的框架下实现隐私保护中常用的Generalization方法发布匿名化数据集，赋予其可证的保护程度  
code:https://github.com/McGill-DMaS/DiffGen  

---

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

---

## Differential Privacy (Source)

Cynthia Dwork, Frank McSherry, Kobbi Nissim, Adam D. Smith:  
Calibrating Noise to Sensitivity in Private Data Analysis. TCC 2006: 265-284  
https://link.springer.com/chapter/10.1007%2F11681878_14  

Cynthia Dwork:  
Differential Privacy. ICALP (2) 2006: 1-12  
https://link.springer.com/chapter/10.1007%2F11787006_1  

---

## OverView and Tutorials

Qiang Yang, Yang Liu, Tianjian Chen, Yongxin Tong  
Federated Machine Learning: Concept and Applications. ACM Transactions on Intelligent Systems and Technology (TIST) Volume 10 Issue 2, Article No. 12, January 2019  
https://arxiv.org/abs/1902.04885  

Graham Cormode, Somesh Jha, Tejas Kulkarni, Ninghui Li, Divesh Srivastava, Tianhao Wang:  
Privacy at Scale: Local Differential Privacy in Practice. SIGMOD Conference 2018: 1655-1658  
http://dimacs.rutgers.edu/~graham/pubs/html/CormodeJhaKulkarniLiSrivastavaWang18.html  


Tianqing Zhu, Gang Li, Wanlei Zhou, Philip S. Yu:  
Differential Privacy and Applications. Advances in Information Security 69, Springer 2017, ISBN 978-3-319-62002-2, pp. 1-222  
https://link.springer.com/book/10.1007%2F978-3-319-62004-6  



Tianqing Zhu, Gang Li, Wanlei Zhou, Philip S. Yu:  
Differentially Private Data Publishing and Analysis: A Survey. IEEE Trans. Knowl. Data Eng. 29(8): 1619-1638 (2017)  
https://ieeexplore.ieee.org/document/7911185  


Kamalika Chaudhuri, Anand D. Sarwate:  
Differentially Private Machine Learning: Theory, Algorithms, and Applications       nips2017 tutorial  
https://www.ece.rutgers.edu/~asarwate/nips2017/  


Ninghui Li, Min Lyu, Dong Su, Weining Yang:  
Differential Privacy: From Theory to Practice. Synthesis Lectures on Information Security, Privacy, & Trust, Morgan & Claypool Publishers 2016, pp. 1-138  
https://ieeexplore.ieee.org/document/7731575?bkn=7731575  


Cynthia Dwork, Aaron Roth:  
The Algorithmic Foundations of Differential Privacy. Foundations and Trends in Theoretical Computer Science 9(3-4): 211-407 (2014)  
http://nowpublishers.com/article/DownloadSummary/TCS-042  


