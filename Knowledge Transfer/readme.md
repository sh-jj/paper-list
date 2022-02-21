
# Domain Adaptation

* ## Custom Domain Adaptation
  * [Instance Weighting for Domain Adaptation in NLP.](https://www.aclweb.org/anthology/P07-1034.pdf) (ACL 2007, 732 citations)
  * [Covariate Shift Adaptation by Importance Weighted Cross Validation.](http://www.jmlr.org/papers/v8/sugiyama07a.html) (JMLR 2007, 550 citations)
  * ⭐️ [Learning Bounds for Domain Adaptation.](http://papers.nips.cc/paper/3212-learning-bounds-for-domain-adaptation) (NIPS 2008, 316 citations)
  * [Learning Transferable Features with Deep Adaptation Networks.](http://proceedings.mlr.press/v37/long15.html) (ICML 2015)
    > They use MMD to measure the distribution discrepancy between source features and target features. It promoted the applications of deep learning on transfer learning.
  * [AutoDIAL: Automatic DomaIn Alignment Layers]() (ICCV 2017
    > They employ BathchNorm Layer to align data distribution cross domains.  
  * [Boosting for Transfer Learning.](https://dl.acm.org/doi/abs/10.1145/1273496.1273521) (ICML 2017)  
  * ⭐️ [Maximum Classifier Discrepancy for Unsupervised Domain Adaptation](http://openaccess.thecvf.com/content_cvpr_2018/html/Saito_Maximum_Classifier_Discrepancy_CVPR_2018_paper.html) (CVPR 2018, 282 citations)

  * [Domain-Specific Batch Normalization for Unsupervised Domain Adaptation](https://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_Domain-Specific_Batch_Normalization_for_Unsupervised_Domain_Adaptation_CVPR_2019_paper.pdf) (CVPR 2019) ([Code](https://github.com/wgchang/DSBN))
    > They design BathchNorm Layer for source/target domain to align them on reperestations-level. It could be easily extend to multi-source setting.
  * [Transfer Learning via Minimizing the PerformanceGap Between Domains](http://papers.nips.cc/paper/9249-transfer-learning-via-minimizing-the-performance-gap-between-domains) (NeurIPS 2019)
  * [Federated Adversarial Domain Adaptation.](https://arxiv.org/abs/1911.02054) (ICLR 2020)
   
  
* ## Multi-Source Domain Adaptation

  * [Domain Adaptation with Multiple Sources.](http://papers.nips.cc/paper/3550-domain-adaptation-with-multiple-sources) (NIPS 2009, 294 citations)
  * ⭐️[Algorithms and Theory for Multiple-Source Adaptation.](https://arxiv.org/pdf/1805.08727.pdf) (NeurIPS 2018) ([Bibtex](https://dblp.uni-trier.de/rec/conf/nips/HoffmanMZ18.html?view=bibtex))

    > They give an amazing theoretical analysis about weighted distribution ensemble, which provides robustness for multi-source domain adaptation.
    >
  * [Multiple Source Domain Adaptation with Adversarial Learning](https://arxiv.org/pdf/1705.09684.pdf)

    > Combine the "Multiple-Source Adaptation" and "Adversarial Adaptation"
    >
  * [Moment Matching for Multi-Source Domain Adaptation](https://arxiv.org/pdf/1812.01754.pdf) (ICCV 2019, [Homepage](http://ai.bu.edu/M3SDA/#dataset), [Code](https://github.com/VisionLearningGroup/VisionLearningGroup.github.io/tree/master/M3SDA/code_MSDA_digit), [Unofficial Code](https://github.com/xiechen0692/Moment-Matching-for-Multi-Source-Domain-Adaptation-M3SDA))

    > Propose a dataset "DomainNet".
  * [A Discriminative Technique for Multiple-Source Adaptation](http://proceedings.mlr.press/v139/cortes21b/cortes21b.pdf) (ICML 2021)
* ## Multi-Target Domain Adaptation

  * [Unsupervised Multi-Target Domain Adaptation: An Information Theoretic Approach](https://ieeexplore.ieee.org/abstract/document/8970464) (TIP 2020)
    > Minimize the mutual information between domain-invariant features and domain-specific features to adapt to multi-target domains.
    >
* ## Domain Agnostic Learning / Latent Domain Adaptation

  > Target data has mixed domains without domain labels.
  >

  * [Discovering Latent Domains for Multisource Domain Adaptation.](https://link.springer.com/content/pdf/10.1007%2F978-3-642-33709-3_50.pdf) (ECCV 2012)
  * [Latent Domains Modeling for Visual Domain Adaptation](https://www.aaai.org/ocs/index.php/AAAI/AAAI14/paper/view/8418/8641) (AAAI 2014)
  * ⭐️ [Inferring Latent Domains for Unsupervised Deep Domain Adaptation.](https://arxiv.org/abs/2103.13873) (TPAMI 2019) ([Code](https://github.com/mancinimassimiliano/latent_domains_DA), [Bibtex](https://dblp.uni-trier.de/rec/journals/pami/ManciniPBCR21.html?view=bibtex))

    > They use multi-domain domain alignment (normalization) layer to mine the multiple latent domain structure, a side branch to predict the domain label.
    >
  * ⭐️ [Domain Agnostic Learning with Disentangled Representations](http://proceedings.mlr.press/v97/peng19b.html) (ICML 2019) ([Code](https://github.com/VisionLearningGroup/DAL))

    > Disentangle the domain-specific features to promote the extraction of domain-invariant features.
    >
  * [⭐️ Open Compound Domain Adaptation]() (CVPR 2020) ([Homepage](https://liuziwei7.github.io/projects/CompoundDomain))

    > Utilize domain-spefic features to adapt unlabled data gradually via Curriculum Learing.
    >
  * [Discover, Hallucinate, and Adapt: Open Compound Domain Adaptation for Semantic Segmentation](https://arxiv.org/abs/2110.04111) (NeurIPS 2020)
  * 
* ## Heterogeneous Features
  * [Translated Learning: Transfer Learning across Different Feature Spaces](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.145.5832&rep=rep1&type=pdf) (NIPS 2008)
  * [Heterogeneous Transfer Learning for Image Classification](https://www.aaai.org/ocs/index.php/AAAI/AAAI11/paper/viewPaper/3671) (AAAI 2011)


## Incremental Domain Adaptation
* ## Gradual Domain Adaptation
   * ⭐ [Understanding Self-Training for Gradual Domain Adaptation](http://proceedings.mlr.press/v119/kumar20c/kumar20c.pdf) (ICML 2020, [code](https://github.com/p-lambda/gradual_domain_adaptation))
   * 
## Partial Domain Adaptation

## Others

# Domain Generalization

# Multi-Task Learning
* ## Homogeneous
    * [Adaptive Smoothed Online Multi-Task Learning](http://papers.nips.cc/paper/6433-adaptive-smoothed-online-multi-task-learning) (NIPS 2016)  
    * [Federated Multi-Task Learning](http://papers.nips.cc/paper/7029-federated-multi-task-learning) (NIPS 2017)
    * [Multi-task Learning with Labeled and Unlabeled Tasks.](https://dl.acm.org/citation.cfm?id=3305971) (ICML 2017)
    * [Robust Learning from Untrusted Sources](https://arxiv.org/abs/1901.10310)  (ICML2019, [code](https://github.com/NikolaKon1994/Robust-Learning-from-Untrusted-Sources))
      > For untrusted data sources with different data quality, it use weighted empirical loss to achieve collaborative learning. To learn the weight of different sources, it introduces a small clean dataset and measure the distance between the clean dataset and local dataset. During the estimation of weight of untrusted sources, the procedure can rely on gradient descent only.
* ## Heterogeneous Features
    * [Multi-Task Learning in Heterogeneous Feature Spaces](https://ojs.aaai.org/index.php/AAAI/article/view/7909/7768&hl=zh-CN&sa=T&oi=gsb-gga&ct=res&cd=0&d=12997287504521233539&ei=htMcYe_DFIr2yATNnK7YAg&scisig=AAGBfm24A0r9yL-AN-gNsiMnBy6vQiRWEQ) (AAAI 2011)

# Few-Shot Learning
* ## Custom
  * [Meta-Learning with Memory-Augmented Neural Networks.](http://proceedings.mlr.press/v48/santoro16.html) (ICML 2016)  
      > They employ a external memory module (like cache) to storage the reperastion of data from previous tasks.Such a design is similar to knn, except that only the reperastion vectors are stored here.
   
  * [Meta Networks.](https://dl.acm.org/citation.cfm?id=3305945) (ICML 2017)  
      > In few-shot learning, it's difficult to parameterize model rapidly through a few examples. They employ loss gradient as meta information and generate fast parameters for learner by a meta-learner. Base learner consists of slow parameters (optimized on specific-task) and fast parameters (generated by meta-leaner with meta-information across tasks).  
   
  * [Prototypical Networks for Few-shot Learning.](http://papers.nips.cc/paper/6996-prototypical-networks-for-few-shot-learning) (NIPS 2017)  
      > "Prototype", a way imitating humans to understand the world. They build a meta-learner mapping instances to a low-dimensional space, and the prototypes of various categories are obtained by clustering. For target task in few-shot learning, the prototypes are built by meta-learner and answer the queries through neighbor-based method. 
  * [Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks](http://proceedings.mlr.press/v70/finn17a.html) (ICML 2017)
* ## Semi-Supervised Few-Shot Learning
  * [Meta-Learning for Semi-Supervised Few-Shot Classification](https://openreview.net/forum?id=HJcSzz-CZ) (ICLR 2018)
    > This paper extends the prototypical network to semi-supervised scheme. Mask clusters are employed to handle the unexpected instances which doesn't belong to the target task. Such a way of mining unlabeled data is rough and have space for improvement. However, the key problem in this situation is that there is a long way from existing few-shot learning method to practice.
  * [Task Cooperation for Semi-Supervised Few-Shot Learning](https://www.aaai.org/AAAI21Papers/AAAI-5922.YeHJ.pdf) (AAAI 2021)
  * [Tailoring Embedding Function to Heterogeneous Few-Shot Tasks by Global and Local Feature Adaptors](http://www.lamda.nju.edu.cn/lus/files/AAAI21_GLoFA.pdf) (AAAI 2021)


# Life-Long Learning
* ## Ensemble-based
    * [Expert Gate: Lifelong Learning with a Network of Experts](https://arxiv.org/pdf/1611.06194.pdf) (CVPR 2017)
        > maintain a model pool during lifelong learning  
        > use autoencoder as model sperification and estimate task relatedness through reconstruction loss.

# Class Incremental Learning
* Custom
    * [Co-Transport for Class-Incremental Learning](https://arxiv.org/pdf/2107.12654.pdf) (MM 2021)
    * [Detecting Sequentially Novel Classes with Stable Generalization Ability](https://link.springer.com/chapter/10.1007%2F978-3-030-75762-5_30) (PAKDD 2021)

# Open-Set Recognition / Out-of-distribution data detection
[Learning Placeholders for Open-Set Recognition](http://www.lamda.nju.edu.cn/zhoudw/file/CVPR21/CVPR21.pdf) (CVPR 2021)

## Datasets

  * Multitask Dataset of Product Reviews: http://cvml.ist.ac.at/productreviews/
  
  * Animals with Attributes 2: https://cvml.ist.ac.at/AwA2/
  
  * ECMLPKDD2006 Spam Classification http://ecmlpkdd2006.org/challenge.html
  
