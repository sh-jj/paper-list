# Model Reuse

* ## Latent Domains
  * [Towards Robust Model Reuse in the Presence of Latent Domains](https://www.ijcai.org/proceedings/2021/0407.pdf)
* ## Heterogeneous Features
  * [Rectify Heterogeneous Models with Semantic Mapping](http://proceedings.mlr.press/v80/ye2018c/ye2018c.pdf) (ICML 2018)
  * [Learning with Feature Evolvable Streams](https://arxiv.org/pdf/1706.05259.pdf) (NIPS 2017)

# Multi-Task Learning

* ## Heterogeneous Multi-Task Learning
    * [Multi-Task Learning in Heterogeneous Feature Spaces](https://ojs.aaai.org/index.php/AAAI/article/view/7909/7768&hl=zh-CN&sa=T&oi=gsb-gga&ct=res&cd=0&d=12997287504521233539&ei=htMcYe_DFIr2yATNnK7YAg&scisig=AAGBfm24A0r9yL-AN-gNsiMnBy6vQiRWEQ) (AAAI 2011)

# Domain Adaptation

* ## Custom Domain Adaptation
  * 🌟[Domain Adaptation: Learning Bounds and Algorithms](https://arxiv.org/pdf/0902.3430.pdf)
  * 
  * [Learning Transferable Features with Deep Adaptation Networks.](http://proceedings.mlr.press/v37/long15.html) (ICML 2015)

    > They use MMD to measure the distribution discrepancy between source features and target features. It promoted the applications of deep learning on transfer learning.
    >
  * [Instance Weighting for Domain Adaptation in NLP.](https://www.aclweb.org/anthology/P07-1034.pdf) (ACL 2007, 732 citations)
  * [Covariate Shift Adaptation by Importance Weighted Cross Validation.](http://www.jmlr.org/papers/v8/sugiyama07a.html) (JMLR 2007, 550 citations)
  * [Learning Bounds for Domain Adaptation.](http://papers.nips.cc/paper/3212-learning-bounds-for-domain-adaptation) (NIPS 2008, 316 citations)
  * [AutoDIAL: Automatic DomaIn Alignment Layers]() (ICCV 2017
    > They employ BathchNorm Layer to align data distribution cross domains.
  * [⭐️ Maximum Classifier Discrepancy for Unsupervised Domain Adaptation](http://openaccess.thecvf.com/content_cvpr_2018/html/Saito_Maximum_Classifier_Discrepancy_CVPR_2018_paper.html) (CVPR 2018, 282 citations)

  * [Domain-Specific Batch Normalization for Unsupervised Domain Adaptation](https://openaccess.thecvf.com/content_CVPR_2019/papers/Chang_Domain-Specific_Batch_Normalization_for_Unsupervised_Domain_Adaptation_CVPR_2019_paper.pdf) (CVPR 2019) ([Code](https://github.com/wgchang/DSBN))
    > They design BathchNorm Layer for source/target domain to align them on reperestations-level. It could be easily extend to multi-source setting.

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
    >
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

## Incremental Domain Adaptation
##  Partial Domain Adaptation

## Others

# Domain Generalization

##
