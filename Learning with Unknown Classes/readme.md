


## With Abnormal Class
_Some unlabeled examples are from classes which are not present in the target class distribution._  
_It's particularly related to outlier detection._

### Surveys

* [Realistic Evaluation of Deep Semi-Supervised Learning Algorithms](http://papers.nips.cc/paper/7585-realistic-evaluation-of-de) (NIPS 2018, 200 citations) [[Code](https://github.com/brain-research/realistic-ssl-evaluation
)]
* [Deep learning for anomaly detection: A survey](https://arxiv.org/abs/1901.03407) (2018, 137 citations)

### Metric-based 
* [LOF: Identifying Density-Based Local Outliers](https://dl.acm.org/doi/abs/10.1145/342009.335388) (SIGMOD 2000, 5000+ citations)
  >  Calculate the degree of anomaly (outlier factor) for each data point according to the density difference around its neighbors.
  
* [iCaRL: Incremental Classifier and Representation Learning ](http://openaccess.thecvf.com/content_cvpr_2017/html/Rebuffi_iCaRL_Incremental_Classifier_CVPR_2017_paper.html) (CVPR 2017, 378 citations)  
  >  Use deep feature extractor and nearest-prototype discriminator to learning the novel classes during streaming data.
  
* [Meta-Learning for Semi-Supervised Few-Shot Classification](https://arxiv.org/abs/1803.00676) (ICLR 2018, 175 citations) [[Code](https://github.com/renmengye/few-shot-ssl-public)]
  > Learn the distance density and scope of each class prototype (cluster) to exclude abnormal unlabeled data.
### Tree-based

* [Isolation Forest](https://cs.nju.edu.cn/zhouzh/zhouzh.files/publication/icdm08b.pdf) (ICDM 2008, 1100+ citations)
  > Isolation means 'separating an instance from the rest of the instances'. Anomaly instances generally require less partitions to be isolated (shorter path).  
  > - The fewer instances of anomalies result in a smaller number of partitions - shorter pathes in a tree structure.  
  > - Instances with distinguishable attribute-values are more likely to be separated in early partitioning.  

### Margin-based
* [Support Vector Method for Novelty Detection](http://papers.nips.cc/paper/1723-support-vector-method-for-novelty-detection.pdf) (NIPS 2000, 1261 citations)
* [Learning with Augmented Class by Exploiting Unlabeled Data](https://www.aaai.org/ocs/index.php/AAAI/AAAI14/paper/viewPaper/8388) (AAAI 2014)
* [High-dimensional and large-scale anomaly detection using a linear one-class SVM with deep learning](https://www.sciencedirect.com/science/article/pii/S0031320316300267) (PR 2016, 379 citations)
* [Anomaly Detection using One-Class Neural Networks](https://arxiv.org/abs/1802.06360) (2018, 86 citations) [[Code](https://github.com/raghavchalapathy/oc-nn)]


  
## With Emerging Class 
_In streaming data, novel classes emerge which are not present in the training set._  
_It includes novel-class detection, known-class classification, and model update. That is different from traditional classification problem or novel class detection (or anomaly detection) because those problems are equivalent to one of the three tasks,
without addressing classification or model update._  
_To handle streaming data, we need to pay attention to the computation cost and memory cost of the algorithm._

### Metric-based
* [Streaming Classification with Emerging New Class by Class Matrix Sketching](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/view/14514/14419) (AAAI 2017)

### Tree-based

* [Semi-Supervised Streaming Learning with Emerging New Labels](https://www.aaai.org/Papers/AAAI/2020GB/AAAI-ZhuY.4960.pdf) (AAAI 2020)

## With Extended Class
_Unlabeled data contains multiple potential target classes that are not present in the labeled training set._  
_Compared with 'Learning with Abnormal Class', the instances belonging to potential target classes may not rare._  
_Compared with 'Learning with Emerging Class', there always be multiple potential classes at the same time, which requires us to distinguish these instances belonging to new classes._

### Metric-based
* [Semi-Supervised Class Discovery](https://arxiv.org/abs/2002.03480).
  > A key to class discovery is to judge if a novel class (and its corresponding examples) we found could be updated into the model. This paper uses Dataset Reconstruction Accuracy, which measures if the detector could recover the label of known-classes instances, to represent the ability of detector.
