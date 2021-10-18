
# Weakly Supervised Learning

## Semi-Supervised Learning

[Dash: Semi-Supervised Learning with Dynamic Thresholding](https://proceedings.mlr.press/v139/xu21e.html) (ICML 2021)

Towards Safe Weakly Supervised Learning. (TPAMI 2021)
> For some candidate weakly supervised learners, it use a min-max framework to optimize the worst-case performance gain against base supervised learner.

[Lightweight Label Propagation for Large-Scale Network Data](http://www.lamda.nju.edu.cn/liyf/paper/ijcai18-slp.pdf) (TKDE 2021)


Instance selection method for improving graph-based semi-supervised learning.  (FCS 2018)  
http://lamda.nju.edu.cn/liyf/paper/FCS18-gsslis.pdf  
> It use confidence to aggregate prediction by SSL based on different kinds of graph and decrease the risk of performance degeneration.

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

## Multi-instance Learning
[Deep multiple instance selection](http://scis.scichina.com/en/2021/130102.pdf) (SCIENCE CHINA: Information Sciences 2021)

[Multi-Instance Learning With Emerging Novel Class](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8896009) (TKDE 2021)


