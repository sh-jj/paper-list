# Differential Privacy

* ## 0. Pivot

    * [Cynthia Dwork, Frank McSherry, Kobbi Nissim, Adam D. Smith: Calibrating Noise to Sensitivity in Private Data Analysis. TCC 2006: 265-284](https://link.springer.com/chapter/10.1007%2F11681878_14)

    * [Cynthia Dwork:  Differential Privacy. ICALP (2) 2006: 1-12](https://link.springer.com/chapter/10.1007%2F11787006_1)

* ## 1. General Machine Learning with Differential Privacy

    * Differentially Private Learning with Small Public Data
        > There are two key factors in differentailly private SGD, privacy budget and gredient clipping threshold at each iteration. Private-Public (PPSGD) is prosposed, which use small public labeled data to estimate these factors at next iteration.

    * [Martín Abadi, Úlfar Erlingsson, Ian J. Goodfellow, H. Brendan McMahan, Ilya Mironov, Nicolas Papernot, Kunal Talwar, Li Zhang:  On the Protection of Private Information in Machine Learning Systems: Two Recent Approches. CSF 2017: 1-6](https://ieeexplore.ieee.org/document/8049647)
        > It compares Noisy-SGD and PATE on some fundamental principles when designing a privacy-protection system.

    * [Jaewoo Lee, Daniel Kifer:  
    Concentrated Differentially Private Gradient Descent with Adaptive per-Iteration Privacy Budget. KDD 2018: 1656-1665](
    https://dl.acm.org/citation.cfm?doid=3219819.3220076)
        > The motivation is that we need more accurate gradients in later iteration. And this is the first private gradient-based algorithm in which the privacy budget and step size for each iteration is dynamically determined at runtime based on the quality of the noisy statistics obtained for the current iteration.

    * [Jiaqi Zhang, Kai Zheng, Wenlong Mou, Liwei Wang: Efficient Private ERM for Smooth Objectives. IJCAI 2017: 3922-3928](https://www.ijcai.org/proceedings/2017/548)
        >- Gradient descent method with output perturbation. Compared with previous work(Raef Bassily, 2014), they improve the running time and show better experimental results.  
        >- Expand dp-GD to non-convex but smooth objectives. The method looks like that (Raef Bassily, 2014), the privacy and utility are been guaranteed in this paper.  
  
  
    * [Beyza Ermis, Ali Taylan Cemgil:  Differentially Private Dropout. CoRR abs/1712.01665 (2017) ](http://arxiv.org/abs/1712.01665)
        > introduce a noise interpretation to dropout, and prove the noise on gradient satisfies dp  


    * Xu Long, Jun Sakuma: Differentially Private Semi-Supervised Classification. SMARTCOMP 2017: 1-6

    * [Raef Bassily, Adam D. Smith, Abhradeep Thakurta: Private Empirical Risk Minimization: Efficient Algorithms and Tight Error Bounds. FOCS 2014: 464-473](https://arxiv.org/pdf/1405.7085.pdf)
        > - Implementation of differential privacy by using sampling randomness of sgd
        > - The lower bound of the empirical error of dpERM is given
        > - Realizable parameter solution framework based on Localization+EM (compared to the previous (Kifer, 2012) framework, an achievable solution is given)

    * [Shuang Song, Kamalika Chaudhuri, Anand D. Sarwate:   Stochastic gradient descent with differentially private updates. GlobalSIP 2013: 245-248](https://ieeexplore.ieee.org/document/6736861)
        > - The dp version of sgd, which adds noise to the gradient based on the sensitivity of a gradient descent function
        > - Mini-batch gradient descent
        > - In order to avoid privacy attenuation caused by iteration, each batch is disjoint, and the entire data set can only be traversed once


    * [Jun Zhang, Xiaokui Xiao, Yin Yang, Zhenjie Zhang, Marianne Winslett: PrivGene: differentially private model fitting using genetic algorithms. SIGMOD Conference 2013: 665-676](http://davidyinyang.weebly.com/uploads/9/8/6/2/9862052/privgene_final.pdf)
        > - Each step of the genetic algorithm is privately processed to construct a parameter solution method that satisfies differential privacy 
        > - EEM (Enhanced Exponential Mechanism) is proposed for private selection. When the candidate parameters tend to be the same with the iterative solution process, EEM can provide less noise than EM

    * [Daniel Kifer, Adam D. Smith, Abhradeep Thakurta:  Private Convex Optimization for Empirical Risk Minimization with Applications to High-dimensional Regression. COLT 2012: 25.1-25.40](http://101.96.10.63/www.cse.psu.edu/~ads22/pubs/KST12/KST12-2012-06-07-Colt-camera.pdf)  
        > - Introduce Gaussian noise to the target disturbance, with lower expected error
        > - It is proved that the privateERM with target disturbance still satisfies dp with non-every differentiable regular terms
        > - Analyzed the application of sparse regression scenarios (solved in a better candidate area)


    * [Kamalika Chaudhuri, Claire Monteleoni, Anand D. Sarwate:  Differentially Private Empirical Risk Minimization. Journal of Machine Learning Research 12: 1069-1109 (2011)](https://dl.acm.org/citation.cfm?id=2021036)
        > - Corrected the errors in the previous article (Chaudhuri, 2008), and formally proposed a class of dp framework privateERM based on empirical error minimization methods
        > - The generalization errors of the two methods of output disturbance and target disturbance are analyzed.
        > - Performance analysis applied to logistic regression and svm

    * [Kamalika Chaudhuri, Claire Monteleoni:  Privacy-preserving logistic regression. NIPS 2008: 289-296](http://www.cse.psu.edu/~ads22/privacy598/papers/cm08.pdf)
        > - The sensitivity of the function with regular logistic regression output is analyzed, and the lr that increases Laplace noise on the output to achieve dp is proposed.
        > - The random vector b is added to the objective function, and the randomness of the optimized solution is derived from the randomness of b, which is called lr of the target perturbation

    * [Arik Friedman, Assaf Schuster:  Data mining with differential privacy. KDD 2010: 493-502](https://doi.org/10.1145/1835804.1835868)
        > Differentially private ID3 algorithm. They split the node by exponential mechanism, and relize pruning by 'error based pruning'.

* ##  2. Private Distributed Learning

    * [Bargav Jayaraman, Lingxiao Wang, David Evans, Quanquan Gu:  Distributed Learning without Distress: Privacy-Preserving Empirical Risk Minimization. NeurIPS 2018: 6346-6357](http://papers.nips.cc/paper/7871-distributed-learning-without-distress-privacy-preserving-empirical-risk-minimization)
    [Code](https://github.com/bargavj/distributedMachineLearning)
    > - It combines differential privacy and secure multi-party computation in the application of distributed learning. The output perturbation method is computationally more efficient and gradient perturbation method maintains high accuracy regardless of how the data is partitioned.
    > - ps: To be personally, the second method that iteratively compuate the gradient is the same as federated learning.

    * [Jihun Hamm, Yingjun Cao, Mikhail Belkin:  Learning privately from multiparty data. ICML 2016: 555-563](http://proceedings.mlr.press/v48/hamm16.html)
        > It use cheap auxiliary unlabeled data and local classifier ensemble to create fresh labeled data and then train a differentially private classifier. Notice that, the student model should be a private learning which be limited in convex and linear in differentially private scenario.

    * [Manas A. Pathak, Shantanu Rane, Bhiksha Raj: Multiparty Differential Privacy via Aggregation of Locally Trained Classifiers. NIPS 2010: 1876-1884](http://papers.nips.cc/paper/4034-multiparty-differential-privacy-via-aggregation-of-locally-trained-classifiers)
        > It constructs SMC to average the multipary model parameters and add the noise to result, such that it provides client-level protection.
        Eugene Bagdasaryan, Andreas Veit, Yiqing Hua, Deborah Estrin, Vitaly Shmatikov:  
* ##  3. Private Federated Learning

    
    > Differential Private [Federated Learning](http://proceedings.mlr.press/v54/mcmahan17a.html).

    * [Abhishek Bhowmick, John Duchi, Julien Freudiger, Gaurav Kapoor, Ryan Rogers:  Protection Against Reconstruction and Its Applications in Private Federated Learning. CoRR abs/1812.00984 (2018)](https://arxiv.org/abs/1812.00984)
        > They devlop a new private mechanism for releasing high dimensional vectors to applied in federated learning. To be detailed, it separately privatize vector's direction and magnitude. As a result, they show the experiment in image classification and language models that is comparable to federated learning without these privacy restrictions.

    * [Stacey Truex, Nathalie Baracaldo, Ali Anwar, Thomas Steinke, Heiko Ludwig, Rui Zhang:  A Hybrid Approach to Privacy-Preserving Federated Learning. CoRR abs/1812.03224 (2018)](https://arxiv.org/abs/1812.03224)
        > Differentially private federated learning with secure multiparty computation(SMC)  
        > It utilizes SMC to reduce the noise added on gradient.

    * [Keith Bonawitz, Vladimir Ivanov, Ben Kreuter, Antonio Marcedone, H. Brendan McMahan, Sarvar Patel, Daniel Ramage, Aaron Segal, Karn Seth: Practical Secure Aggregation for Privacy-Preserving Machine Learning. ACM Conference on Computer and Communications Security 2017: 1175-1191](https://dl.acm.org/citation.cfm?doid=3133956.3133982)
        > A new efficient technology to handle multi-party computation for high dimension vectors.


    


    * [Robin C. Geyer, Tassilo Klein, Moin Nabi:  Differentially Private Federated Learning: A Client Level Perspective. CoRR abs/1712.07557 (2017)](https://arxiv.org/abs/1712.07557)  
        > Client-level dp protection, the method is the same with the dp-sgd which regards the client's database as a bag.

* ## 4. Unsupervised Learning with differential privacy

    * [Liyang Xie, Kaixiang Lin, Shu Wang, Fei Wang, Jiayu Zhou: Differentially Private Generative Adversarial Network. CoRR abs/1802.06739 (2018)](https://arxiv.org/abs/1802.06739)  
    [code](https://github.com/illidanlab/dpgan)

    * [Uri Stemmer, Haim Kaplan:  Differentially Private k-Means with Constant Multiplicative Error. NeurIPS 2018: 5436-5446](http://papers.nips.cc/paper/7788-differentially-private-k-means-with-constant-multiplicative-error)  
        > It combines the private candidate and private coreset to construct a more accurate clustering.

    * [Maria-Florina Balcan, Travis Dick, Yingyu Liang, Wenlong Mou, Hongyang Zhang:  Differentially Private Clustering in High-Dimensional Euclidean Spaces. ICML 2017: 322-331](http://proceedings.mlr.press/v70/balcan17a.html)
        >It projects data to low-dimension and find candidate set for clustering, and recover it to high-dimension. It ensures that dense areas are more likely to be retained by dividing space privately.


    * [Dan Feldman, Chongyuan Xiang, Ruihao Zhu, Daniela Rus:  Coresets for differentially private k-means clustering and applications to privacy in mobile sensor networks. IPSN 2017: 3-15](https://ieeexplore.ieee.org/document/7944775)
        > They proposed a new private coreset construction, and run k-means on coreset to get tighter bound than [[Feldman's 2009](https://dl.acm.org/citation.cfm?doid=1536414.1536465)]. The new coreset construction is based on subroutine to find a small ball contains enough points privately. This subroutine is proposed in [[Locating a Small Cluster Privately. PODS2016](https://doi.org/10.1145/2902251.2902296)]

    * [Yining Wang, Yu-Xiang Wang, Aarti Singh:  Differentially private subspace clustering. NIPS 2015: 1000-1008](http://papers.nips.cc/paper/5991-differentially-private-subspace-clustering)
        > It utilities local sensitivity and the assumption which dataset is well-separated in k-subspace clustering to realize the subspace clustering with differential privacy. More specially, it proposed two method that use sample and aggregate framework and exponential mechanism respectively.

    * [Dan Feldman, Amos Fiat, Haim Kaplan, Kobbi Nissim: Private coresets. STOC 2009: 361-370](https://dl.acm.org/citation.cfm?doid=1536414.1536465)
        > Coreset is a notation in computational geometry which be used to approximate the queries on original points. This paper show that coreset with differential privacy can be built by efficient algorithm. Especially, for the queries like k-means or k-median, they provide theoretical bound.The private coreset construction is based on division and count on original points like hash.  
        > Notice:  The non-private coreset is excepted to be built within fewer points, but private coreset may be larger than original set.  The private coreset for other purpose are worthy for exploring.

    * [Kobbi Nissim, Sofya Raskhodnikova, Adam D. Smith:  Smooth sensitivity and sampling in private data analysis. STOC 2007: 75-84](https://doi.org/10.1145/1250790.1250803)
        > It proposed the concept of local sensitivity, that can be considered to add noise and make the protection. In some cases, the local sensitivity is much smaller than the global sensitivity and to maintain the uility of algorithm. However, the local computation of local sensitivity is difficult. To handle it, it provides the sample and aggregate framework to approximate the local sensitivity.
* ## 5. Other Private Machine Learning Applications
    * [Liyang Xie, Kaixiang Lin, Shu Wang, Fei Wang, Jiayu Zhou:  Differentially Private Generative Adversarial Network. CoRR abs/1802.06739 (2018)](https://arxiv.org/abs/1802.06739)  
    [code](https://github.com/illidanlab/dpgan)

    * [Quanming Yao, Xiawei Guo, James T. Kwok, WeiWei Tu, Yuqiang Chen, Wenyuan Dai, Qiang Yang: Differential Private Stack Generalization with an Application to Diabetes Prediction. CoRR abs/1811.09491 (2018)](https://arxiv.org/abs/1811.09491)  
        > First, Split the data to low-level and high-level, then divide low-level dataset into some disjoint subsets. Generate privacy-preserving logistic regression on the disjoint subsets, then stacking on the high-level dataset.  
        > Motivation? multiparty data?

* ## 6. Local Differential Privacy


    * [Differential Privacy Team, Apple:  Learning with privacy at scale. 2017](https://machinelearning.apple.com/docs/learning-with-privacy-at-scale/appledifferentialprivacysystem.pdf)
        > Apple's LDP solution on Frequency Estimation  
        > It combines Count Mean Sketch(a kind of hash method) and randomized response to realize local differential privacy. Besides, it uses Hadamard basis transform to reduce communcation between client and server.

    * [Bolin Ding, Janardhan Kulkarni, Sergey Yekhanin: Collecting Telemetry Data Privately. NIPS 2017: 3574-3583](http://papers.nips.cc/paper/6948-collecting-telemetry-data-privately)  
        > Microsoft's LDP solution to handle continous collection of data.  
        > Compared the memoization in RAPPOR, it adds rounding to protect user's private numeric values with small but frequent changes.

    * [Tianhao Wang, Jeremiah Blocki, Ninghui Li, Somesh Jha:  Locally Differentially Private Protocols for Frequency Estimation. USENIX Security Symposium 2017: 729-745](https://www.usenix.org/conference/usenixsecurity17/technical-sessions/presentation/wang-tianhao)
        > - The survey about existing LDP protocols on frequency estimation.
        > - Propose a pure framework and cast existing protocols(RAPPOR, Random Matrix Projection) into it.
        > - It utilizes the framework to optimize Unary Encoding(Basic RAPPOR) and Binary Local Hashing(Random Matrix Projection) and comp up with Optimal UE and Optimal Local Hashing.

    * [Kazuto Fukuchi, Quang Khai Tran, Jun Sakuma: Differentially Private Empirical Risk Minimization with Input Perturbation. DS 2017: 82-90](https://link.springer.com/chapter/10.1007%2F978-3-319-67786-6_6)  
        > It propose a framework(input perturbation) for ERM, use the representation(p,q) replace the original data(feature,label) in loss function. However, there isn't efficient solution in this paper.

    * [Thông T. Nguyên, Xiaokui Xiao, Yin Yang, Siu Cheung Hui, Hyejin Shin, Junbum Shin:  Collecting and Analyzing Data from Smart Device Users with Local Differential Privacy. CoRR abs/1606.05053 (2016)](https://arxiv.org/abs/1606.05053)  
        > - Harmony: a method to estimate mean and frequencies for multi-dimensional data containing both numerical and categorical attributes
        > - Local differentially private ERM: distributed sgd


    * [Giulia C. Fanti, Vasyl Pihur, Úlfar Erlingsson:  Building a RAPPOR with the Unknown: Privacy-Preserving Learning of Associations and Data Dictionaries. PoPETs 2016(3): 41-61 (2016)](https://content.sciendo.com/view/journals/popets/2016/3/article-p41.xml)  
        > - Estimate the joint distribution of multi-attributes generated by RAPPOR.  
        > - Work on unknown dictionary where the domain of attributes is unknown, regard these as a special category 'others'.

    * [Naoise Holohan, Douglas J. Leith, Oliver Mason:  Optimal Differentially Private Mechanisms for Randomised Response. IEEE Trans. Information Forensics and Security 12(11): 2726-2735 (2017)](https://ieeexplore.ieee.org/document/7967624)
        > - For binary output, this paper gives optimal differentially private mechanism for random response, includes strict and relaxed differential privacy

    * [Yue Wang, Xintao Wu, Donghui Hu: Using Randomized Response for Differential Privacy Preserving Data Collection. EDBT/ICDT Workshops 2016](http://ceur-ws.org/Vol-1558/paper35.pdf)
        > - For an attribute(binary/polychotomous), compare the utlity preservation between Randomized Response and Laplace Mechanism, and prove that Randomized Response outperforms the Laplace Mechanism.

    * [Úlfar Erlingsson, Vasyl Pihur, Aleksandra Korolova:  RAPPOR: Randomized Aggregatable Privacy-Preserving Ordinal Response. ACM Conference on Computer and Communications Security 2014: 1054-1067](https://doi.org/10.1145/2660267.2660348)
    [code](https://github.com/google/rappor)  
        > - Google's LDP solution to handle one-time and tracking attacker.  
        > - It constructs 2 levels's protection using Permanent randomized response and Instantaneous randomized response, the former is used to handle one-time collection and the later is used to handle windowed attacker who has access to multiple reports over time from the same user.

    * [John C. Duchi, Michael I. Jordan, Martin J. Wainwright:  Local Privacy and Statistical Minimax Rates. FOCS 2013: 429-438](https://ieeexplore.ieee.org/document/6686179?arnumber=6686179&tag=1)  
        > - propose local differential privacy  
        > - ~~prove something~~

* ## 7. Privacy loss accouting for differential privacy

    * [Aleksei Triastcyn, Boi Faltings:  Improved Accounting for Differentially Private Learning. CoRR abs/1901.09697 (2019)]( https://arxiv.org/abs/1901.09697)
        > It sums up the moment accountant(Abadi, 2016) as generic privacy accountant.
        > In machine learning, data usually have the same potential distribution. Based on such 'local privacy', it proposes bayesian privacy accountant, which have a tighter bound.

    * [Ilya Mironov:  Rényi Differential Privacy. CSF 2017: 263-275](https://ieeexplore.ieee.org/document/8049725)
        > Based on Rényi Divergence, they proposed a relaxed notion of differential privacy. By Rényi Differential Privacy, the privacy loss accounting of gaussian noise is easier.  

    * [frank mcsherry:  How many secrets do you have?](https://github.com/frankmcsherry/blog/blob/master/posts/2017-02-08.md)

    * [Martín Abadi, Andy Chu, Ian J. Goodfellow, H. Brendan McMahan, Ilya Mironov, Kunal Talwar, Li Zhang:  Deep Learning with Differential Privacy. ACM Conference on Computer and Communications Security 2016: 308-318](https://arxiv.org/pdf/1607.00133.pdf)
    > - Moments accountant with tighter estimates on the overall privacy loss  
    > - Apply the accountant to neural networks  

    * [Cynthia Dwork, Guy N. Rothblum, Salil P. Vadhan:  Boosting and Differential Privacy. FOCS 2010: 51-60](https://ieeexplore.ieee.org/document/5670947)
    > - "Strong Composition"  
    > - Boosting for Queries  

* ## 8. Histogram Publishing
    * [Dong Su, Jianneng Cao, Ninghui Li, Min Lyu: PrivPfC: differentially private data publication for classification. VLDB J. 27(2): 201-223 (2018)](https://link.springer.com/article/10.1007%2Fs00778-017-0492-3)  
    >PrivPfC，basd on DiffGen, it optimized for more feature data sets and binary classification tasks. The iterative process in DiffGen is omitted by generating Generalization candidate mappings and then directly selecting them.
    ([code](https://github.com/DongSuIBM/PrivPfC))


    * [Noman Mohammed, Rui Chen, Benjamin C. M. Fung, Philip S. Yu: Differentially private data release for data mining. KDD 2011: 493-501](https://dl.acm.org/citation.cfm?id=2020408.2020487)
    >DiffGen, under the framework of dp, realizes the generalization method commonly used in privacy protection to publish anonymized data sets, giving it a demonstrable degree of protection 
    ([code](https://github.com/McGill-DMaS/DiffGen))


* ## 9. Overview and Tutorial

    * [Graham Cormode, Somesh Jha, Tejas Kulkarni, Ninghui Li, Divesh Srivastava, Tianhao Wang:  Privacy at Scale: Local Differential Privacy in Practice. SIGMOD Conference 2018: 1655-1658](http://dimacs.rutgers.edu/~graham/pubs/html/CormodeJhaKulkarniLiSrivastavaWang18.html)


    * [Tianqing Zhu, Gang Li, Wanlei Zhou, Philip S. Yu:   Differential Privacy and Applications. Advances in Information Security 69, Springer 2017, ISBN 978-3-319-62002-2, pp. 1-222  ](https://link.springer.com/book/10.1007%2F978-3-319-62004-6)



    * [Tianqing Zhu, Gang Li, Wanlei Zhou, Philip S. Yu:  Differentially Private Data Publishing and Analysis: A Survey. IEEE Trans. Knowl. Data Eng. 29(8): 1619-1638 (2017)](https://ieeexplore.ieee.org/document/7911185)


    * [Kamalika Chaudhuri, Anand D. Sarwate:  Differentially Private Machine Learning: Theory, Algorithms, and Applications, NIPS2017 Tutorial](https://www.ece.rutgers.edu/~asarwate/nips2017/)


    * [Ninghui Li, Min Lyu, Dong Su, Weining Yang:  Differential Privacy: From Theory to Practice. Synthesis Lectures on Information Security, Privacy, & Trust, Morgan & Claypool Publishers 2016, pp. 1-138](https://ieeexplore.ieee.org/document/7731575?bkn=7731575)

    * [Cynthia Dwork, Aaron Roth:  The Algorithmic Foundations of Differential Privacy. Foundations and Trends in Theoretical Computer Science 9(3-4): 211-407 (2014)](http://nowpublishers.com/article/DownloadSummary/TCS-042)

* ## 10. Others, Applications
    * [Differentially Private Semi-Supervised Learning With Known Class Priors](https://ieeexplore.ieee.org/document/8622071). (BigData 2018)
      > It presents a framework for semi-supervised learning, assuming known class priors, and provides the theoretical guarantee on the optimal risk. Under this setting, they give the differentially private learning on the framework. However, they make mistakes on addition of noise, which have been corrected in [[Kamalika Chaudhuri 2011](https://dl.acm.org/citation.cfm?id=2021036)].
    * [Semi-supervised Knowledge Transfer for Deep Learning from Private Training Data](https://openreview.net/forum?id=HkwoSDP). (ICLR 2017)
       > The paper presents a general teacher-student approach for differentially-private learning in which the student learns to predict a noise vote among a set of teachers. The noise allows the student to be differentially private, whilst maintaining good classification accuracies on MNIST and SVHN.  
       > It divides the dataset to some disjoint subsets and provide client-level dp, then use semi-supervised learning to utlize non-private unlabeled data and obtain a student model. Bscause aggregation is much easier to add noise than learning. Take notice of that this framework don't limit the teacher models and student model, which is different from ([Jihun Hamm ICML 2016](http://proceedings.mlr.press/v48/hamm16.html)).
    * [Differentially Private Semi-Supervised Classification](https://ieeexplore.ieee.org/document/7947001) (SMARTCOMP 2017)
       > For a specific SSL(tranductive k-NN learning), it considers privacy of labeled instances and proivdes differentially private protection.  
       > However, it ignores privacy of unlabeled instances and the setting(k-mutual neighbor) limits the effect of unlabeled instances.
    * [A Semi-Supervised Learning Approach to Differential Privacy](https://ieeexplore.ieee.org/document/6754008) (ICDM Workshops 2013)
       > It expends dp Random Decision Tree to utlize unlabeled data, but it only consider the privacy of labeled data. The unlabeled data is considered to be public and non-private. In general, it utlize unlabeled data as auxiliary information to boost performance of dp mechanism.

