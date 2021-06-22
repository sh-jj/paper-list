# paper-list

## Learning with Augemented Class

Qing Da, Yang Yu, Zhi-Hua Zhou:
Learning with Augmented Class by Exploiting Unlabeled Data. AAAI 2014: 1760-1766
> Based on the idea of large margin, make separator close to the positive labeled data and far from the negative labeled data to handle the augmented class. As a result, predictors tend to classify abnormal unlabeled data as negative.

Semi-Supervised Streaming Learning with Emerging New Labels. AAAI 2020
> For streaming data, take abnormal unlabeled data as a new class, and use LP to mine unlabeled data.

Jeremy Nixon, Jeremiah Liu, David Berthelot:  
Semi-Supervised Class Discovery. CoRR abs/2002.03480 (2020)  
https://arxiv.org/abs/2002.03480  
> They use label reconstruction accuracy to measure the effect of new class filter.



## Robust learning

Nikola Konstantinov, Christoph Lampert:  
Robust Learning from Untrusted Sources. ICML2019  
https://arxiv.org/abs/1901.10310  
> For untrusted data sources with different data quality, it use weighted empirical loss to achieve collaborative learning. To learn the weight of different sources, it introduces a small clean dataset and measure the distance between the clean dataset and local dataset. During the estimation of weight of untrusted sources, the procedure can rely on gradient descent only.

Dong Yin, Yudong Chen, Kannan Ramchandran, Peter Bartlett:  
Byzantine-Robust Distributed Learning: Towards Optimal Statistical Rates. ICML 2018: 5636-5645  
https://arxiv.org/abs/1803.01498  
> Byzantine failure in distributed learning: means that some worker machines may behave completely arbitrarily and can send any message to the master machine. They provided two method: median-based GD and trimmed-mean-based GD, that achieve optimal statistical rates.

Jiashi Feng, Huan Xu, Shie Mannor:  
Distributed Robust Learning. CoRR abs/1409.5937 (2014)  
https://arxiv.org/pdf/1409.5937.pdf  
> For distributed learning of linear model, choose the geometric median of local learned model.


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

## Unsupervised Learning with differential privacy

Liyang Xie, Kaixiang Lin, Shu Wang, Fei Wang, Jiayu Zhou:  
Differentially Private Generative Adversarial Network. CoRR abs/1802.06739 (2018)  
https://arxiv.org/abs/1802.06739  
code: https://github.com/illidanlab/dpgan

Uri Stemmer, Haim Kaplan:  
Differentially Private k-Means with Constant Multiplicative Error. NeurIPS 2018: 5436-5446  
http://papers.nips.cc/paper/7788-differentially-private-k-means-with-constant-multiplicative-error  
> It combines the private candidate and private coreset to construct a more accurate clustering.

Maria-Florina Balcan, Travis Dick, Yingyu Liang, Wenlong Mou, Hongyang Zhang:  
Differentially Private Clustering in High-Dimensional Euclidean Spaces. ICML 2017: 322-331  
http://proceedings.mlr.press/v70/balcan17a.html  
>It projects data to low-dimension and find candidate set for clustering, and recover it to high-dimension. It ensures that dense areas are more likely to be retained by dividing space privately.


Dan Feldman, Chongyuan Xiang, Ruihao Zhu, Daniela Rus:  
Coresets for differentially private k-means clustering and applications to privacy in mobile sensor networks. IPSN 2017: 3-15  
https://ieeexplore.ieee.org/document/7944775  
> They proposed a new private coreset construction, and run k-means on coreset to get tighter bound than [[Feldman's 2009](https://dl.acm.org/citation.cfm?doid=1536414.1536465)]. The new coreset construction is based on subroutine to find a small ball contains enough points privately. This subroutine is proposed in [[Locating a Small Cluster Privately. PODS2016](https://doi.org/10.1145/2902251.2902296)]

Yining Wang, Yu-Xiang Wang, Aarti Singh:  
Differentially private subspace clustering. NIPS 2015: 1000-1008  
http://papers.nips.cc/paper/5991-differentially-private-subspace-clustering  
> It utilities local sensitivity and the assumption which dataset is well-separated in k-subspace clustering to realize the subspace clustering with differential privacy. More specially, it proposed two method that use sample and aggregate framework and exponential mechanism respectively.

Dan Feldman, Amos Fiat, Haim Kaplan, Kobbi Nissim:  
Private coresets. STOC 2009: 361-370  
https://dl.acm.org/citation.cfm?doid=1536414.1536465 
> Coreset is a notation in computational geometry which be used to approximate the queries on original points. This paper show that coreset with differential privacy can be built by efficient algorithm. Especially, for the queries like k-means or k-median, they provide theoretical bound.The private coreset construction is based on division and count on original points like hash.  
> Notice:  
The non-private coreset is excepted to be built within fewer points, but private coreset may be larger than original set.  
The private coreset for other purpose are worthy for exploring.


Kobbi Nissim, Sofya Raskhodnikova, Adam D. Smith:  
Smooth sensitivity and sampling in private data analysis. STOC 2007: 75-84  
https://doi.org/10.1145/1250790.1250803  
> It proposed the concept of local sensitivity, that can be considered to add noise and make the protection. In some cases, the local sensitivity is much smaller than the global sensitivity and to maintain the uility of algorithm. However, the local computation of local sensitivity is difficult. To handle it, it provides the sample and aggregate framework to approximate the local sensitivity.


## Weakly Supervised Learning


Yu-Feng Li, Lan-Zhe Guo, Zhi-Hua Zhou:  
Towards Safe Weakly Supervised Learning. IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), in press.
> For some candidate weakly supervised learners, it use a min-max framework to optimize the worst-case performance gain against base supervised learner.

Hai Wang, Shao-Bo Wang, Yu-Feng Li:  
Instance selection method for improving graph-based semi-supervised learning. Frontiers Comput. Sci. 12(4): 725-735 (2018)  
http://lamda.nju.edu.cn/liyf/paper/FCS18-gsslis.pdf  
> It use confidence to aggregate prediction by SSL based on different kinds of graph and decrease the risk of performance degeneration.

Anh T. Pham, Jing Xi:  
Differentially Private Semi-Supervised Learning With Known Class Priors. BigData 2018: 801-810  
https://ieeexplore.ieee.org/document/8622071
> It presents a framework for semi-supervised learning, assuming known class priors, and provides the theoretical guarantee on the optimal risk. Under this setting, they give the differentially private learning on the framework. However, they make mistakes on addition of noise, which have been corrected in [[Kamalika Chaudhuri 2011](https://dl.acm.org/citation.cfm?id=2021036)].

Nicolas Papernot, Martín Abadi, Úlfar Erlingsson, Ian J. Goodfellow, Kunal Talwar:  
Semi-supervised Knowledge Transfer for Deep Learning from Private Training Data. ICLR 2017  
https://openreview.net/forum?id=HkwoSDP  
> The paper presents a general teacher-student approach for differentially-private learning in which the student learns to predict a noise vote among a set of teachers. The noise allows the student to be differentially private, whilst maintaining good classification accuracies on MNIST and SVHN.  
> It divides the dataset to some disjoint subsets and provide client-level dp, then use semi-supervised learning to utlize non-private unlabeled data and obtain a student model. Bscause aggregation is much easier to add noise than learning. Take notice of that this framework don't limit the teacher models and student model, which is different from ([Jihun Hamm ICML 2016](http://proceedings.mlr.press/v48/hamm16.html)).

Xu Long, Jun Sakuma:  
Differentially Private Semi-Supervised Classification. SMARTCOMP 2017: 1-6  
https://ieeexplore.ieee.org/document/7947001  
> For a specific SSL(tranductive k-NN learning), it considers privacy of labeled instances and proivdes differentially private protection.  
> However, it ignores privacy of unlabeled instances and the setting(k-mutual neighbor) limits the effect of unlabeled instances.

Yu-Feng Li, Han-Wen Zha, Zhi-Hua Zhou:  
Learning Safe Prediction for Semi-Supervised Regression. AAAI 2017: 2217-2223  
https://aaai.org/ocs/index.php/AAAI/AAAI17/paper/view/14587  
> A safe prediction from multiple semi-supervised regressors, which is better than a supervised learner in the worset situation. To be detailed, the problem is transfromed to a projection.

Yu-Feng Li, Shao-Bo Wang, Zhi-Hua Zhou:  
Graph Quality Judgement: A Large Margin Expedition. IJCAI 2016: 1725-1731  
http://lamda.nju.edu.cn/liyf/paper/ijcai16-lead.pdf  
> If we have some prediction based on different SSL, we can build a aggregation as 'LEAD', which this paper proposed to maximize the margin of unlabeled data. A larger margin on unlabeled data means lower risk of performance degeneration. For this purpose, it use S3VM to learn a linear combination of multiple prediction by different SSL, which have the max margin.

Yu-Feng Li, Zhi-Hua Zhou:  
Towards Making Unlabeled Data Never Hurt. IEEE Trans. Pattern Anal. Mach. Intell. 37(1): 175-188 (2015)  
http://lamda.nju.edu.cn/liyf/paper/TPAMI15-S4VM.pdf  
> There are more than a large margin in semi-supervised data, which are diverse, choose one of them directly may lead to performance degeneration. It use S3VMs to generate a pool of separators, and maximize the worst-case improvement over inductive SVM, the method proposed are called S4VM.

Geetha Jagannathan, Claire Monteleoni, Krishnan Pillaipakkamnatt:  
A Semi-Supervised Learning Approach to Differential Privacy. ICDM Workshops 2013: 841-848  
https://ieeexplore.ieee.org/document/6754008  
> It expends dp Random Decision Tree to utlize unlabeled data, but it only consider the privacy of labeled data. The unlabeled data is considered to be public and non-private. In general, it utlize unlabeled data as auxiliary information to boost performance of dp mechanism.

Yu-Feng Li, Zhi-Hua Zhou:  
Improving Semi-Supervised Support Vector Machines Through Unlabeled Instances Selection. AAAI 2011  
http://lamda.nju.edu.cn/liyf/paper/aaai11-s3vm-us.pdf  
> If we have got prediction from SVM and S3VM, it proposed a method to provide guide which prediction we should choose. It performed hierarchical clustering on unlabeled data, and use the delta of the length of the paths from instance_i to its nearest positive and negative labeled instances to represent the confidence. The higher confidence means lower risk of the unlabled instances. For unlabeled instances with higher confdence, we would predict it by S3VM, otherwises by SVM.  
> It have not exclude influence on S3VM by unlabeled instances with high risk.

Pavan Kumar Mallapragada, Rong Jin, Anil K. Jain, Yi Liu:  
SemiBoost: Boosting for Semi-Supervised Learning. IEEE Trans. Pattern Anal. Mach. Intell. 31(11): 2000-2014 (2009)  
https://ieeexplore.ieee.org/document/4633363  
> SemiBoost is a framework that leverages unlabeled data to enhance an existing supervised learning algorithm. By using cluster hypothesis and manifold hypothesis in semi-supervised learning, it's a mixture of self-training, graph-based semi-supervised learning and adaboost. In self-training, pseudo-labels are used to enhance the model (manifold hypothesis), and the selected samples with high confidence are usually far away from the decision boundary and have little value. SemiBoost adds the similarity measure from graph-based semi-supervised learning into objective function to enlarge the decision boundary (clustering hypothesis). The overall improvement process of boosting is similar to Adaboost.


Helmut Grabner, Christian Leistner, Horst Bischof:  
Semi-supervised On-Line Boosting for Robust Tracking. ECCV (1) 2008: 234-247  
https://link.springer.com/chapter/10.1007%2F978-3-540-88682-2_19  
> It modified the SemiBoost to a online version, then track the online adaptation.

Christian Leistner, Helmut Grabner, Horst Bischof:  
Semi-supervised boosting using visual similarity learning. CVPR 2008  
https://www.computer.org/10.1109/CVPR.2008.4587629  
> Based on SemiBoost, they use a given classifier as prior to measure the similarity between samples.

Jing Jiang, ChengXiang Zhai:
Instance Weighting for Domain Adaptation in NLP. ACL 2007
https://www.aclweb.org/anthology/P07-1034
> A framework to weight the instances(label/unlabeled data) in the situation of domain adaption.  


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


## OverView and Tutorials

Yu-Feng Li, De-Ming Liang  
Safe Semi-Supervised Learning: A Brief Introduction. Frontiers of Computer Science (FCS)  
http://lamda.nju.edu.cn/liyf/paper/fcs19-safessl.pdf  

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


