# Awesome DRL Cloud Scheduling

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of *Deep Reinforcement Learning (DRL)* research and related works on:

- **Resource scheduling / placement** in cloud environments
- **Service autoscaling** (microservice scaling-in / scaling-out)
- **Cloud-level scheduling decisions** involving task placement and resource allocation

---

## Contents

- [Introduction](#introduction)
- [Research Papers](#research-papers)
  - [DRL — Resource Scheduling](#drl--resource-scheduling)
  - [DRL — Autoscaling](#drl--autoscaling)
  - [DRL — Edge Computing](#drl--edge-computing)
  - [DRL — Robustness & Security](#drl--robustness--security)
- [Beyond DRL](#beyond-drl)
  - [Beyond DRL — Benchmarks & Simulators](#beyond-drl--benchmarks--simulators)
  - [Beyond DRL — Heuristic & Evolutionary Scheduling](#beyond-drl--heuristic--evolutionary-scheduling)
  - [Beyond DRL — ML Predictive Autoscaling](#beyond-drl--ml-predictive-autoscaling)
  - [Beyond DRL — Microservice Architecture & Analysis](#beyond-drl--microservice-architecture--analysis)
  - [Beyond DRL — Other](#beyond-drl--other)
  - [Beyond DRL — Surveys & Reviews](#beyond-drl--surveys--reviews)
  - [Beyond DRL — System Design & Platform](#beyond-drl--system-design--platform)
  - [Beyond DRL — Traditional Autoscaling](#beyond-drl--traditional-autoscaling)
  - [Beyond DRL — Traditional Resource Management](#beyond-drl--traditional-resource-management)
  - [Beyond DRL — Workload Analysis & Characterization](#beyond-drl--workload-analysis--characterization)
- [Datasets](#datasets)
- [Contributing](#contributing)
- [References](#references)
- [License](#license)

---

## Introduction

With the increasing complexity of cloud environments and the dynamic nature of workloads, traditional scheduling algorithms often fall short in optimizing resource allocation. Deep Reinforcement Learning (DRL) offers a promising approach by learning optimal scheduling policies through environment interaction.

This repository collects significant works that leverage DRL for cloud scheduling and autoscaling, as well as related research in machine learning, heuristics, workload analysis, and system design.

---

## Research Papers

### DRL — Resource Scheduling

- **[DDQN-TS: A novel bi-objective intelligent scheduling algorithm in the cloud environment](https://scholar.google.com/scholar?q=DDQN-TS%3A%2BA%2Bnovel%2Bbi-objective%2Bintelligent%2Bscheduling)**
  *Authors*: Zhao Tong, Feng Ye, Bilan Liu, Jinhui Cai, Jing Mei
  *Publication*: Neurocomputing-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[SLAs-Aware Online Task Scheduling Based on Deep Reinforcement Learning Method in Cloud Environment](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Longyu Ran, Xiaoyu Shi, Mingsheng Shang
  *Publication*: HPCC-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep reinforcement learning-based methods for resource scheduling in cloud computing: a review and future directions](https://arxiv.org/)**
  *Authors*: Guangyao Zhou, Wenhong Tian, Rajkumar Buyya, Ruini Xue, Liang Song
  *Publication*: arXiv-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Resource Management with Deep Reinforcement Learning](https://dl.acm.org/doi/10.1145/3013727.3013736)**
  *Authors*: Hongzi Mao, Mohammad Alizadeh, Ishai Menache, Srikanth Kandula
  *Publication*: HotNets-2016
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[RLQ: Workload Allocation With Reinforcement Learning in Distributed Queues](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Alessandro Staffolani, Victor-Alexandru Darvariu, Paolo Bellavista, Mirco Musolesi
  *Publication*: TPDS-2023
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Model-free control for distributed stream data processing using deep reinforcement learning](https://www.vldb.org/)**
  *Authors*: Teng Li, Zhiyuan Xu, Jian Tang, Yanzhi Wang
  *Publication*: VLDB-2018
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Model-free control for distributed stream data processing using deep reinforcement learning](https://www.vldb.org/)**
  *Authors*: Teng Li, Zhiyuan Xu, Jian Tang, Yanzhi Wang
  *Publication*: VLDB-2018
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Performance and Cost-Efficient Spark Job Scheduling Based on Deep Reinforcement Learning in Cloud Computing Environments](https://ieeexplore.ieee.org/document/9354797)**
  *Authors*: Muhammed Tawfiqul Islam, Shanika Karunasekera, Rajkumar Buyya
  *Publication*: TPDS-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Cloud Resource Scheduling With Deep Reinforcement Learning and Imitation Learning](https://scholar.google.com/scholar?q=Cloud%2BResource%2BScheduling%2BWith%2BDeep%2BReinforcement)**
  *Authors*: Wenxia Guo, Wenhong Tian, Yufei Ye, Lingxiao Xu, Kui Wu
  *Publication*: IOTJ-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Toward a Reinforcement Learning Environment Toolbox for Intelligent Electric Motor Control](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=5962385)**
  *Authors*: Arne Traue, Gerrit Book, Wilhelm Kirchgassner, Oliver Wallscheid
  *Publication*: TNNLS-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Efficient Compute-Intensive Job Allocation in Data Centers via Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/8979737)**
  *Authors*: Deliang Yi, Xin Zhou, Yonggang Wen, Rui Tan
  *Publication*: TPDS-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Dynamic Job Shop Scheduling via Deep Reinforcement Learning](https://proceedings.neurips.cc/)**
  *Authors*: Xinjie Liang, Wen Song, Pengfei Wei
  *Publication*: NeurIPS-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[DRAS: Deep Reinforcement Learning for Cluster Scheduling in High Performance Computing](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Yuping Fan, Boyang Li, Dustin Favorite, Naunidh Singh, Taylor Childers, Paul Rich, William Allcock, Michael E. Papka, Zhiling Lan
  *Publication*: TPDS-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[RLScheduler: An Automated HPC Batch Job Scheduler Using Reinforcement Learning](https://dl.acm.org/conference/sc)**
  *Authors*: Di Zhang, Dong Dai, Youbiao He, Forrest Sheng Bao, Bing Xie
  *Publication*: SC-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Optimizing Job Scheduling using Deep Reinforcement Learning](https://dl.acm.org/conference/hpdc)**
  *Authors*: Rohit Sigar, Avadh Kishor, Pramod Kumar Singh, Joydip Dhar
  *Publication*: HPDC-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[ADRL: A Hybrid Anomaly-Aware Deep Reinforcement Learning-Based Resource Scaling in Clouds](https://ieeexplore.ieee.org/document/9384482)**
  *Authors*: Sara Kardani-Moghaddam, Rajkumar Buyya, Kotagiri Ramamohanarao
  *Publication*: TPDS-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Multi-Dimensional Resource Allocation in Distributed Data Centers Using Deep Reinforcement Learning](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=4234)**
  *Authors*: Wenting Wei, Huaxi Gu, Kun Wang, Jianjia Li, Xuan Zhang, Ning Wang
  *Publication*: TNSM-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning Based Adaptive Operator Selection for Evolutionary Multi-Objective Optimization](https://scholar.google.com/scholar?q=Deep%2BReinforcement%2BLearning%2BBased%2BAdaptive%2BOperator)**
  *Authors*: Ye Tian, Xiaopeng Li, Haiping Ma, Xingyi Zhang, Kay Chen Tan, Yaochu Jin
  *Publication*: TETCI-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[DRL-cloud: Deep reinforcement learning-based resource provisioning and task scheduling for cloud service providers](https://ieeexplore.ieee.org/document/8297294)**
  *Authors*: Mingxi Cheng, Ji Li, Shahin Nazarian
  *Publication*: ASP-DAC-2018
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[DRL-cloud: Deep reinforcement learning-based resource provisioning and task scheduling for cloud service providers](https://ieeexplore.ieee.org/document/8297294)**
  *Authors*: Mingxi Cheng, Ji Li, Shahin Nazarian
  *Publication*: ASP-DAC-2018
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Adaptive and Efficient Resource Allocation in Cloud Datacenters Using Actor-Critic Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9634581)**
  *Authors*: Zheyi Chen, Jia Hu, Geyong Min, Chunbo Luo, Tarek El-Ghazawi
  *Publication*: TPDS-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Scheduling of Time-Varying Workloads Using Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/17673)**
  *Authors*: Shanka Subhra Mondal, Nikhil Sheoran, Subrata Mitra
  *Publication*: AAAI-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning Enhanced Greedy Algorithm for Online Scheduling of Batched Tasks in Cloud in Cloud HPC Systems](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Yuanhao Yang, Hong Shen
  *Publication*: TPDS-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A heuristic multi-objective task scheduling framework for container-based clouds via actor-critic reinforcement learning](https://scholar.google.com/scholar?q=A%2Bheuristic%2Bmulti-objective%2Btask%2Bscheduling%2Bframework)**
  *Authors*: Lilu Zhu, Feng Wu, Yanfeng Hu, Kai Huang, Xinmei Tian
  *Publication*: 2023
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Integrated and Fungible Scheduling of Deep Learning Workloads Using Multi-Agent Reinforcement Learning](https://scholar.google.com/scholar?q=Integrated%2Band%2BFungible%2BScheduling%2Bof%2BDeep)**
  *Authors*: Jialun Li, Danyang Xiao, Diying Yang, Xuan Mo, Weigang Wu
  *Publication*: 2025
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Millimeter Wave Communications With an Intelligent Reflector: Performance Optimization and Distributional Reinforcement Learning](https://scholar.google.com/scholar?q=Millimeter%2BWave%2BCommunications%2BWith%2Ban%2BIntelligent)**
  *Authors*: Qianqian Zhang, Walid Saad, Mehdi Bennis
  *Publication*: 2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[READYS: A Reinforcement Learning Based Strategy for Heterogeneous Dynamic Scheduling](https://ieeexplore.ieee.org/xpl/conhome/1000057/all-proceedings)**
  *Authors*: Nathan Grinsztajn, Olivier Beaumont, Emmanuel Jeannot, Philippe Preux
  *Publication*: CLUSTER-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A multi-objective trade-off framework for cloud resource scheduling based on the Deep Q-network algorithm](https://link.springer.com/article/10.1007/s10586-022-03561-9)**
  *Authors*: Zhiping Peng, Jianpeng Lin, Delong Cui, Qirui Li, Jieguang He
  *Publication*: Cluster Computing-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Cost-aware job scheduling for cloud instances using deep reinforcement learning](https://link.springer.com/article/10.1007/s10586-022-03577-1)**
  *Authors*: Feng Cheng, Yifeng Huang, Bhavana Tanpure, Pawan Sawalani, Long Cheng, Cong Liu
  *Publication*: Cluster Computing-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Energy-Efficient Task Scheduling in Data Centers Using Adaptive Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Energy-Efficient%2BTask%2BScheduling%2Bin%2BData%2BCenters)**
  *Authors*: Dinuț Ionuț-Cosmin, Bogdan Alexandrescu, Rodica-Claudia Constantinescu
  *Publication*: Code-2025
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Task Scheduling in Cloud Using Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Task%2BScheduling%2Bin%2BCloud%2BUsing%2BDeep)**
  *Authors*: Shashank Swarup, Elhadi M. Shakshuki, Ansar Yasar
  *Publication*: Code-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[GARLSched: Generative adversarial deep reinforcement learning task scheduling optimization for large-scale high performance computing systems](https://www.sciencedirect.com/science/article/pii/S0167739X22001617)**
  *Authors*: Jingbo Li, Xingjun Zhang, Jia Wei, Zeyu Ji, Zheng Wei
  *Publication*: FGCS-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Distributional Reinforcement Learning for mmWave Communications with Intelligent Reflectors on a UAV](https://ieeexplore.ieee.org/xpl/conhome/1000103/all-proceedings)**
  *Authors*: Qianqian Zhang, Walid Saad, Mehdi Bennis
  *Publication*: GLOBECOM-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[RLSK: A Job Scheduler for Federated Kubernetes Clusters based on Reinforcement Learning](https://ieeexplore.ieee.org/document/9162808)**
  *Authors*: Jiaming Huang, Chuming Xiao, Weigang Wu
  *Publication*: IC2E-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning Based Mobility Load Balancing Under Multiple Behavior Policies](https://ieeexplore.ieee.org/xpl/conhome/1000102/all-proceedings)**
  *Authors*: Yue Xu, Wenjun Xu, Zhi Wang, Jiaru Lin, Shuguang Cui
  *Publication*: ICC-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning based Compute-Intensive Workload Allocation in Data Centers with High Energy Efficiency](https://ieeexplore.ieee.org/xpl/conhome/1000101/all-proceedings)**
  *Authors*: Zhenfeng Gao, Wei Liu, Long Suo, Jiandong Li, Yijun Lu
  *Publication*: ICCC-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Actor-Critic with Transformer for Cloud Computing Resource Three Stage Job Scheduling](https://scholar.google.com/scholar?q=Actor-Critic%2Bwith%2BTransformer%2Bfor%2BCloud%2BComputing)**
  *Authors*: Yanbo Xu, Jiakun Zhao
  *Publication*: ICCCBDA-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Minerva: A reinforcement learning-based technique for optimal scheduling and bottleneck detection in distributed factory operations](https://ieeexplore.ieee.org/xpl/conhome/1000156/all-proceedings)**
  *Authors*: Tara Elizabeth Thomas, Jinkyu Koo, Somali Chaterji, Saurabh Bagchi
  *Publication*: ICCSN-2018
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep reinforcement learning-aided multi-step job scheduling in optical data center networks](https://scholar.google.com/scholar?q=Deep%2Breinforcement%2Blearning-aided%2Bmulti-step%2Bjob%2Bscheduling)**
  *Authors*: Che-Yu Liu, Xiaoliang Chen, Roberto Proietti, Zuqing Zhu, S. J. Ben Yoo
  *Publication*: ICDBC-2025
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A Hierarchical Framework of Cloud Resource Allocation and Power Management Using Deep Reinforcement Learning](https://ieeexplore.ieee.org/xpl/conhome/1000050/all-proceedings)**
  *Authors*: Ning Liu, Zhe Li, Jielong Xu, Zhiyuan Xu, Sheng Lin, Qinru Qiu, Jian Tang, Yanzhi Wang
  *Publication*: ICDCS-2017
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Toward Efficient Compute-Intensive Job Allocation for Green Data Centers: A Deep Reinforcement Learning Approach](https://ieeexplore.ieee.org/xpl/conhome/1000050/all-proceedings)**
  *Authors*: Deliang Yi, Xin Zhou, Yonggang Wen, Rui Tan
  *Publication*: ICDCS-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[DeepEE: Joint Optimization of Job Scheduling and Cooling Control for Data Center Energy Efficiency Using Deep Reinforcement Learning](https://ieeexplore.ieee.org/xpl/conhome/1000050/all-proceedings)**
  *Authors*: Yongyi Ran, Han Hu, Xin Zhou, Yonggang Wen
  *Publication*: ICDCS-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Spear: Optimized Dependency-Aware Task Scheduling with Deep Reinforcement Learning](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Zhiming Hu, James Tu, Baochun Li
  *Publication*: ICDCS-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Heterogeneous-Aware Online Cloud Task Scheduler Based on Clustering and Deep Reinforcement Learning Ensemble](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Dan Gu, Jing Chen, Xiaoyu Shi, Longyu Ran, Ying Zhang, Mingsheng Shang
  *Publication*: ICNC-FSKD-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning for Multi-resource Cloud Job Scheduling](https://scholar.google.com/scholar?q=Deep%2BReinforcement%2BLearning%2Bfor%2BMulti-resource%2BCloud)**
  *Authors*: Jianpeng Lin, Zhiping Peng, Delong Cui
  *Publication*: ICNP-2017
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A Multi-Graph Attributed Reinforcement Learning based Optimization Algorithm for Large-scale Hybrid Flow Shop Scheduling Problem](https://dl.acm.org/conference/kdd)**
  *Authors*: Fei Ni, Jianye Hao, Jiawen Lu, Xialiang Tong, Mingxuan Yuan, Jiahui Duan, Yi Ma, Kun He
  *Publication*: KDD-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A Dual-Agent Scheduler for Distributed Deep Learning Jobs on Public Cloud via Reinforcement Learning](https://dl.acm.org/doi/10.1145/3580305.3599371)**
  *Authors*: Mingzhe Xing, Hangyu Mao, Shenglin Yin, Lichen Pan, Zhengchao Zhang, Zhen Xiao, Jieyi Long
  *Publication*: KDD-2023
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A Dynamic Resource Allocation Strategy with Reinforcement Learning for Multimodal Multi-objective Optimization](https://link.springer.com/journal/11042)**
  *Authors*: Qian-Long Dang, Wei Xu, Yang-Fei Yuan
  *Publication*: MIR-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Data Centers Job Scheduling with Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Data%2BCenters%2BJob%2BScheduling%2Bwith%2BDeep)**
  *Authors*: Sisheng Liang, Zhou Yang, Fang Jin, Yong Chen
  *Publication*: PAKDD-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning for Dynamic Workflow Scheduling in Cloud Environment](https://ieeexplore.ieee.org/xpl/conhome/1000062/all-proceedings)**
  *Authors*: Tingting Dong, Fei Xue, Changbai Xiao, Jiangjiang Zhang
  *Publication*: SCC-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Microscaler: Automatic Scaling for Microservices with an Online Learning Approach](https://ieeexplore.ieee.org/document/8835244)**
  *Authors*: Guangba Yu, Pengfei Chen, Zibin Zheng
  *Publication*: ICWS-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[<i>Microscaler</i>: Cost-Effective Scaling for Microservice Applications in the Cloud With an Online Learning Approach](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=8918)**
  *Authors*: Guangba Yu, Pengfei Chen, Zibin Zheng
  *Publication*: TCC-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[SIMPPO A Scalable and Incremental Online Learning Framework for Serverless Resource Management](https://dl.acm.org/conference/socc)**
  *Authors*: SIMPPO A Scalable and
  *Publication*: SoCC-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[SibylOpt: Managing Green Data Centers Using Off-Online Deep Reinforcement Learning](https://dl.acm.org/conference/socc)**
  *Authors*: Ning Gu, Kuo Zhang, Thu Nguyen, Peijian Wang, Tania Lorido Botran
  *Publication*: SoCC-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[gym-hpa: Efficient Auto-Scaling via Reinforcement Learning for Complex Microservice-based Applications in Kubernetes](https://ieeexplore.ieee.org/document/10145462)**
  *Authors*: José Santos, Tim Wauters, Bruno Volckaert, Filip De Turck
  *Publication*: NOMS-2023
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A-SARSA: A Predictive Container Auto-Scaling Algorithm Based on Reinforcement Learning](https://ieeexplore.ieee.org/document/9277342)**
  *Authors*: Shubo Zhang, Tianyang Wu, Maolin Pan, Chaomeng Zhang, Yang Yu
  *Publication*: ICWS-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning: A Survey](https://scholar.google.com/scholar?q=Deep%2BReinforcement%2BLearning%3A%2BA%2BSurvey)**
  *Authors*: Xu Wang, Sen Wang, Xingxing Liang, Dawei Zhao, Jincai Huang, Xin Xu, Bin Dai, Qiguang Miao
  *Publication*: 2024
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

---
### DRL — Autoscaling

- **[Fast and Fine-grained Autoscaler for Streaming Jobs with Reinforcement Learning](https://www.ijcai.org/proceedings/2022/531)**
  *Authors*: Mingzhe Xing, Hangyu Mao, Zhen Xiao
  *Publication*: IJCAI-2022
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[A Meta Reinforcement Learning Approach for Predictive Autoscaling in the Cloud](https://dl.acm.org/conference/kdd)**
  *Authors*: Siqiao Xue, Chao Qu, Xiaoming Shi, Cong Liao, Shiyi Zhu, Xiaoyu Tan, Lintao Ma, Shiyu Wang, Shijun Wang, Yun Hu
  *Publication*: KDD-2022
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[Reinforcement learning-based application Autoscaling in the Cloud: A survey](https://scholar.google.com/scholar?q=Reinforcement%2Blearning-based%2Bapplication%2BAutoscaling%2Bin%2Bthe)**
  *Authors*: Yisel Garí, David A. Monge, Elina Pacini, Cristian Mateos, Carlos García Garino
  *Publication*: ENG APPL ARTIF INTEL-2021
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[Reinforcement learning-assisted autoscaling mechanisms for serverless computing platforms](https://scholar.google.com/scholar?q=Reinforcement%2Blearning-assisted%2Bautoscaling%2Bmechanisms%2Bfor%2Bserverless)**
  *Authors*: Anastasios Zafeiropoulos, Eleni Fotopoulou, Nikos Filinis, Symeon Papavassiliou
  *Publication*: SMPT-2022
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[DScaler: A Horizontal Autoscaler of Microservice Based on Deep Reinforcement Learning](https://ieeexplore.ieee.org/xpl/conhome/1000119/all-proceedings)**
  *Authors*: Zhijiao Xiao, Song Hu
  *Publication*: APNOMS-2022
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[AWARE Automate Workload Autoscaling with Reinforcement Learning in Production Cloud Systems](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Haoran Qiu, Weichao Mao
  *Publication*: ATC-2023
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[Intelligent microservices autoscaling module using reinforcement learning](https://scholar.google.com/scholar?q=Intelligent%2Bmicroservices%2Bautoscaling%2Bmodule%2Busing%2Breinforcement)**
  *Authors*: Abeer Abdel Khaleq, Ilkyeun Ra
  *Publication*: CC-2023
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

---
### DRL — Edge Computing

- **[Deep Reinforcement Learning for Load-Balancing Aware Network Control in IoT Edge Systems](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Qingzhi Liu, Tiancong Xia, Long Cheng, Merijn van Eijk, Tanir Ozcelebi, Ying Mao
  *Publication*: TPDS-2022
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Dynamic Scheduling for Stochastic Edge-Cloud Computing Environments Using A3C Learning and Residual Recurrent Neural Networks](https://ieeexplore.ieee.org/document/9047484)**
  *Authors*: Shreshth Tuli, Shashikant Ilager, Kotagiri Ramamohanarao, Rajkumar Buyya
  *Publication*: TMC-2020
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Energy Efficient Task Scheduling in Fog Environment using Deep Reinforcement Learning Approach](https://scholar.google.com/scholar?q=Energy%2BEfficient%2BTask%2BScheduling%2Bin%2BFog)**
  *Authors*: Shashank Swarup, Elhadi M. Shakshuki, Ansar Yasar
  *Publication*: 2021
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Optimization of lightweight task offloading strategy for mobile edge computing based on deep reinforcement learning](https://www.sciencedirect.com/science/article/pii/S0167739X19323840)**
  *Authors*: Haifeng Lu, Chunhua Gu, Fei Luo, Weichao Ding, Xinping Liu
  *Publication*: FGCS-2020
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Neural Task Scheduling with Reinforcement Learning for Fog Computing Systems](https://ieeexplore.ieee.org/xpl/conhome/1000103/all-proceedings)**
  *Authors*: Simeng Bian, Xi Huang, Ziyu Shao, Yang Yang
  *Publication*: GLOBECOM-2019
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Deep Reinforcement Learning-Based Workload Scheduling for Edge Computing](https://link.springer.com/article/10.1007/s10586-022-03625-x)**
  *Authors*: Tao Zheng, Jian Wan, Jilin Zhang, Congfeng Jiang
  *Publication*: JCCASA-2022
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[A Deep Reinforcement Learning Approach to Multi-Component Job Scheduling in Edge Computing](https://scholar.google.com/scholar?q=A%2BDeep%2BReinforcement%2BLearning%2BApproach%2Bto)**
  *Authors*: Zhi Cao, Honggang Zhang, Yu Cao, Benyuan Liu
  *Publication*: MSN-2019
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[A Deep Reinforcement Learning Approach to Online Microservice Deployment in Mobile Edge Computing](https://scholar.google.com/scholar?q=A%2BDeep%2BReinforcement%2BLearning%2BApproach%2Bto)**
  *Authors*: Yuqi Zhao, Jian Wang, Bing Li
  *Publication*: ICSOC-2023
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

---
### DRL — Robustness & Security

- **[Adversarial Attacks in a Deep Reinforcement Learning based Cluster Scheduler](https://scholar.google.com/scholar?q=Adversarial%2BAttacks%2Bin%2Ba%2BDeep%2BReinforcement)**
  *Authors*: Shaojun Zhang, Chen Wang, Albert Y. Zomaya
  *Publication*: 2020
  *Summary*: This paper investigates the robustness and security of deep reinforcement learning-based schedulers in cloud environments. The study identifies vulnerabilities to adversarial attacks and proposes defense mechanisms to enhance scheduler stability. The work provides insights into the reliability of DRL schedulers under varying conditions.
  **Code**: Not available

- **[Robustness Analysis and Enhancement of Deep Reinforcement Learning-Based Schedulers](https://scholar.google.com/scholar?q=Robustness%2BAnalysis%2Band%2BEnhancement%2Bof%2BDeep)**
  *Authors*: Shaojun Zhang, Chen Wang, Albert Y. Zomaya
  *Publication*: 2023
  *Summary*: This paper investigates the robustness and security of deep reinforcement learning-based schedulers in cloud environments. The study identifies vulnerabilities to adversarial attacks and proposes defense mechanisms to enhance scheduler stability. The work provides insights into the reliability of DRL schedulers under varying conditions.
  **Code**: Not available

---

## Beyond DRL

*Papers that use other methods (ML prediction, evolutionary algorithms, system design, etc.) but are relevant to cloud scheduling and autoscaling.*

### Beyond DRL — Benchmarks & Simulators

- **[GloudSim: Google trace based cloud simulator with virtual machines](https://scholar.google.com/scholar?q=GloudSim%3A%2BGoogle%2Btrace%2Bbased%2Bcloud%2Bsimulator)**
  *Authors*: Sheng Di, Franck Cappello
  *Publication*: 2015
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[BigDataBench: A big data benchmark suite from internet services](https://ieeexplore.ieee.org/xpl/conhome/1000056/all-proceedings)**
  *Authors*: Lei Wang, Jianfeng Zhan, Chunjie Luo, Yuqing Zhu, Qiang Yang, Yongqiang He, Wanling Gao, Zhen Jia, Yingjie Shi, Shujie Zhang
  *Publication*: HPCA-2014
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[BigDataBench-S: An Open-Source Scientific Big Data Benchmark Suite](https://ieeexplore.ieee.org/xpl/conhome/1000059/all-proceedings)**
  *Authors*: Xinhui Tian, Shaopeng Dai, Zhihui Du, Wanling Gao, Rui Ren, Yaodong Cheng, Zhifei Zhang, Zhen Jia, Peijian Wang, Jianfeng Zhan
  *Publication*: IPDPSW-2017
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[An Open-Source Benchmark Suite for Microservices and Their Hardware-Software Implications for Cloud &amp; Edge Systems](https://dl.acm.org/conference/asplos)**
  *Authors*: Yu Gan, Yanqi Zhang, Dailun Cheng, Ankitha Shetty, Priyal Rathi, Nayan Katarki, Ariana Bruno, Justin Hu, Brian Ritchken, Brendon Jackson
  *Publication*: ASPLOS-2019
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[Benchmarking microservice systems for software engineering research](https://scholar.google.com/scholar?q=Benchmarking%2Bmicroservice%2Bsystems%2Bfor%2Bsoftware%2Bengineering)**
  *Authors*: Xiang Zhou, Xin Peng, Tao Xie, Jun Sun, Chenjie Xu, Chao Ji, Wenyun Zhao
  *Publication*: ICSE-2018
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[μBench: An Open-Source Factory of Benchmark Microservice Applications](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Andrea Detti, Ludovico Funari, Luca Petrucci
  *Publication*: TPDS-2021
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[PerfSim: A Performance Simulator for Cloud Native Microservice Chains](https://scholar.google.com/scholar?q=PerfSim%3A%2BA%2BPerformance%2BSimulator%2Bfor%2BCloud)**
  *Authors*: Michel Gokan Khan, Javid Taheri, Auday Al-Dulaimy, Andreas Kassler
  *Publication*: 2023
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[PerfSim: A Performance Simulator for Cloud Native Microservice Chains](https://arxiv.org/)**
  *Authors*: Michel Gokan Khan, Javid Taheri, Auday Al-Dulaimy, Andreas Kassler
  *Publication*: arXiv-2021
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available


### Beyond DRL — Heuristic & Evolutionary Scheduling

- **[Neural network based multi-objective evolutionary algorithm for dynamic workflow scheduling in cloud computing](https://www.sciencedirect.com/journal/future-generation-computer-systems)**
  *Authors*: Goshgar Ismayilov, Haluk Rahmi Topcuoglu
  *Publication*: FGCS-2020
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Combining Size-Based Load Balancing with Round-Robin for Scalable Low Latency](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Jonatha Anselmi
  *Publication*: TPDS-2020
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[DDMTS: A novel dynamic load balancing scheduling scheme under SLA constraints in cloud computing](https://scholar.google.com/scholar?q=DDMTS%3A%2BA%2Bnovel%2Bdynamic%2Bload%2Bbalancing)**
  *Authors*: Zhao Tong, Xiaomei Deng, Hongjian Chen, Jing Mei
  *Publication*: JPDC-2021
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Hybridization of firefly and Improved Multi-Objective Particle Swarm Optimization algorithm for energy efficient load balancing in Cloud Computing environments](https://scholar.google.com/scholar?q=Hybridization%2Bof%2Bfirefly%2Band%2BImproved%2BMulti-Objective)**
  *Authors*: A. Francis Saviour Devaraj, Mohamed Elhoseny, S. Dhanasekaran, E. Laxmi Lydia, K. Shankar
  *Publication*: JPDC-2020
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Mobility-Aware Computation Offloading with Adaptive Load Balancing in Small-Cell MEC](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Feng Lyu, Zhe Dong, Huaqing Wu, Sijing Duan, Fan Wu, Yaoxue Zhang, Xuemin Sherman Shen
  *Publication*: ICC-2022
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[A discrete PSO-based static load balancing algorithm for distributed simulations in a cloud environment](https://www.sciencedirect.com/journal/future-generation-computer-systems)**
  *Authors*: Zhang Miao, Peng Yong, Yang Mei, Yin Quanjun, Xie Xu
  *Publication*: FGCS-2021
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Multi-objective scheduling strategy for scientific workflows in cloud environment: A Firefly-based approach](https://scholar.google.com/scholar?q=Multi-objective%2Bscheduling%2Bstrategy%2Bfor%2Bscientific%2Bworkflows)**
  *Authors*: Mainak Adhikari, Tarachand Amgoth, Satish Narayana Srirama
  *Publication*: AppSoftCom-2019
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Reliability-Aware Multi-Objective Memetic Algorithm for Workflow Scheduling Problem in Multi-Cloud System](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Shuo Qin, Dechang Pi, Zhongshi Shao, Yue Xu, Yang Chen
  *Publication*: TPDS-2023
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[A Cooperative Coevolution Genetic Programming Hyper-Heuristics Approach for On-Line Resource Allocation in Container-Based Clouds](https://scholar.google.com/scholar?q=A%2BCooperative%2BCoevolution%2BGenetic%2BProgramming%2BHyper-Heuristics)**
  *Authors*: Boxiong Tan, Hui Ma, Yi Mei, Mengjie Zhang
  *Publication*: 2022
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Research and Improvement of Dynamic Highly Available Load Balancing Algorithm for Microservices](https://scholar.google.com/scholar?q=Research%2Band%2BImprovement%2Bof%2BDynamic%2BHighly)**
  *Authors*: Jianting Li, Guohong Yi, Bingqian Wu, Zhicao Cao, Xiaodong Xu
  *Publication*: 2022
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Resource scheduling algorithm with load balancing for cloud service provisioning](https://scholar.google.com/scholar?q=Resource%2Bscheduling%2Balgorithm%2Bwith%2Bload%2Bbalancing)**
  *Authors*: V. Priya, C. Sathiya Kumar, Ramani Kannan
  *Publication*: AppSoftCom-2019
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Multi objective task scheduling algorithm in cloud computing using grey wolf optimization](https://link.springer.com/journal/10586)**
  *Authors*: Sudheer Mangalampalli, Ganesh Reddy Karri, Mohit Kumar
  *Publication*: Cluster Computing-2022
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[A multi-objective load balancing algorithm for virtual machine placement in cloud data centers based on machine learning](https://link.springer.com/journal/607)**
  *Authors*: Arezoo Ghasemi, Abolfazl Toroghi Haghighat
  *Publication*: Computing-2020
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Load balancing in cloud computing – A hierarchical taxonomical classification](https://scholar.google.com/scholar?q=Load%2Bbalancing%2Bin%2Bcloud%2Bcomputing%2B%E2%80%93)**
  *Authors*: Shahbaz Afzal, G. Kavitha
  *Publication*: JCCASA-2019
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available


### Beyond DRL — ML Predictive Autoscaling

- **[Predictive Job Scheduling under Uncertain Constraints in Cloud Computing](https://ojs.aaai.org/)**
  *Authors*: Hang Dong, Boshi Wang, Bo Qiao, Wenqian Xing, Chuan Luo, Si Qin, Qingwei Lin, Dongmei Zhang, Gurpreet Virdi, Thomas Moscibroda
  *Publication*: AAAI-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Perph: A Workload Co-location Agent with Online Performance Prediction and Resource Inference](https://ieeexplore.ieee.org/xpl/conhome/1000075/all-proceedings)**
  *Authors*: Jianyong Zhu, Renyu Yang, Chunming Hu, Tianyu Wo, Shiqing Xue, Jin Ouyang, Jie Xu
  *Publication*: CCGrid-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[K-AGRUED: A Container Autoscaling Technique for Cloud-based Web Applications in Kubernetes Using Attention-based GRU Encoder-Decoder](https://scholar.google.com/scholar?q=K-AGRUED%3A%2BA%2BContainer%2BAutoscaling%2BTechnique%2Bfor)**
  *Authors*: Javad Dogani, Farshad Khunjush, Mehdi Seydali
  *Publication*: JGC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[esDNN: Deep Neural Network Based Multivariate Workload Prediction in Cloud Computing Environments](https://scholar.google.com/scholar?q=esDNN%3A%2BDeep%2BNeural%2BNetwork%2BBased%2BMultivariate)**
  *Authors*: Minxian Xu, Chenghao Song, Huaming Wu, Sukhpal Singh Gill, Kejiang Ye, Chengzhong Xu
  *Publication*: TOIT-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Graph Neural Network-Based SLO-Aware Proactive Resource Autoscaling Framework for Microservices](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Jinwoo Park, Byungkwon Choi, Chunghan Lee, Dongsu Han
  *Publication*: CoNEXT-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[HANSEL: Adaptive horizontal scaling of microservices using Bi-LSTM](https://scholar.google.com/scholar?q=HANSEL%3A%2BAdaptive%2Bhorizontal%2Bscaling%2Bof%2Bmicroservices)**
  *Authors*: Ming Yan, XiaoMeng Liang, ZhiHui Lu, Jie Wu, Wei Zhang
  *Publication*: APPL SOFT COMPUT-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[PYRAFORMER LOW-COMPLEXITY PYRAMIDAL ATTENTION FOR LONG-RANGE TIME SERIES MODELING](https://openreview.net/)**
  *Authors*: Shizhan Liu , , Hang Yu
  *Publication*: ICLR-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[An Integrated Approach for the Near Real-Time Parking Occupancy Prediction](https://scholar.google.com/scholar?q=An%2BIntegrated%2BApproach%2Bfor%2Bthe%2BNear)**
  *Authors*: Jun Li, Haohao Qu, Linlin You
  *Publication*: TITS-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Proactive auto-scaling for cloud environments using temporal convolutional neural networks](https://scholar.google.com/scholar?q=Proactive%2Bauto-scaling%2Bfor%2Bcloud%2Benvironments%2Busing)**
  *Authors*: Ehsan Golshani, Mehrdad Ashtiani
  *Publication*: JPDC-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[PERT-GNN: Latency Prediction for Microservice-based Cloud-Native Applications via Graph Neural Networks](https://dl.acm.org/conference/kdd)**
  *Authors*: Da Sun Handason Tam, Yang Liu, Huanle Xu, Siyue Xie, Wing Cheong Lau
  *Publication*: KDD-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Proactive Resource Autoscaling Scheme Based on SCINet for High-Performance Cloud Computing](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=8918)**
  *Authors*: Byeonghui Jeong, Jueun Jeon, Young-Sik Jeong
  *Publication*: TCC-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[DeepScaler: Holistic Autoscaling for Microservices Based on Spatiotemporal GNN with Adaptive Graph Learning](https://ieeexplore.ieee.org/document/10298341)**
  *Authors*: Chunyang Meng, Shijie Song, Haogang Tong, Maolin Pan, Yang Yu
  *Publication*: ASE-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Burst-Aware Predictive Autoscaling for Containerized Microservices](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Muhammad Abdullah, Waheed Iqbal, Josep Lluis Berral, Jorda Polo, David Carrera
  *Publication*: TSC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[An Efficient Multivariate Autoscaling Framework Using Bi-LSTM for Cloud Computing](https://scholar.google.com/scholar?q=An%2BEfficient%2BMultivariate%2BAutoscaling%2BFramework%2BUsing)**
  *Authors*: Nhat-Minh Dang-Quang, Myungsik Yoo
  *Publication*: 2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Learning Predictive Autoscaling Policies for Cloud-Hosted Microservices Using Trace-Driven Modeling](https://scholar.google.com/scholar?q=Learning%2BPredictive%2BAutoscaling%2BPolicies%2Bfor%2BCloud-Hosted)**
  *Authors*: Muhammad Abdullah, Waheed Iqbal, Abdelkarim Erradi, Faisal Bukhari
  *Publication*: 2019
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Proactive auto-scaling technique for web applications in container-based edge computing using federated learning model](https://scholar.google.com/scholar?q=Proactive%2Bauto-scaling%2Btechnique%2Bfor%2Bweb%2Bapplications)**
  *Authors*: Javad Dogani, Farshad Khunjush
  *Publication*: JPDC-2024
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Workload time series prediction in storage systems: a deep learning based approach](https://scholar.google.com/scholar?q=Workload%2Btime%2Bseries%2Bprediction%2Bin%2Bstorage)**
  *Authors*: Li Ruan, Yu Bai, Shaoning Li, Shuibing He, Limin Xiao
  *Publication*: CC-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[The Power of Prediction Microservice Auto Scaling via Workload Learning](https://dl.acm.org/conference/socc)**
  *Authors*: The Power of Prediction Microservice Auto Scaling
  *Publication*: SoCC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[The Power of Prediction Microservice Auto Scaling via Workload Learning PPT](https://dl.acm.org/conference/socc)**
  *Authors*: The Power of Prediction Microservice Auto Scaling
  *Publication*: SoCC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[SCINet: Time Series Modeling and Forecasting with Sample Convolution and Interaction](https://scholar.google.com/scholar?q=SCINet%3A%2BTime%2BSeries%2BModeling%2Band%2BForecasting)**
  *Authors*: Muxi Chen, Qiuxia Lai, Minhao Liu, Lingna Ma, Qiang Xu, Zhijian Xu, Ailing Zeng
  *Publication*: NeuIPS-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[PASS: Predictive Auto-Scaling System for Large-scale Enterprise Web Applications](https://scholar.google.com/scholar?q=PASS%3A%2BPredictive%2BAuto-Scaling%2BSystem%2Bfor%2BLarge-scale)**
  *Authors*: Yunda Guo, Jiake Ge, Panfeng Guo, Yunpeng Chai, Tao Li, Mengnan Shi, Yang Tu, Jian Ouyang
  *Publication*: 2024
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available


### Beyond DRL — Microservice Architecture & Analysis

- **[Adaptive Resource Efficient Microservice Deployment in Cloud-Edge Continuum](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Kaihua Fu, Wei Zhang, Quan Chen, Deze Zeng, Minyi Guo
  *Publication*: TPDS-2022
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[Seer Leveraging Big Data to Navigate the Complexity of Performance Debugging in Cloud Microservices](https://dl.acm.org/conference/asplos)**
  *Authors*: of Performance Debugging in Cloud Microservices
  *Publication*: ASPLOS-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[Performance Modeling for Cloud Microservice Applications](https://scholar.google.com/scholar?q=Performance%2BModeling%2Bfor%2BCloud%2BMicroservice%2BApplications)**
  *Authors*: Anshul Jindal, Vladimir Podolskiy, Michael Gerndt
  *Publication*: ICPE-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[µTune Auto-Tuned Threading for OLDI Microservices](https://www.usenix.org/conference/osdi)**
  *Authors*: Design, Implementation
  *Publication*: OSDI-2018
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[SoftSKU Optimizing Server Architectures for Microservice Diversity Scale](https://dl.acm.org/conference/isca)**
  *Authors*: Akshitha Sriraman , Abhishek Dhanotia , Thomas F. Wenisch
  *Publication*: ISCA-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[SmartVM: a SLA-aware microservice deployment framework](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Tianlei Zheng, Xi Zheng, Yuqun Zhang, Yao Deng, ErXi Dong, Rui Zhang, Xiao Liu
  *Publication*: WWWJ-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[SHOWAR Right-Sizing And Efficient Scheduling of Microservices](https://dl.acm.org/conference/socc)**
  *Authors*: SHOWAR Right-Sizing And Efficient Scheduling of
  *Publication*: SoCC-2021
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[QoS-Aware and Resource Efficient Microservice Deployment in Cloud-Edge Continuum](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Kaihua Fu, Wei Zhang, Quan Chen, Deze Zeng, Xin Peng, Wenli Zheng, Minyi Guo
  *Publication*: IPDPS-2021
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[A Kubernetes controller for managing the availability of elastic microservice based stateful applications](https://scholar.google.com/scholar?q=A%2BKubernetes%2Bcontroller%2Bfor%2Bmanaging%2Bthe)**
  *Authors*: Leila Abdollahi Vayghan, Mohamed Aymen Saied, Maria Toeroe, Ferhat Khendek
  *Publication*: 2021
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available


### Beyond DRL — Other

- **[1-s2.0-S1319157821000033-main](https://scholar.google.com/scholar?q=1-s2.0-S1319157821000033-main)**
  *Authors*: Arabinda Pradhan a, Sukant Kishoro Bisoy a, , Amardeep Das b
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Deep Learning-based Job Placement in Distributed Machine Learning Clusters](https://ieeexplore.ieee.org/document/8732818)**
  *Authors*: Yixin Bao, Yanghua Peng, Chuan Wu
  *Publication*: INFOCOM-2019
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Aladdin: Optimized Maximum Flow Management for Shared Production Clusters](https://ieeexplore.ieee.org/xpl/conhome/1000059/all-proceedings)**
  *Authors*: Heng Wu, Wenbo Zhang, Yuanjia Xu, Hao Xiang, Tao Huang, Haiyang Ding, Zheng Zhang
  *Publication*: IPDPS-2019
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Learning Driven Computation Offloading for Asymmetrically Informed Edge Computing](https://ieeexplore.ieee.org/document/8239581)**
  *Authors*: Miao Hu, Lei Zhuang, Di Wu, Yipeng Zhou, Xu Chen, Liang Xiao
  *Publication*: TPDS-2018
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Omega flexible scalable schedulers for large compute clusters](https://dl.acm.org/conference/eurosys)**
  *Authors*: new features can be deployed, decreases ef ciency, uti-
  *Publication*: EuroSys-2013
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[3719003](https://scholar.google.com/scholar?q=3719003)**
  *Authors*: Public Datasets for Cloud Computing A Comprehensive
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[A Study of Systems with Multiple Operating Levels, Probabilistic Thresholds and Hysteresis](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Alexandre Brandwajn, Thomas Begin, Hind Castel-Taleb, Tulin Atmaca
  *Publication*: TPDS-2018
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[A Hierarchical Receding Horizon Algorithm for QoS-Driven Control of Multi-IaaS Applications](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=8918)**
  *Authors*: Danilo Ardagna, Michele Ciavotta, Riccardo Lancellotti, Michele Guerriero
  *Publication*: TCC-2021
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[NeurIPS-2019-park-an-open-platform-for-learning-augmented-computer-systems-AuthorFeedback](https://scholar.google.com/scholar?q=NeurIPS-2019-park-an-open-platform-for-learning-augmented-computer-systems-AuthorFeedback)**
  *Authors*: We thank the reviewers for their interest in the paper, their constructive feedback. In the following, we address the
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[NeurIPS-2019-park-an-open-platform-for-learning-augmented-computer-systems-Paper](https://scholar.google.com/scholar?q=NeurIPS-2019-park-an-open-platform-for-learning-augmented-computer-systems-Paper)**
  *Authors*: Hongzi Mao, Parimarjan Negi, Akshay Narayan, Hanrui Wang, Jiacheng Yang
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[NeurIPS-2019-park-an-open-platform-for-learning-augmented-computer-systems-Supplemental](https://scholar.google.com/scholar?q=NeurIPS-2019-park-an-open-platform-for-learning-augmented-computer-systems-Supplemental)**
  *Authors*: Hongzi Mao, Parimarjan Negi, Akshay Narayan, Hanrui Wang, Jiacheng Yang
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Tetris-2014](https://scholar.google.com/scholar?q=Tetris-2014)**
  *Authors*: Multi-Resource Packing for Cluster Schedulers
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Scaling Large Production Clusters with Partitioned Synchronization](https://scholar.google.com/scholar?q=Scaling%2BLarge%2BProduction%2BClusters%2Bwith%2BPartitioned)**
  *Authors*: Scaling Large Production Clusters with
  *Publication*: USENIX ATC-2021
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[1-s2.0-S1574119222001353-main](https://scholar.google.com/scholar?q=1-s2.0-S1574119222001353-main)**
  *Authors*: Pervasive, Mobile Computing
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[3603166.3632165](https://scholar.google.com/scholar?q=3603166.3632165)**
  *Authors*: Machine Learning for Predictive Resource Scaling of
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Workload consolidation in alibaba clusters](https://dl.acm.org/conference/socc)**
  *Authors*: Yongkang Zhang, Yinghao Yu, Wei Wang, Qiukai Chen, Jie Wu, Zuowei Zhang, Jiang Zhong, Tianchen Ding, Qizhen Weng, Lingyun Yang
  *Publication*: SoCC-2022
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[UniSched: A Unified Scheduler for Deep Learning Training Jobs With Different User Demands](https://dl.acm.org/conference/socc)**
  *Authors*: Wei Gao, Zhisheng Ye, Peng Sun, Tianwei Zhang, Yonggang Wen
  *Publication*: SoCC-2021
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[ASTRAEA: A Fair Deep Learning Scheduler for Multi-Tenant GPU Clusters](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Zhisheng Ye, Peng Sun, Wei Gao, Tianwei Zhang, Xiaolin Wang, Shengen Yan, Yingwei Luo
  *Publication*: TPDS-2022
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[The vision of autonomic computing](https://scholar.google.com/scholar?q=The%2Bvision%2Bof%2Bautonomic%2Bcomputing)**
  *Authors*: J.O. Kephart, D.M. Chess
  *Publication*: 2003
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[978-3-031-48421-6](https://scholar.google.com/scholar?q=978-3-031-48421-6)**
  *Authors*: Flavia Monti Stefanie Rinderle-Ma
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[s10586-025-05237-9](https://scholar.google.com/scholar?q=s10586-025-05237-9)**
  *Authors*: Transformer-based performance prediction, proactive resource
  *Publication*: Unknown
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available


### Beyond DRL — Surveys & Reviews

- **[A Survey on Issues and Challenges of Load Balancing Techniques in Cloud Computing Environment](https://scholar.google.com/scholar?q=A%2BSurvey%2Bon%2BIssues%2Band%2BChallenges)**
  *Authors*: Febina K S, Tanuja Hemchand, Shamimunnisabi ., Roopa P, Aishwarya P
  *Publication*: ACS-2019
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[A comprehensive survey for scheduling techniques in cloud computing](https://www.sciencedirect.com/journal/journal-of-network-and-computer-applications)**
  *Authors*: Mohit Kumar, S.C. Sharma, Anubhav Goel, S.P. Singh
  *Publication*: JNCA-2019
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Cloud Dynamic Load Balancing and Reactive Fault Tolerance Techniques: A Systematic Literature Review (SLR)](https://scholar.google.com/scholar?q=Cloud%2BDynamic%2BLoad%2BBalancing%2Band%2BReactive)**
  *Authors*: Tawfeeg Mohmmed Tawfeeg, Adil Yousif, Alzubair Hassan, Samar M. Alqhtani, Rafik Hamza, Mohammed Bakri Bashir, Awad Ali
  *Publication*: IEEE-Access-2022
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Load balancing techniques in cloud computing environment: A review](https://scholar.google.com/scholar?q=Load%2Bbalancing%2Btechniques%2Bin%2Bcloud%2Bcomputing)**
  *Authors*: Dalia Abdulkareem Shafiq, N.Z. Jhanjhi, Azween Abdullah
  *Publication*: JKSU-CIS-2022
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[State of the Art on Microservices Autoscaling: An Overview](https://scholar.google.com/scholar?q=State%2Bof%2Bthe%2BArt%2Bon%2BMicroservices)**
  *Authors*: João Paulo K. S. Nunes, Thiago Bianchi, Anderson Y. Iwasaki, Elisa Yumi Nakagawa
  *Publication*: SBC-2021
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Machine Learning-based Orchestration of Containers: A Taxonomy and Future Directions](https://scholar.google.com/scholar?q=Machine%2BLearning-based%2BOrchestration%2Bof%2BContainers%3A%2BA)**
  *Authors*: Zhiheng Zhong, Minxian Xu, Maria Alejandra Rodriguez, Chengzhong Xu, Rajkumar Buyya
  *Publication*: ACMComSur-2022
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[A Survey and Taxonomy of Self-Aware and Self-Adaptive Cloud Autoscaling Systems](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Tao Chen, Rami Bahsoon, Xin Yao
  *Publication*: ACMComSur-2018
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Monte Carlo Tree Search: a review of recent modifications and applications](https://scholar.google.com/scholar?q=Monte%2BCarlo%2BTree%2BSearch%3A%2Ba%2Breview)**
  *Authors*: Maciej Świechowski, Konrad Godlewski, Bartosz Sawicki, Jacek Mańdziuk
  *Publication*: AIR-2023
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Beyond games: a systematic review of neural Monte Carlo tree search applications](https://scholar.google.com/scholar?q=Beyond%2Bgames%3A%2Ba%2Bsystematic%2Breview%2Bof)**
  *Authors*: Marco Kemmerling, Daniel Lütticke, Robert H. Schmitt
  *Publication*: AppIn-2024
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available


### Beyond DRL — System Design & Platform

- **[Large-scale cluster management at Google with Borg](https://dl.acm.org/conference/eurosys)**
  *Authors*: Abhishek Verma, Luis Pedrosa, Madhukar Korupolu, David Oppenheimer, Eric Tune, John Wilkes
  *Publication*: EuroSys-2015
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[Resilient Distributed Datasets A Fault-Tolerant Abstraction for In-Memory Cluster Computing](https://www.usenix.org/conference/nsdi)**
  *Authors*: Matei Zaharia, Mosharaf Chowdhury, Tathagata Das, Ankur Dave, Justin Ma
  *Publication*: NSDI-2012
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[LegoOS A Disseminated, Distributed OS for Hardware Resource Disaggregation](https://www.usenix.org/conference/osdi)**
  *Authors*: Design, Implementation
  *Publication*: OSDI-2018
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[Overload Control for Scaling WeChat Microservices](https://dl.acm.org/conference/socc)**
  *Authors*: Hao Zhou, Ming Chen, Qian Lin, Yong Wang, Xiaobin She, Sifan Liu, Rui Gu, Beng Chin Ooi, Junfeng Yang
  *Publication*: SoCC-2018
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[GrandSLAm Guaranteeing SLAs for Jobs in Microservices Execution Frameworks](https://dl.acm.org/conference/eurosys)**
  *Authors*: effort in adopting, maintaining servers by providing a
  *Publication*: EuroSys-2019
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[Service fabric a distributed platform for building microservices in the cloud](https://dl.acm.org/conference/eurosys)**
  *Authors*: Service Fabric A Distributed Platform for Building
  *Publication*: EuroSys-2018
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available


### Beyond DRL — Traditional Autoscaling

- **[ProScale: Proactive Autoscaling for Microservice With Time-Varying Workload at the Edge](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Ke Cheng, Sheng Zhang, Chenghong Tu, Xiaohang Shi, Zhaoheng Yin, Sanglu Lu, Yu Liang, Qing Gu
  *Publication*: TPDS-2023
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[An Auto-Scaling Approach for Microservices in Cloud Computing Environments](https://scholar.google.com/scholar?q=An%2BAuto-Scaling%2BApproach%2Bfor%2BMicroservices%2Bin)**
  *Authors*: Matineh ZargarAzad, Mehrdad Ashtiani
  *Publication*: 2023
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Cdascaler: a cost-effective dynamic autoscaling approach for containerized microservices](https://scholar.google.com/scholar?q=Cdascaler%3A%2Ba%2Bcost-effective%2Bdynamic%2Bautoscaling%2Bapproach)**
  *Authors*: Numan Shafi, Muhammad Abdullah, Waheed Iqbal, Abdelkarim Erradi, Faisal Bukhari
  *Publication*: 2024
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[AHPA: Adaptive Horizontal Pod Autoscaling Systems on Alibaba Cloud Container Service for Kubernetes](https://ojs.aaai.org/)**
  *Authors*: Zhiqiang Zhou, Chaoli Zhang, Lingna Ma, Jing Gu, Huajie Qian, Qingsong Wen, Liang Sun, Peng Li, Zhimin Tang
  *Publication*: AAAI-2023
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Coordinating Fast Concurrency Adapting With Autoscaling for SLO-Oriented Web Applications](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Jianshu Liu, Shungeng Zhang, Qingyang Wang, Jinpeng Wei
  *Publication*: TPDS-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Chameleon: A Hybrid, Proactive Auto-Scaling Mechanism on a Level-Playing Field](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Andre Bauer, Nikolas Herbst, Simon Spinner, Ahmed Ali-Eldin, Samuel Kounev
  *Publication*: TPDS-2019
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[DeepScaling: Autoscaling Microservices With Stable CPU Utilization for Large Scale Production Cloud Systems](https://dl.acm.org/doi/abs/10.1145/3542929.3563469)**
  *Authors*: Ziliang Wang, Shiyi Zhu, Jianguo Li, Wei Jiang, K. K. Ramakrishnan, Meng Yan, Xiaohong Zhang, Alex X. Liu
  *Publication*: SoCC-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[DeepScaling: Autoscaling Microservices With Stable CPU Utilization for Large Scale Production Cloud Systems](https://dl.acm.org/doi/abs/10.1145/3542929.3563469)**
  *Authors*: Ziliang Wang, Shiyi Zhu, Jianguo Li, Wei Jiang, K. K. Ramakrishnan, Meng Yan, Xiaohong Zhang, Alex X. Liu
  *Publication*: SoCC-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[DeepScaling: Autoscaling Microservices With Stable CPU Utilization for Large Scale Production Cloud Systems](https://dl.acm.org/doi/abs/10.1145/3542929.3563469)**
  *Authors*: Ziliang Wang, Shiyi Zhu, Jianguo Li, Wei Jiang, K. K. Ramakrishnan, Meng Yan, Xiaohong Zhang, Alex X. Liu
  *Publication*: TN-2024
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Proactive Autoscaling for Cloud-Native Applications using Machine Learning](https://ieeexplore.ieee.org/xpl/conhome/1000103/all-proceedings)**
  *Authors*: Nicolas Marie-Magdelaine, Toufik Ahmed
  *Publication*: GLOBECOM-2020
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Practical Efficient Microservice Autoscaling with QoS Assurance](https://dl.acm.org/conference/hpdc)**
  *Authors*: Md Rajib Hossen, Mohammad A. Islam, Kishwar Ahmed
  *Publication*: HPDC-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Practical Efficient Microservice Autoscaling with QoS Assurance](https://dl.acm.org/conference/hpdc)**
  *Authors*: Md Rajib Hossen, Mohammad A. Islam, Kishwar Ahmed
  *Publication*: HPDC-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[PBScaler: A Bottleneck-Aware Autoscaling Framework for Microservice-Based Applications](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Shuaiyu Xie, Jian Wang, Bing Li, Zekun Zhang, Duantengchuan Li, Patrick C. K. Hung
  *Publication*: TSC-2024
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Erlang: Application-Aware Autoscaling for Cloud Microservices](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Vighnesh Sachidananda, Anirudh Sivaraman
  *Publication*: arXiv-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[RobustScaler: QoS-Aware Autoscaling for Complex Workloads](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Huajie Qian, Qingsong Wen, Liang Sun, Jing Gu, Qiulin Niu, Zhimin Tang
  *Publication*: ICDE-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[ATOM: Model-Driven Autoscaling for Microservices](https://ieeexplore.ieee.org/xpl/conhome/1000050/all-proceedings)**
  *Authors*: Alim Ul Gias, Giuliano Casale, Murray Woodside
  *Publication*: ICDCS-2019
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[BASE: Burst-Adaptive Autoscaling via Stacked Ensembles for SLO Assurance and Cost Efficiency](https://arxiv.org/)**
  *Authors*: Chunyang Meng, Haogang Tong, Tianyang Wu, Maolin Pan, Yang Yu, Yi Jiang
  *Publication*: arXiv-2024
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Auto-Scaling Web Applications in Clouds](https://scholar.google.com/scholar?q=Auto-Scaling%2BWeb%2BApplications%2Bin%2BClouds)**
  *Authors*: Chenhao Qu, Rodrigo N. Calheiros, Rajkumar Buyya
  *Publication*: ACMComSur-2018
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[A bi-metric autoscaling approach for n-tier web applications on kubernetes](https://scholar.google.com/scholar?q=A%2Bbi-metric%2Bautoscaling%2Bapproach%2Bfor%2Bn-tier)**
  *Authors*: Changpeng Zhu, Bo Han, Yinliang Zhao
  *Publication*: FCS-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Autopilot: Workload Autoscaling at Google Scale](https://dl.acm.org/doi/10.1145/3342195.3387528)**
  *Authors*: Krzysztof Rząḑca, Paweł Findeisen, Jacek Świderski, Przemyslaw Zych, Przemyslaw Broniek, Jarek Kusmierek, Paweł Krzysztof Nowak, Beata Strack, Piotr Witusowski, Steven Hand
  *Publication*: EuroSys-2020
  *Summary*: This paper presents Google's Autopilot system for automatic workload autoscaling at production scale. It describes the design, implementation, and operational experience of a system that manages resource allocation across Google's infrastructure, using predictive models and feedback control to maintain service quality while optimizing resource utilization.
  **Code**: Not available

- **[Application deployment using containers with auto-scaling for microservices in cloud environment](https://scholar.google.com/scholar?q=Application%2Bdeployment%2Busing%2Bcontainers%2Bwith%2Bauto-scaling)**
  *Authors*: Satish Narayana Srirama, Mainak Adhikari, Souvik Paul
  *Publication*: 2020
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Deep Learning-Based Autoscaling Using Bidirectional Long Short-Term Memory for Kubernetes](https://scholar.google.com/scholar?q=Deep%2BLearning-Based%2BAutoscaling%2BUsing%2BBidirectional%2BLong)**
  *Authors*: Nhat-Minh Dang-Quang, Myungsik Yoo
  *Publication*: 2021
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[An adaptive auto-scaling framework for cloud resource provisioning](https://www.sciencedirect.com/journal/future-generation-computer-systems)**
  *Authors*: Spyridon Chouliaras, Stelios Sotiriadis
  *Publication*: FGCS-2023
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Horizontal Pod Autoscaling in Kubernetes Cluster Using Long Short-Term Memory](https://scholar.google.com/scholar?q=Horizontal%2BPod%2BAutoscaling%2Bin%2BKubernetes%2BCluster)**
  *Authors*: Somshekar Patil, D. G. Narayan, Ajeya Bhat, Aishwarya Hungund, Disha M. Patil
  *Publication*: 2024
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available


### Beyond DRL — Traditional Resource Management

- **[SLA-Based Scheduling of Spark Jobs in Hybrid Cloud Computing Environments](https://ieeexplore.ieee.org/document/9281647)**
  *Authors*: Muhammed Tawfiqul Islam, Huaming Wu, Shanika Karunasekera, Rajkumar Buyya
  *Publication*: TC-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Learning Resource Allocation and Pricing for Cloud Profit Maximization](https://ojs.aaai.org/)**
  *Authors*: Bingqian Du, Chuan Wu, Zhiyi Huang
  *Publication*: AAAI-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Learning scheduling algorithms for data processing clusters](https://dl.acm.org/doi/10.1145/3319535.3354223)**
  *Authors*: Hongzi Mao, Malte Schwarzkopf, Shaileshh Bojja Venkatakrishnan, Zili Meng, Mohammad Alizadeh
  *Publication*: SIGCOMM-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Modeling Analysis and Cost-Performance Ratio Optimization of Virtual Machine Scheduling in Cloud Computing](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Bo Wan, Jiale Dang, Zhetao Li, Hongfang Gong, Feng Zhang, Sangyoon Oh
  *Publication*: TPDS-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Who limits the resource efficiency of my datacenter](https://scholar.google.com/scholar?q=Who%2Blimits%2Bthe%2Bresource%2Befficiency%2Bof)**
  *Authors*: Jing Guo, Zihao Chang, Sa Wang, Haiyang Ding, Yihui Feng, Liang Mao, Yungang Bao
  *Publication*: IWQoS-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[A load balance oriented cost efficient scheduling method for parallel tasks](https://www.sciencedirect.com/journal/journal-of-network-and-computer-applications)**
  *Authors*: Yu Xin, Zhi-Qiang Xie, Jing Yang
  *Publication*: JNCA-2017
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Affinity-Aware Resource Provisioning for Long-Running Applications in Shared Clusters](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Clement Mommessin, Renyu Yang, Natalia Shakhlevich, Xiaoyang Sun, Satish Kumar, Junqing Xiao, Jie Xu
  *Publication*: JPDC-2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[TERMS: Task management policies to achieve high performance for mixed workloads using surplus resources](https://scholar.google.com/scholar?q=TERMS%3A%2BTask%2Bmanagement%2Bpolicies%2Bto%2Bachieve)**
  *Authors*: Jinyu Yu, Wei Tong, Pengze Lv, Dan Feng
  *Publication*: JPDC-2022
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Detection of SLA Violation for Big Data Analytics Applications in Cloud](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=12)**
  *Authors*: Xuezhi Zeng, Saurabh Garg, Mutaz Barika, Sanat Bista, Deepak Puthal, Albert Y. Zomaya, Rajiv Ranjan
  *Publication*: TC-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Hydra: Deadline-Aware and Efficiency-Oriented Scheduling for Deep Learning Jobs on Heterogeneous GPUs](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Zichao Yang, Heng Wu, Yuanjia Xu, Yuewen Wu, Hua Zhong, Wenbo Zhang
  *Publication*: 2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Zhao 和 Wu - 2022 - Large-Scale Machine Learning Cluster Scheduling vi](https://scholar.google.com/scholar?q=Zhao%2B%E5%92%8C%2BWu%2B-%2B2022%2B-)**
  *Authors*: Transactions on Network, Service Management
  *Publication*: Unknown
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Memory-harvesting VMs in cloud platforms](https://dl.acm.org/conference/asplos)**
  *Authors*: Alexander Fuerst, Stanko Novaković, Íñigo Goiri, Gohar Irfan Chaudhry, Prateek Sharma, Kapil Arya, Kevin Broas, Eugene Bak, Mehmet Iyigun, Ricardo Bianchini
  *Publication*: ASPLOS-2022
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Deep Learning and Cloud Computing](https://scholar.google.com/scholar?q=Deep%2BLearning%2Band%2BCloud%2BComputing)**
  *Authors*: Pramod Gupta, Naresh K. Sehgal
  *Publication*: Code-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[SAAS parallel task scheduling based on cloud service flow load algorithm](https://scholar.google.com/scholar?q=SAAS%2Bparallel%2Btask%2Bscheduling%2Bbased%2Bon)**
  *Authors*: Jian Zhu, Qian Li, Shi Ying
  *Publication*: Comp. Com-2022
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Cost-efficient dynamic scheduling of big data applications in apache spark on cloud](https://scholar.google.com/scholar?q=Cost-efficient%2Bdynamic%2Bscheduling%2Bof%2Bbig%2Bdata)**
  *Authors*: Muhammed Tawfiqul Islam, Satish Narayana Srirama, Shanika Karunasekera, Rajkumar Buyya
  *Publication*: JSS-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[ThermoSim: Deep learning based framework for modeling and simulation of thermal-aware resource management for cloud computing environments](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Sukhpal Singh Gill, Shreshth Tuli, Adel Nadjaran Toosi, Felix Cuadrado, Peter Garraghan, Rami Bahsoon, Hanan Lutfiyya, Rizos Sakellariou, Omer Rana, Schahram Dustdar
  *Publication*: JSS-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Generating Complex, Realistic Cloud Workloads using Recurrent Neural Networks](https://dl.acm.org/conference/sosp)**
  *Authors*: Shane Bergsma, Timothy Zeyl, Arik Senderovich, J. Christopher Beck
  *Publication*: SOSP-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Scavenger A Black-Box Batch Workload Resource Manager for Improving Utilization in Cloud Environments](https://dl.acm.org/conference/socc)**
  *Authors*: Scavenger A Black-Box Batch Workload Resource Manager for
  *Publication*: SoCC-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Adversarial Deep Learning for Online Resource Allocation](https://scholar.google.com/scholar?q=Adversarial%2BDeep%2BLearning%2Bfor%2BOnline%2BResource)**
  *Authors*: Bingqian Du, Zhiyi Huang, Chuan Wu
  *Publication*: TOMPECS-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[DDRM: An SLO-aware Deep Dynamic Resource Management Framework for Microservices](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Liangping Tang, Jin Wang, Wanyou Wang, Gaotao Shi, Zhijun Li
  *Publication*: OSDI-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[State Space Model and Queuing Network Based Cloud Resource Provisioning for Meshed Web Systems](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=71)**
  *Authors*: Yamin Lei, Zhicheng Cai, Xiaoping Li, Rajkumar Buyya
  *Publication*: TPDS-2022
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Sinan: ML-based and QoS-aware resource management for cloud microservices](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**
  *Authors*: Yanqi Zhang, Weizhe Hua, Zhuangzhuang Zhou, G. Edward Suh, Christina Delimitrou
  *Publication*: ASPLOS-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Distributed resource management across process boundaries](https://dl.acm.org/conference/socc)**
  *Authors*: Lalith Suresh, Peter Bodik, Ishai Menache, Marco Canini, Florin Ciucu
  *Publication*: SoCC-2017
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[K8sSim: A Simulation Tool for Kubernetes Schedulers and Its Applications in Scheduling Algorithm Optimization](https://scholar.google.com/scholar?q=K8sSim%3A%2BA%2BSimulation%2BTool%2Bfor%2BKubernetes)**
  *Authors*: Shilin Wen, Rui Han, Ke Qiu, Xiaoxin Ma, Zeqing Li, Hongjie Deng, Chi Harold Liu
  *Publication*: MicroM-2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[HSACMA: a hierarchical scalable adaptive cloud monitoring architecture](https://scholar.google.com/scholar?q=HSACMA%3A%2Ba%2Bhierarchical%2Bscalable%2Badaptive%2Bcloud)**
  *Authors*: Rui Wang, Shi Ying, Meiyan Li, Shun Jia
  *Publication*: SQJ-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Maintaining SLOs of Cloud-Native Applications Via Self-Adaptive Resource Sharing](https://ieeexplore.ieee.org/xpl/conhome/1000133/all-proceedings)**
  *Authors*: Vladimir Podolskiy, Michael Mayo, Abigail Koay, Michael Gerndt, Panos Patros
  *Publication*: SASO-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Maintaining SLOs of Cloud-Native Applications Via Self-Adaptive Resource Sharing](https://ieeexplore.ieee.org/xpl/conhome/1000133/all-proceedings)**
  *Authors*: Vladimir Podolskiy, Michael Mayo, Abigail Koay, Michael Gerndt, Panos Patros
  *Publication*: SASO-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Erms: Efficient Resource Management for Shared Microservices with SLA Guarantees](https://dl.acm.org/conference/asplos)**
  *Authors*: Shutian Luo, Huanle Xu, Kejiang Ye, Guoyao Xu, Liping Zhang, Jian He, Guodong Yang, Chengzhong Xu
  *Publication*: ASPLOS-2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Optimizing Resource Management for Shared Microservices: A Scalable System Design](https://scholar.google.com/scholar?q=Optimizing%2BResource%2BManagement%2Bfor%2BShared%2BMicroservices%3A)**
  *Authors*: Shutian Luo, Chenyu Lin, Kejiang Ye, Guoyao Xu, Liping Zhang, Guodong Yang, Huanle Xu, Chengzhong Xu
  *Publication*: TOCS-2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available


### Beyond DRL — Workload Analysis & Characterization

- **[Characterizing Microservice Dependency and Performance](https://dl.acm.org/conference/socc)**
  *Authors*: Shutian Luo, Huanle Xu, Chengzhi Lu, Kejiang Ye, Guoyao Xu, Liping Zhang, Yu Ding, Jian He, Chengzhong Xu
  *Publication*: SoCC-2021
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterizing and Synthesizing Task Dependencies of Data-Parallel Jobs in Alibaba Cloud](https://dl.acm.org/conference/socc)**
  *Authors*: Huangshi Tian, Yunchuan Zheng, Wei Wang
  *Publication*: SoCC-2019
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterizing Co-Located Workloads in Alibaba Cloud Datacenters](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=8918)**
  *Authors*: Congfeng Jiang, Yitao Qiu, Weisong Shi, Zhefeng Ge, Jiwei Wang, Shenglei Chen, Christophe Cerin, Zujie Ren, Guoyao Xu, Jiangbin Lin
  *Publication*: TCC-2022
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Imbalance in the cloud: An analysis on Alibaba cluster trace](https://scholar.google.com/scholar?q=Imbalance%2Bin%2Bthe%2Bcloud%3A%2BAn%2Banalysis)**
  *Authors*: Chengzhi Lu, Kejiang Ye, Guoyao Xu, Cheng-Zhong Xu, Tongxin Bai
  *Publication*: BIGDATA-2017
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characteristics of Co-Allocated Online Services and Batch Jobs in Internet Data Centers: A Case Study From Alibaba Cloud](https://scholar.google.com/scholar?q=Characteristics%2Bof%2BCo-Allocated%2BOnline%2BServices%2Band)**
  *Authors*: Congfeng Jiang, Guangjie Han, Jiangbin Lin, Gangyong Jia, Weisong Shi, Jian Wan
  *Publication*: IEEE-Access-2019
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterizing Job-Task Dependency in Cloud Workloads Using Graph Learning](https://ieeexplore.ieee.org/xpl/conhome/1000059/all-proceedings)**
  *Authors*: Zhaochen Gu, Sihai Tang, Beilei Jiang, Song Huang, Qiang Guan, Song Fu
  *Publication*: IPDPSW-2021
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterizing Job Microarchitectural Profiles at Scale: Dataset and Analysis](https://dl.acm.org/conference/socc)**
  *Authors*: Kangjin Wang, Ying Li, Cheng Wang, Tong Jia, Kingsum Chow, Yang Wen, Yaoyong Dou, Guoyao Xu, Chuanjia Hou, Jie Yao
  *Publication*: SoCC-2022
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterization and prediction of deep learning workloads in large-scale GPU datacenters](https://dl.acm.org/conference/sc)**
  *Authors*: Qinghao Hu, Peng Sun, Shengen Yan, Yonggang Wen, Tianwei Zhang
  *Publication*: SC-2021
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available


---

## Datasets

- **[alibaba/clusterdata](https://github.com/alibaba/clusterdata?tab=readme-ov-file)** – Alibaba Cluster Trace Program, cluster data collected from production clusters in Alibaba for cluster management research.

---

## Contributing

Contributions welcome!

1. Fork this repository.
2. Create a branch for your addition (paper, dataset, project, etc.).
3. Add your entry including title, link, authors, and a brief summary.
4. Submit a pull request—maintainers will review and merge.

---

## References

Below are repositories and related works that inspired this collection:

- **[pkoperek/drl-cloud-management-list](https://github.com/pkoperek/drl-cloud-management-list)** – A list of DRL cloud management papers.

We sincerely thank the maintainers and authors of these repositories for their foundational contributions.

---

## License

This repository is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.
