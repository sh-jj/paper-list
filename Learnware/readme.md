# Learnware
[Learnware](https://cs.nju.edu.cn/zhouzh/zhouzh.files/publication/fcs16learnware.pdf) is proposed by Pr. Zhi-Hua Zhou in 2016.
## Model Reuse
  Build a model based on limited labeled data (or unlabeled data), with the help of well-trained models from related tasks.

* ## Covariate Shift 
  * [Modal Consistency Based Pre-trained Multi-Model Reuse](https://www.ijcai.org/proceedings/2017/0459.pdf) (IJCAI 2017)
  * [Model Reuse with Reduced Kernel Mean Embedding Specification.](https://arxiv.org/abs/2001.07135) (TKDE 2021)
  * [Towards Enabling Learnware to Handle Unseen Jobs](http://129.211.169.156/publication/aaai21_unseenJob.pdf) (AAAI 2021)
  * [Towards Robust Model Reuse in the Presence of Latent Domains](https://www.ijcai.org/proceedings/2021/0407.pdf) (IJCAI 2021)
  * 
* ## Concept Shift
  
  * [Handling Concept Drift via Model Reuse](https://link.springer.com/article/10.1007/s10994-019-05835-w) (ML 2020)
  * [Boosting-Based Reliable Model Reuse](http://proceedings.mlr.press/v129/ding20a/ding20a.pdf) (ACML 2020)
  * [Rapid Performance Gain through Active Model Reuse.](http://www.lamda.nju.edu.cn/liyf/paper/ijcai19-acmr.pdf) (IJCAI 2019)
  * [Exploiting the Intrinsic Neighborhood Structure for Source-free Domain Adaptation](https://arxiv.org/pdf/2110.04202.pdf) (NeurIPS 2021)
  * 
  
* ## Features Shift / Reuse with Heterogeneous Features

  * [Rectify Heterogeneous Models with Semantic Mapping](http://proceedings.mlr.press/v80/ye2018c/ye2018c.pdf) (ICML 2018)

  
* ## Labels Shift / Reuse with Heterogeneous Labels
  * [FitNets: Hints for Thin Deep Nets](https://arxiv.org/abs/1412.6550) (2014)    
  * [Deep Learning for Fixed Model Reuse](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/viewPaper/14586) (AAAI 2017)
  * [Learning What and Where to Transfer.](https://arxiv.org/abs/1905.05901) (ICML 2019)
  * [Heterogeneous Model Reuse via Optimizing Multiparty Multiclass Margin](http://proceedings.mlr.press/v97/wu19c/wu19c.pdf) (ICML 2019)
  * [Learning New Tricks From Old Dogs: Multi-Source Transfer Learning From Pre-Trained Networks.](http://papers.nips.cc/paper/8688-learning-new-tricks-from-old-dogs-multi-source-transfer-learning-from-pre-trained-networks) (NeurIPS 2019)
     <!-- > This paper has tried to mine the ability of multi-source during transfer. Sepecially, they propose maximal correlation weighting to generate an ensemble module to utilize the internal output from multiple pre-trained networks.
     > In my opinion, it seems like the custom stacking where the second model designed by maximize correlation.  
     > So, what kind of ensemble module is reasonable? robust? efficient? ... -->
  * [Distilling Cross-Task Knowledge via Relationship Matching](https://openaccess.thecvf.com/content_CVPR_2020/papers/Ye_Distilling_Cross-Task_Knowledge_via_Relationship_Matching_CVPR_2020_paper.pdf) (CVPR 2020)
  * [Co-Tuning for Transfer Learning](http://ise.thss.tsinghua.edu.cn/~mlong/doc/co-tuning-for-transfer-learning-nips20.pdf) (NeurIPS 2020)
  * [LogME: Practical Assessment of Pre-trained Models for Transfer Learning](http://ise.thss.tsinghua.edu.cn/~mlong/doc/LogME-Practical-Assessment-of-Pre-trained-Models-for-Transfer-Learning-icml21.pdf) (ICML 2021)

* ## Architecture Shift / Distillation
  * [Distilling the Knowledge in a Neural Network.](https://arxiv.org/abs/1503.02531) (2015)     
  * [Explaining Knowledge Distillation by Quantifying the Knowledge.](https://arxiv.org/abs/2003.03622) (CVPR 2020)  
  * [Contrastive representation distillation.](https://arxiv.org/abs/1910.10699) (ICLR 2020)  
  * 
## Model Evolution
  Evolve the model from the training environment to an open and dynamic environment.
* ## Features Shift / Learning with Evolving Features
  * [Learning with Feature Evolvable Streams](https://arxiv.org/pdf/1706.05259.pdf) (NIPS 2017)
  * [Rectify Heterogeneous Models with Semantic Mapping](http://proceedings.mlr.press/v80/ye2018c/ye2018c.pdf) (ICML 2018)
  * [Learning with Feature and Distribution Evolvable Streams](http://proceedings.mlr.press/v119/zhang20ad/zhang20ad.pdf) (ICML 2020)
  * [Storage Fit Learning with Feature Evolvable Streams](https://arxiv.org/abs/2007.11280) (AAAI 2021)
  * [Exploratory Machine Learning with Unknown Unknowns](https://www.aaai.org/AAAI21Papers/AAAI-6937.ZhaoP.pdf) (AAAI 2021)
* ## Label Shift / Learning with Evolving Classes
  * [Classification and novel class detection in concept-drifting data streams under time constraints](https://ieeexplore.ieee.org/abstract/document/5453372/) (TKDE 2011)
  * [Streaming Classification with Emerging New Class by Class Matrix Sketching](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/view/14514/14419) (AAAI 2017)
  * [iCaRL: Incremental Classifier and Representation Learning ](http://openaccess.thecvf.com/content_cvpr_2017/html/Rebuffi_iCaRL_Incremental_Classifier_CVPR_2017_paper.html) (CVPR 2017)  
  <!-- >  Use deep feature extractor and nearest-prototype discriminator to learning the novel classes during streaming data. -->  
  * [One-Pass Learning with Incremental and Decremental Features](https://arxiv.org/abs/1605.09082) (TPMAI 2018)
  * [Semi-Supervised Streaming Learning with Emerging New Labels](https://www.aaai.org/Papers/AAAI/2020GB/AAAI-ZhuY.4960.pdf) (AAAI 2020)
  * [Co-Transport for Class-Incremental Learning](https://dl.acm.org/doi/pdf/10.1145/3474085.3475306) (MM 2021)

  
