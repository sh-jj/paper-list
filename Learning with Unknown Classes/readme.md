


## With Abnormal Class
_Some unlabeled examples are from classes which are not present in the target class distribution._  
_It's particularly related to outlier detection._

### Surveys
* [Realistic Evaluation of Deep Semi-Supervised Learning Algorithms](http://papers.nips.cc/paper/7585-realistic-evaluation-of-de) (NIPS 2018, 200 citations) [[Code](https://github.com/brain-research/realistic-ssl-evaluation
)]

### Metric-based 
* [LOF: Identifying Density-Based Local Outliers](https://dl.acm.org/doi/abs/10.1145/342009.335388) (SIGMOD 2000, 5000+ citations)
  >  Calculate the degree of anomaly (outlier factor) for each data point according to the density difference around its neighbors.
* [Meta-Learning for Semi-Supervised Few-Shot Classification](https://arxiv.org/abs/1803.00676) (ICLR 2018, 175 citations) [[Code](https://github.com/renmengye/few-shot-ssl-public)]
  > Learn the distance density and scope of each class prototype (cluster) to exclude abnormal unlabeled data.
  
## With Emerging Class 
_In streaming data, novel classes emerge which are not present in the training set._  
_It includes new-class detection, known-class classification, and model update. That is different from traditional classification problem or novel class detection (or anomaly detection) because those problems are equivalent to one of the three tasks,
without addressing classification or model update._

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
