
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

