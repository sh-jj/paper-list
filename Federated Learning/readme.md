# Papers

## Personalization 

Virginia Smith, Chao-Kai Chiang, Maziar Sanjabi, Ameet S. Talwalkar:  
Federated Multi-Task Learning. NIPS 2017: 4424-4434  
http://papers.nips.cc/paper/7029-federated-multi-task-learning
> This paper fit federated learning problem as multi-task learning and provide different models for each client. 
> A optimization method MOCHA for multi-task learning has been proposed to handle the chanllenges in federated setting.
> For each client, the contribution to global update depends on its progress on local tasks. 
> As a result, the update from unstable and out-of-distribution could be limited.

Valentina Zantedeschi, Aurélien Bellet, Marc Tommasi  
Fully Decentralized Joint Learning of Personalized Models and Collaboration Graphs. [Research Report] Inria. 2019. ffhal-02166433f  
https://hal.inria.fr/hal-02166433/
> This paper builds a connection between graph regularization in multi-task learning and communication graph in federated learning.
> Local models and relation graph are obtained by iterative optimization.

Yihan Jiang, Jakub Konecný, Keith Rush, Sreeram Kannan:  
Improving Federated Learning Personalization via Model Agnostic Meta Learning. CoRR abs/1909.12488 (2019)  
https://arxiv.org/abs/1909.12488
> This paper builds a connection between meta-learning (MAML) and federated learning, that meta-training in MAML corresponds to global update in federated learning. It adapts to the federated learning setting through fast adaptation ability by limited data.  
> Defect: Meta-learning "sounds like" a solution to federated learning. However, how to deal with system challenges is still a problem.
The contribution of this paper is limited.

## Aggregation

Mehryar Mohri, Gary Sivek, Ananda Theertha Suresh:  
Agnostic Federated Learning. ICML 2019: 4615-4625  
http://proceedings.mlr.press/v97/mohri19a.html  
> This paper argues that uniform solution commonly adopted in federated learning may not provide a satisfactory performance, because meaningful data may be concentrated in a small number of nodes (Pareto's law).  
> Agnostic FL means that the target distribution is agnostic. And this paper fomulates it as min-max game. The target distribution is defined as a convex combination of multiple sources where the model performs the worst.

[Bayesian Nonparametric Federated Learning of Neural Networks.](https://arxiv.org/abs/1905.12022) (ICML 2019)
   
[Federated Learning with Matched Averaging.](https://arxiv.org/abs/2002.06440) (ICLR 2020)

## System Robustness
Dong Yin, Yudong Chen, Kannan Ramchandran, Peter Bartlett:  
Byzantine-Robust Distributed Learning: Towards Optimal Statistical Rates. ICML 2018: 5636-5645  
https://arxiv.org/abs/1803.01498  
> Byzantine failure in distributed learning: means that some worker machines may behave completely arbitrarily and can send any message to the master machine. They provided two method: median-based GD and trimmed-mean-based GD, that achieve optimal statistical rates.

Jiashi Feng, Huan Xu, Shie Mannor:  
Distributed Robust Learning. CoRR abs/1409.5937 (2014)  
https://arxiv.org/pdf/1409.5937.pdf  
> For distributed learning of linear model, choose the geometric median of local learned model.

## Transfer
[Federated Adversarial Domain Adaptation.](https://arxiv.org/abs/1911.02054) (ICLR 2020)

## Survey

Peter Kairouz, H. Brendan McMahan, Brendan Avent, Aurélien Bellet, Mehdi Bennis, Arjun Nitin Bhagoji, Keith Bonawitz, Zachary Charles, Graham Cormode, Rachel Cummings, Rafael G. L. D'Oliveira, Salim El Rouayheb, David Evans, Josh Gardner, Zachary Garrett, Adrià Gascón, Badih Ghazi, Phillip B. Gibbons, Marco Gruteser, Zaïd Harchaoui, Chaoyang He, Lie He, Zhouyuan Huo, Ben Hutchinson, Justin Hsu, Martin Jaggi, Tara Javidi, Gauri Joshi, Mikhail Khodak, Jakub Konecný, Aleksandra Korolova, Farinaz Koushanfar, Sanmi Koyejo, Tancrède Lepoint, Yang Liu, Prateek Mittal, Mehryar Mohri, Richard Nock, Ayfer Özgür, Rasmus Pagh, Mariana Raykova, Hang Qi, Daniel Ramage, Ramesh Raskar, Dawn Song, Weikang Song, Sebastian U. Stich, Ziteng Sun, Ananda Theertha Suresh, Florian Tramèr, Praneeth Vepakomma, Jianyu Wang, Li Xiong, Zheng Xu, Qiang Yang, Felix X. Yu, Han Yu, Sen Zhao:  
Advances and Open Problems in Federated Learning. CoRR abs/1912.04977 (2019)  
https://arxiv.org/abs/1912.04977

Kevin Hsieh, Amar Phanishayee, Onur Mutlu, Phillip B. Gibbons:  
The Non-IID Data Quagmire of Decentralized Machine Learning. CoRR abs/1910.00189 (2019)  
https://arxiv.org/pdf/1910.00189.pdf  

# Authors

## Google

Mehryar Mohri  
https://cs.nyu.edu/~mohri/  

H. Brendan McMahan  
https://research.google/people/author35837/  

Jakub Konečný  
http://jakubkonecny.com/

## CMU
Virginia Smith  
https://www.cs.cmu.edu/~smithv/

## Others
Ji Liu (Kwai Inc.)  
http://jiliu-ml.org/  


