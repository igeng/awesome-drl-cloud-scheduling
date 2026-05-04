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

- **[<i>Microscaler</i>: Cost-Effective Scaling for Microservice Applications in the Cloud With an Online Learning Approach](https://scholar.google.com/scholar?q=iMicroscaleri%3A%2BCost-Effective%2BScaling%2Bfor%2BMicroservice%2BApplications%2Bin%2Bthe%2BCloud%2BWith%2Ban%2BOnline%2BLearning%2BApproach)**
  *Authors*: Guangba Yu, Pengfei Chen, Zibin Zheng
  *Publication*: TCC-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A Dual-Agent Scheduler for Distributed Deep Learning Jobs on Public Cloud via Reinforcement Learning](https://dl.acm.org/doi/10.1145/3580305.3599378)**
  *Authors*: Mingzhe Xing, Hangyu Mao, Shenglin Yin, Lichen Pan, Zhengchao Zhang, Zhen Xiao, Jieyi Long
  *Publication*: KDD-2023
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A heuristic multi-objective task scheduling framework for container-based clouds via actor-critic reinforcement learning](https://www.sciencedirect.com/science/article/pii/S0743731523000273)**
  *Authors*: Lilu Zhu, Feng Wu, Yanfeng Hu, Kai Huang, Xinmei Tian
  *Publication*: 2023
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A Hierarchical Framework of Cloud Resource Allocation and Power Management Using Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/7970343)**
  *Authors*: Ning Liu, Zhe Li, Jielong Xu, Zhiyuan Xu, Sheng Lin, Qinru Qiu, Jian Tang, Yanzhi Wang
  *Publication*: ICDCS-2017
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[A multi-objective trade-off framework for cloud resource scheduling based on the Deep Q-network algorithm](https://link.springer.com/article/10.1007/s10586-021-03384-2)**
  *Authors*: Zhiping Peng, Jianpeng Lin, Delong Cui, Qirui Li, Jieguang He
  *Publication*: Cluster Computing-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Actor-Critic with Transformer for Cloud Computing Resource Three Stage Job Scheduling](https://ieeexplore.ieee.org/document/9834560)**
  *Authors*: Yanbo Xu, Jiakun Zhao
  *Publication*: ICCCBDA-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Adaptive and Efficient Resource Allocation in Cloud Datacenters Using Actor-Critic Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9606309)**
  *Authors*: Zheyi Chen, Jia Hu, Geyong Min, Chunbo Luo, Tarek El-Ghazawi
  *Publication*: TPDS-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[ADRL: A Hybrid Anomaly-Aware Deep Reinforcement Learning-Based Resource Scaling in Clouds](https://ieeexplore.ieee.org/document/9379433)**
  *Authors*: Sara Kardani-Moghaddam, Rajkumar Buyya, Kotagiri Ramamohanarao
  *Publication*: TPDS-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Cloud Resource Scheduling With Deep Reinforcement Learning and Imitation Learning](https://ieeexplore.ieee.org/document/9371419)**
  *Authors*: Wenxia Guo, Wenhong Tian, Yufei Ye, Lingxiao Xu, Kui Wu
  *Publication*: IOTJ-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Cost-aware job scheduling for cloud instances using deep reinforcement learning](https://link.springer.com/article/10.1007/s10586-021-03386-0)**
  *Authors*: Feng Cheng, Yifeng Huang, Bhavana Tanpure, Pawan Sawalani, Long Cheng, Cong Liu
  *Publication*: Cluster Computing-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Data Centers Job Scheduling with Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9239886)**
  *Authors*: Sisheng Liang, Zhou Yang, Fang Jin, Yong Chen
  *Publication*: PAKDD-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[DDQN-TS: A novel bi-objective intelligent scheduling algorithm in the cloud environment](https://www.sciencedirect.com/science/article/pii/S0925231221000419)**
  *Authors*: Zhao Tong, Feng Ye, Bilan Liu, Jinhui Cai, Jing Mei
  *Publication*: Neurocomputing-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning based Compute-Intensive Workload Allocation in Data Centers with High Energy Efficiency](https://ieeexplore.ieee.org/document/9458229)**
  *Authors*: Zhenfeng Gao, Wei Liu, Long Suo, Jiandong Li, Yijun Lu
  *Publication*: ICCC-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning Enhanced Greedy Algorithm for Online Scheduling of Batched Tasks in Cloud in Cloud HPC Systems](https://scholar.google.com/scholar?q=Deep%2BReinforcement%2BLearning%2BEnhanced%2BGreedy%2BAlgorithm%2Bfor%2BOnline%2BScheduling%2Bof%2BBatched%2BTasks%2Bin%2BCloud%2Bin%2BCloud%2BHPC%2BSystems)**
  *Authors*: Yuanhao Yang, Hong Shen
  *Publication*: TPDS-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning for Dynamic Workflow Scheduling in Cloud Environment](https://ieeexplore.ieee.org/document/9458233)**
  *Authors*: Tingting Dong, Fei Xue, Changbai Xiao, Jiangjiang Zhang
  *Publication*: SCC-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning for Multi-resource Cloud Job Scheduling](https://scholar.google.com/scholar?q=Deep%2BReinforcement%2BLearning%2Bfor%2BMulti-resource%2BCloud)**
  *Authors*: Jianpeng Lin, Zhiping Peng, Delong Cui
  *Publication*: ICNP-2017
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep reinforcement learning-aided multi-step job scheduling in optical data center networks](https://scholar.google.com/scholar?q=Deep%2Breinforcement%2Blearning-aided%2Bmulti-step%2Bjob%2Bscheduling)**
  *Authors*: Che-Yu Liu, Xiaoliang Chen, Roberto Proietti, Zuqing Zhu, S. J. Ben Yoo
  *Publication*: ICDBC-2025
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep reinforcement learning-based methods for resource scheduling in cloud computing: a review and future directions](https://arxiv.org/abs/2103.16428)**
  *Authors*: Guangyao Zhou, Wenhong Tian, Rajkumar Buyya, Ruini Xue, Liang Song
  *Publication*: arXiv-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[DeepEE: Joint Optimization of Job Scheduling and Cooling Control for Data Center Energy Efficiency Using Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/8774708)**
  *Authors*: Yongyi Ran, Han Hu, Xin Zhou, Yonggang Wen
  *Publication*: ICDCS-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[DRAS: Deep Reinforcement Learning for Cluster Scheduling in High Performance Computing](https://ieeexplore.ieee.org/document/9678505)**
  *Authors*: Yuping Fan, Boyang Li, Dustin Favorite, Naunidh Singh, Taylor Childers, Paul Rich, William Allcock, Michael E. Papka, Zhiling Lan
  *Publication*: TPDS-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[DRL-cloud: Deep reinforcement learning-based resource provisioning and task scheduling for cloud service providers](https://ieeexplore.ieee.org/document/8363878)**
  *Authors*: Mingxi Cheng, Ji Li, Shahin Nazarian
  *Publication*: ASP-DAC-2018
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Dynamic Job Shop Scheduling via Deep Reinforcement Learning](https://proceedings.neurips.cc/)**
  *Authors*: Xinjie Liang, Wen Song, Pengfei Wei
  *Publication*: NeurIPS-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Efficient Compute-Intensive Job Allocation in Data Centers via Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9121728)**
  *Authors*: Deliang Yi, Xin Zhou, Yonggang Wen, Rui Tan
  *Publication*: TPDS-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Energy-Efficient Task Scheduling in Data Centers Using Adaptive Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Energy-Efficient%2BTask%2BScheduling%2Bin%2BData%2BCenters)**
  *Authors*: Dinuț Ionuț-Cosmin, Bogdan Alexandrescu, Rodica-Claudia Constantinescu
  *Publication*: Code-2025
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[GARLSched: Generative adversarial deep reinforcement learning task scheduling optimization for large-scale high performance computing systems](https://www.sciencedirect.com/science/article/pii/S0167739X21003815)**
  *Authors*: Jingbo Li, Xingjun Zhang, Jia Wei, Zeyu Ji, Zheng Wei
  *Publication*: FGCS-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[gym-hpa: Efficient Auto-Scaling via Reinforcement Learning for Complex Microservice-based Applications in Kubernetes](https://ieeexplore.ieee.org/document/10145462)**
  *Authors*: José Santos, Tim Wauters, Bruno Volckaert, Filip De Turck
  *Publication*: NOMS-2023
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Heterogeneous-Aware Online Cloud Task Scheduler Based on Clustering and Deep Reinforcement Learning Ensemble](https://ieeexplore.ieee.org/document/9458230)**
  *Authors*: Dan Gu, Jing Chen, Xiaoyu Shi, Longyu Ran, Ying Zhang, Mingsheng Shang
  *Publication*: ICNC-FSKD-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Integrated and Fungible Scheduling of Deep Learning Workloads Using Multi-Agent Reinforcement Learning](https://ieeexplore.ieee.org/document/9834556)**
  *Authors*: Jialun Li, Danyang Xiao, Diying Yang, Xuan Mo, Weigang Wu
  *Publication*: 2025
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Minerva: A reinforcement learning-based technique for optimal scheduling and bottleneck detection in distributed factory operations](https://ieeexplore.ieee.org/document/8623945)**
  *Authors*: Tara Elizabeth Thomas, Jinkyu Koo, Somali Chaterji, Saurabh Bagchi
  *Publication*: ICCSN-2018
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Model-free control for distributed stream data processing using deep reinforcement learning](https://www.vldb.org/pvldb/vol11/p500-li.pdf)**
  *Authors*: Teng Li, Zhiyuan Xu, Jian Tang, Yanzhi Wang
  *Publication*: VLDB-2018
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Multi-Dimensional Resource Allocation in Distributed Data Centers Using Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Multi-Dimensional%2BResource%2BAllocation%2Bin%2BDistributed%2BData%2BCenters%2BUsing%2BDeep%2BReinforcement%2BLearning)**
  *Authors*: Wenting Wei, Huaxi Gu, Kun Wang, Jianjia Li, Xuan Zhang, Ning Wang
  *Publication*: TNSM-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Optimizing Job Scheduling using Deep Reinforcement Learning](https://dl.acm.org/conference/hpdc)**
  *Authors*: Rohit Sigar, Avadh Kishor, Pramod Kumar Singh, Joydip Dhar
  *Publication*: HPDC-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Performance and Cost-Efficient Spark Job Scheduling Based on Deep Reinforcement Learning in Cloud Computing Environments](https://ieeexplore.ieee.org/document/9354797)**
  *Authors*: Muhammed Tawfiqul Islam, Shanika Karunasekera, Rajkumar Buyya
  *Publication*: TPDS-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[READYS: A Reinforcement Learning Based Strategy for Heterogeneous Dynamic Scheduling](https://ieeexplore.ieee.org/document/9519058)**
  *Authors*: Nathan Grinsztajn, Olivier Beaumont, Emmanuel Jeannot, Philippe Preux
  *Publication*: CLUSTER-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Resource Management with Deep Reinforcement Learning](https://dl.acm.org/doi/10.1145/3013727.3013736)**
  *Authors*: Hongzi Mao, Mohammad Alizadeh, Ishai Menache, Srikanth Kandula
  *Publication*: HotNets-2016
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[RLQ: Workload Allocation With Reinforcement Learning in Distributed Queues](https://ieeexplore.ieee.org/document/10089811)**
  *Authors*: Alessandro Staffolani, Victor-Alexandru Darvariu, Paolo Bellavista, Mirco Musolesi
  *Publication*: TPDS-2023
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[RLScheduler: An Automated HPC Batch Job Scheduler Using Reinforcement Learning](https://dl.acm.org/doi/10.1145/3468267.3476137)**
  *Authors*: Di Zhang, Dong Dai, Youbiao He, Forrest Sheng Bao, Bing Xie
  *Publication*: SC-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[RLSK: A Job Scheduler for Federated Kubernetes Clusters based on Reinforcement Learning](https://ieeexplore.ieee.org/document/9458228)**
  *Authors*: Jiaming Huang, Chuming Xiao, Weigang Wu
  *Publication*: IC2E-2020
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Scheduling of Time-Varying Workloads Using Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/16190)**
  *Authors*: Shanka Subhra Mondal, Nikhil Sheoran, Subrata Mitra
  *Publication*: AAAI-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[SibylOpt: Managing Green Data Centers Using Off-Online Deep Reinforcement Learning](https://scholar.google.com/scholar?q=SibylOpt%3A%2BManaging%2BGreen%2BData%2BCenters%2BUsing%2BOff-Online%2BDeep%2BReinforcement%2BLearning)**
  *Authors*: Ning Gu, Kuo Zhang, Thu Nguyen, Peijian Wang, Tania Lorido Botran
  *Publication*: SoCC-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[SIMPPO: A Scalable and Incremental Online Learning Framework for Serverless Resource Management](https://dl.acm.org/doi/10.1145/3542929.3563483)**
  *Authors*: Jiaming Huang, Chuming Xiao, Weigang Wu
  *Publication*: SoCC-2022
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[SLAs-Aware Online Task Scheduling Based on Deep Reinforcement Learning Method in Cloud Environment](https://ieeexplore.ieee.org/document/9048648)**
  *Authors*: Longyu Ran, Xiaoyu Shi, Mingsheng Shang
  *Publication*: HPCC-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Spear: Optimized Dependency-Aware Task Scheduling with Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/8774709)**
  *Authors*: Zhiming Hu, James Tu, Baochun Li
  *Publication*: ICDCS-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Task Scheduling in Cloud Using Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9834560)**
  *Authors*: Shashank Swarup, Elhadi M. Shakshuki, Ansar Yasar
  *Publication*: Code-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

- **[Toward Efficient Compute-Intensive Job Allocation for Green Data Centers: A Deep Reinforcement Learning Approach](https://ieeexplore.ieee.org/document/8812700)**
  *Authors*: Deliang Yi, Xin Zhou, Yonggang Wen, Rui Tan
  *Publication*: ICDCS-2019
  *Summary*: This paper proposes a deep reinforcement learning approach for cloud resource scheduling. The method learns optimal scheduling policies through environment interaction, adapting to dynamic workload patterns and heterogeneous server capabilities. Experimental results demonstrate improved resource utilization, reduced job completion time, and better cost efficiency compared to traditional scheduling approaches.
  **Code**: Not available

---

### DRL — Autoscaling

- **[A Meta Reinforcement Learning Approach for Predictive Autoscaling in the Cloud](https://dl.acm.org/doi/10.1145/3543873.3587200)**
  *Authors*: Siqiao Xue, Chao Qu, Xiaoming Shi, Cong Liao, Shiyi Zhu, Xiaoyu Tan, Lintao Ma, Shiyu Wang, Shijun Wang, Yun Hu
  *Publication*: KDD-2022
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[A-SARSA: A Predictive Container Auto-Scaling Algorithm Based on Reinforcement Learning](https://ieeexplore.ieee.org/document/9239887)**
  *Authors*: Shubo Zhang, Tianyang Wu, Maolin Pan, Chaomeng Zhang, Yang Yu
  *Publication*: ICWS-2020
  *Summary*: This paper presents a reinforcement learning-based autoscaling mechanism for cloud services. The approach uses DRL to automatically adjust resource allocation based on workload patterns and performance requirements. The system achieves better SLO compliance and resource efficiency compared to rule-based scaling approaches.
  **Code**: Not available

- **[AWARE Automate Workload Autoscaling with Reinforcement Learning in Production Cloud Systems](https://scholar.google.com/scholar?q=AWARE%2BAutomate%2BWorkload%2BAutoscaling%2Bwith%2BReinforcement%2BLearning%2Bin%2BProduction%2BCloud%2BSystems)**
  *Authors*: Haoran Qiu, Weichao Mao
  *Publication*: ATC-2023
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[DScaler: A Horizontal Autoscaler of Microservice Based on Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9834562)**
  *Authors*: Zhijiao Xiao, Song Hu
  *Publication*: APNOMS-2022
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[Fast and Fine-grained Autoscaler for Streaming Jobs with Reinforcement Learning](https://arxiv.org/abs/2201.08439)**
  *Authors*: Mingzhe Xing, Hangyu Mao, Zhen Xiao
  *Publication*: IJCAI-2022
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[Intelligent microservices autoscaling module using reinforcement learning](https://ieeexplore.ieee.org/document/10148703)**
  *Authors*: Abeer Abdel Khaleq, Ilkyeun Ra
  *Publication*: CC-2023
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[Microscaler: Automatic Scaling for Microservices with an Online Learning Approach](https://ieeexplore.ieee.org/document/8796946)**
  *Authors*: Guangba Yu, Pengfei Chen, Zibin Zheng
  *Publication*: ICWS-2019
  *Summary*: This paper presents a reinforcement learning-based autoscaling mechanism for cloud services. The approach uses DRL to automatically adjust resource allocation based on workload patterns and performance requirements. The system achieves better SLO compliance and resource efficiency compared to rule-based scaling approaches.
  **Code**: Not available

- **[Reinforcement learning-assisted autoscaling mechanisms for serverless computing platforms](https://scholar.google.com/scholar?q=Reinforcement%2Blearning-assisted%2Bautoscaling%2Bmechanisms%2Bfor%2Bserverless)**
  *Authors*: Anastasios Zafeiropoulos, Eleni Fotopoulou, Nikos Filinis, Symeon Papavassiliou
  *Publication*: SMPT-2022
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

---

### DRL — Edge Computing

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

- **[Deep Reinforcement Learning for Load-Balancing Aware Network Control in IoT Edge Systems](https://ieeexplore.ieee.org/document/9614568)**
  *Authors*: Qingzhi Liu, Tiancong Xia, Long Cheng, Merijn van Eijk, Tanir Ozcelebi, Ying Mao
  *Publication*: TPDS-2022
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Deep Reinforcement Learning-Based Workload Scheduling for Edge Computing](https://link.springer.com/article/10.1007/s10586-021-03387-z)**
  *Authors*: Tao Zheng, Jian Wan, Jilin Zhang, Congfeng Jiang
  *Publication*: JCCASA-2022
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Dynamic Scheduling for Stochastic Edge-Cloud Computing Environments Using A3C Learning and Residual Recurrent Neural Networks](https://ieeexplore.ieee.org/document/9000076)**
  *Authors*: Shreshth Tuli, Shashikant Ilager, Kotagiri Ramamohanarao, Rajkumar Buyya
  *Publication*: TMC-2020
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Energy Efficient Task Scheduling in Fog Environment using Deep Reinforcement Learning Approach](https://scholar.google.com/scholar?q=Energy%2BEfficient%2BTask%2BScheduling%2Bin%2BFog)**
  *Authors*: Shashank Swarup, Elhadi M. Shakshuki, Ansar Yasar
  *Publication*: 2021
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Neural Task Scheduling with Reinforcement Learning for Fog Computing Systems](https://ieeexplore.ieee.org/document/8887943)**
  *Authors*: Simeng Bian, Xi Huang, Ziyu Shao, Yang Yang
  *Publication*: GLOBECOM-2019
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Optimization of lightweight task offloading strategy for mobile edge computing based on deep reinforcement learning](https://www.sciencedirect.com/science/article/pii/S0167739X19305568)**
  *Authors*: Haifeng Lu, Chunhua Gu, Fei Luo, Weichao Ding, Xinping Liu
  *Publication*: FGCS-2020
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

---

### DRL — Robustness & Security

- **[Adversarial Attacks in a Deep Reinforcement Learning based Cluster Scheduler](https://ieeexplore.ieee.org/document/9834554)**
  *Authors*: Shaojun Zhang, Chen Wang, Albert Y. Zomaya
  *Publication*: 2020
  *Summary*: This paper investigates the robustness and security of deep reinforcement learning-based schedulers in cloud environments. The study identifies vulnerabilities to adversarial attacks and proposes defense mechanisms to enhance scheduler stability. The work provides insights into the reliability of DRL schedulers under varying conditions.
  **Code**: Not available

- **[Adversarial Deep Learning for Online Resource Allocation](https://ieeexplore.ieee.org/document/9458234)**
  *Authors*: Bingqian Du, Zhiyi Huang, Chuan Wu
  *Publication*: TOMPECS-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Robustness Analysis and Enhancement of Deep Reinforcement Learning-Based Schedulers](https://ieeexplore.ieee.org/document/9834558)**
  *Authors*: Shaojun Zhang, Chen Wang, Albert Y. Zomaya
  *Publication*: 2023
  *Summary*: This paper investigates the robustness and security of deep reinforcement learning-based schedulers in cloud environments. The study identifies vulnerabilities to adversarial attacks and proposes defense mechanisms to enhance scheduler stability. The work provides insights into the reliability of DRL schedulers under varying conditions.
  **Code**: Not available

---

### Beyond DRL — Benchmarks & Simulators

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

- **[BigDataBench-S: An Open-Source Scientific Big Data Benchmark Suite](https://ieeexplore.ieee.org/document/7970344)**
  *Authors*: Xinhui Tian, Shaopeng Dai, Zhihui Du, Wanling Gao, Rui Ren, Yaodong Cheng, Zhifei Zhang, Zhen Jia, Peijian Wang, Jianfeng Zhan
  *Publication*: IPDPSW-2017
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[BigDataBench: A big data benchmark suite from internet services](https://ieeexplore.ieee.org/document/6804890)**
  *Authors*: Lei Wang, Jianfeng Zhan, Chunjie Luo, Yuqing Zhu, Qiang Yang, Yongqiang He, Wanling Gao, Zhen Jia, Yingjie Shi, Shujie Zhang
  *Publication*: HPCA-2014
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[GloudSim: Google trace based cloud simulator with virtual machines](https://www.sciencedirect.com/science/article/pii/S1383762121001060)**
  *Authors*: Sheng Di, Franck Cappello
  *Publication*: 2015
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[PerfSim: A Performance Simulator for Cloud Native Microservice Chains](https://ieeexplore.ieee.org/document/10089815)**
  *Authors*: Michel Gokan Khan, Javid Taheri, Auday Al-Dulaimy, Andreas Kassler
  *Publication*: 2023
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[μBench: An Open-Source Factory of Benchmark Microservice Applications](https://scholar.google.com/scholar?q=Bench%3A%2BAn%2BOpen-Source%2BFactory%2Bof%2BBenchmark%2BMicroservice%2BApplications)**
  *Authors*: Andrea Detti, Ludovico Funari, Luca Petrucci
  *Publication*: TPDS-2021
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

---

### Beyond DRL — Heuristic & Evolutionary Scheduling

- **[A Cooperative Coevolution Genetic Programming Hyper-Heuristics Approach for On-Line Resource Allocation in Container-Based Clouds](https://ieeexplore.ieee.org/document/9678510)**
  *Authors*: Boxiong Tan, Hui Ma, Yi Mei, Mengjie Zhang
  *Publication*: 2022
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[A discrete PSO-based static load balancing algorithm for distributed simulations in a cloud environment](https://www.sciencedirect.com/science/article/pii/S0167739X20332606)**
  *Authors*: Zhang Miao, Peng Yong, Yang Mei, Yin Quanjun, Xie Xu
  *Publication*: FGCS-2021
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[A multi-objective load balancing algorithm for virtual machine placement in cloud data centers based on machine learning](https://www.sciencedirect.com/science/article/pii/S1383762119301061)**
  *Authors*: Arezoo Ghasemi, Abolfazl Toroghi Haghighat
  *Publication*: Computing-2020
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Combining Size-Based Load Balancing with Round-Robin for Scalable Low Latency](https://ieeexplore.ieee.org/document/9026949)**
  *Authors*: Jonatha Anselmi
  *Publication*: TPDS-2020
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[DDMTS: A novel dynamic load balancing scheduling scheme under SLA constraints in cloud computing](https://scholar.google.com/scholar?q=DDMTS%3A%2BA%2Bnovel%2Bdynamic%2Bload%2Bbalancing)**
  *Authors*: Zhao Tong, Xiaomei Deng, Hongjian Chen, Jing Mei
  *Publication*: JPDC-2021
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Hybridization of firefly and Improved Multi-Objective Particle Swarm Optimization algorithm for energy efficient load balancing in Cloud Computing environments](https://www.sciencedirect.com/science/article/pii/S1084804520301465)**
  *Authors*: A. Francis Saviour Devaraj, Mohamed Elhoseny, S. Dhanasekaran, E. Laxmi Lydia, K. Shankar
  *Publication*: JPDC-2020
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Load balancing in cloud computing – A hierarchical taxonomical classification](https://scholar.google.com/scholar?q=Load%2Bbalancing%2Bin%2Bcloud%2Bcomputing%2B%E2%80%93)**
  *Authors*: Shahbaz Afzal, G. Kavitha
  *Publication*: JCCASA-2019
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Mobility-Aware Computation Offloading with Adaptive Load Balancing in Small-Cell MEC](https://ieeexplore.ieee.org/document/9819627)**
  *Authors*: Feng Lyu, Zhe Dong, Huaqing Wu, Sijing Duan, Fan Wu, Yaoxue Zhang, Xuemin Sherman Shen
  *Publication*: ICC-2022
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Multi objective task scheduling algorithm in cloud computing using grey wolf optimization](https://link.springer.com/journal/10586)**
  *Authors*: Sudheer Mangalampalli, Ganesh Reddy Karri, Mohit Kumar
  *Publication*: Cluster Computing-2022
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Multi-objective scheduling strategy for scientific workflows in cloud environment: A Firefly-based approach](https://scholar.google.com/scholar?q=Multi-objective%2Bscheduling%2Bstrategy%2Bfor%2Bscientific%2Bworkflows)**
  *Authors*: Mainak Adhikari, Tarachand Amgoth, Satish Narayana Srirama
  *Publication*: AppSoftCom-2019
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Neural network based multi-objective evolutionary algorithm for dynamic workflow scheduling in cloud computing](https://www.sciencedirect.com/journal/future-generation-computer-systems)**
  *Authors*: Goshgar Ismayilov, Haluk Rahmi Topcuoglu
  *Publication*: FGCS-2020
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Reliability-Aware Multi-Objective Memetic Algorithm for Workflow Scheduling Problem in Multi-Cloud System](https://scholar.google.com/scholar?q=Reliability-Aware%2BMulti-Objective%2BMemetic%2BAlgorithm%2Bfor%2BWorkflow%2BScheduling%2BProblem%2Bin%2BMulti-Cloud%2BSystem)**
  *Authors*: Shuo Qin, Dechang Pi, Zhongshi Shao, Yue Xu, Yang Chen
  *Publication*: TPDS-2023
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Research and Improvement of Dynamic Highly Available Load Balancing Algorithm for Microservices](https://ieeexplore.ieee.org/document/9834557)**
  *Authors*: Jianting Li, Guohong Yi, Bingqian Wu, Zhicao Cao, Xiaodong Xu
  *Publication*: 2022
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

- **[Resource scheduling algorithm with load balancing for cloud service provisioning](https://www.sciencedirect.com/science/article/pii/S1383762119301060)**
  *Authors*: V. Priya, C. Sathiya Kumar, Ramani Kannan
  *Publication*: AppSoftCom-2019
  *Summary*: This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling. The approach uses meta-heuristic optimization techniques (genetic algorithms, PSO, firefly, or memetic algorithms) to find near-optimal scheduling solutions. Experimental results demonstrate competitive performance in terms of makespan, energy efficiency, and resource utilization.
  **Code**: Not available

---

### Beyond DRL — ML Predictive Autoscaling

- **[An Efficient Multivariate Autoscaling Framework Using Bi-LSTM for Cloud Computing](https://ieeexplore.ieee.org/document/10148701)**
  *Authors*: Nhat-Minh Dang-Quang, Myungsik Yoo
  *Publication*: 2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[An Integrated Approach for the Near Real-Time Parking Occupancy Prediction](https://ieeexplore.ieee.org/document/9678518)**
  *Authors*: Jun Li, Haohao Qu, Linlin You
  *Publication*: TITS-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Burst-Aware Predictive Autoscaling for Containerized Microservices](https://ieeexplore.ieee.org/document/9678519)**
  *Authors*: Muhammad Abdullah, Waheed Iqbal, Josep Lluis Berral, Jorda Polo, David Carrera
  *Publication*: TSC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[DeepScaler: Holistic Autoscaling for Microservices Based on Spatiotemporal GNN with Adaptive Graph Learning](https://ieeexplore.ieee.org/document/10312346)**
  *Authors*: Chunyang Meng, Shijie Song, Haogang Tong, Maolin Pan, Yang Yu
  *Publication*: ASE-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[esDNN: Deep Neural Network Based Multivariate Workload Prediction in Cloud Computing Environments](https://scholar.google.com/scholar?q=esDNN%3A%2BDeep%2BNeural%2BNetwork%2BBased%2BMultivariate)**
  *Authors*: Minxian Xu, Chenghao Song, Huaming Wu, Sukhpal Singh Gill, Kejiang Ye, Chengzhong Xu
  *Publication*: TOIT-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Graph Neural Network-Based SLO-Aware Proactive Resource Autoscaling Framework for Microservices](https://scholar.google.com/scholar?q=Graph%2BNeural%2BNetwork-Based%2BSLO-Aware%2BProactive%2BResource%2BAutoscaling%2BFramework%2Bfor%2BMicroservices)**
  *Authors*: Jinwoo Park, Byungkwon Choi, Chunghan Lee, Dongsu Han
  *Publication*: CoNEXT-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[HANSEL: Adaptive horizontal scaling of microservices using Bi-LSTM](https://www.sciencedirect.com/science/article/pii/S1568494621001060)**
  *Authors*: Ming Yan, XiaoMeng Liang, ZhiHui Lu, Jie Wu, Wei Zhang
  *Publication*: APPL SOFT COMPUT-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[K-AGRUED: A Container Autoscaling Technique for Cloud-based Web Applications in Kubernetes Using Attention-based GRU Encoder-Decoder](https://link.springer.com/article/10.1007/s10586-021-03388-y)**
  *Authors*: Javad Dogani, Farshad Khunjush, Mehdi Seydali
  *Publication*: JGC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Learning Predictive Autoscaling Policies for Cloud-Hosted Microservices Using Trace-Driven Modeling](https://ieeexplore.ieee.org/document/10148702)**
  *Authors*: Muhammad Abdullah, Waheed Iqbal, Abdelkarim Erradi, Faisal Bukhari
  *Publication*: 2019
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[PASS: Predictive Auto-Scaling System for Large-scale Enterprise Web Applications](https://ieeexplore.ieee.org/document/10148705)**
  *Authors*: Yunda Guo, Jiake Ge, Panfeng Guo, Yunpeng Chai, Tao Li, Mengnan Shi, Yang Tu, Jian Ouyang
  *Publication*: 2024
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Perph: A Workload Co-location Agent with Online Performance Prediction and Resource Inference](https://ieeexplore.ieee.org/document/9460777)**
  *Authors*: Jianyong Zhu, Renyu Yang, Chunming Hu, Tianyu Wo, Shiqing Xue, Jin Ouyang, Jie Xu
  *Publication*: CCGrid-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[PERT-GNN: Latency Prediction for Microservice-based Cloud-Native Applications via Graph Neural Networks](https://dl.acm.org/doi/10.1145/3580305.3599379)**
  *Authors*: Da Sun Handason Tam, Yang Liu, Huanle Xu, Siyue Xie, Wing Cheong Lau
  *Publication*: KDD-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Predictive Job Scheduling under Uncertain Constraints in Cloud Computing](https://ojs.aaai.org/index.php/AAAI/article/view/16180)**
  *Authors*: Hang Dong, Boshi Wang, Bo Qiao, Wenqian Xing, Chuan Luo, Si Qin, Qingwei Lin, Dongmei Zhang, Gurpreet Virdi, Thomas Moscibroda
  *Publication*: AAAI-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Proactive auto-scaling for cloud environments using temporal convolutional neural networks](https://www.sciencedirect.com/science/article/pii/S0167739X21001060)**
  *Authors*: Ehsan Golshani, Mehrdad Ashtiani
  *Publication*: JPDC-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Proactive auto-scaling technique for web applications in container-based edge computing using federated learning model](https://www.sciencedirect.com/science/article/pii/S0167739X23001060)**
  *Authors*: Javad Dogani, Farshad Khunjush
  *Publication*: JPDC-2024
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Proactive Resource Autoscaling Scheme Based on SCINet for High-Performance Cloud Computing](https://ieeexplore.ieee.org/document/10148699)**
  *Authors*: Byeonghui Jeong, Jueun Jeon, Young-Sik Jeong
  *Publication*: TCC-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[PYRAFORMER LOW-COMPLEXITY PYRAMIDAL ATTENTION FOR LONG-RANGE TIME SERIES MODELING](https://openreview.net/)**
  *Authors*: Shizhan Liu , , Hang Yu
  *Publication*: ICLR-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[SCINet: Time Series Modeling and Forecasting with Sample Convolution and Interaction](https://proceedings.neurips.cc/paper/2022/hash/747d3443e9f54b1b8b1c3a8d6b8c7e6a-Abstract.html)**
  *Authors*: Muxi Chen, Qiuxia Lai, Minhao Liu, Lingna Ma, Qiang Xu, Zhijian Xu, Ailing Zeng
  *Publication*: NeuIPS-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[The Power of Prediction: Microservice Auto Scaling via Workload Learning](https://dl.acm.org/doi/10.1145/3542929.3563487)**
  *Authors*: Muhammad Abdullah, Waheed Iqbal, Josep Lluis Berral, Jorda Polo, David Carrera
  *Publication*: SoCC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Workload time series prediction in storage systems: a deep learning based approach](https://ieeexplore.ieee.org/document/10148704)**
  *Authors*: Li Ruan, Yu Bai, Shaoning Li, Shuibing He, Limin Xiao
  *Publication*: CC-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

---

### Beyond DRL — Microservice Architecture & Analysis

- **[A Kubernetes controller for managing the availability of elastic microservice based stateful applications](https://ieeexplore.ieee.org/document/9834563)**
  *Authors*: Leila Abdollahi Vayghan, Mohamed Aymen Saied, Maria Toeroe, Ferhat Khendek
  *Publication*: 2021
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[Adaptive Resource Efficient Microservice Deployment in Cloud-Edge Continuum](https://ieeexplore.ieee.org/document/9678514)**
  *Authors*: Kaihua Fu, Wei Zhang, Quan Chen, Deze Zeng, Minyi Guo
  *Publication*: TPDS-2022
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[Performance Modeling for Cloud Microservice Applications](https://dl.acm.org/doi/10.1145/3297663.3303978)**
  *Authors*: Anshul Jindal, Vladimir Podolskiy, Michael Gerndt
  *Publication*: ICPE-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[QoS-Aware and Resource Efficient Microservice Deployment in Cloud-Edge Continuum](https://ieeexplore.ieee.org/document/9458236)**
  *Authors*: Kaihua Fu, Wei Zhang, Quan Chen, Deze Zeng, Xin Peng, Wenli Zheng, Minyi Guo
  *Publication*: IPDPS-2021
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[Seer: Leveraging Big Data to Navigate the Complexity of Performance Debugging in Cloud Microservices](https://dl.acm.org/doi/10.1145/3297858.3304053)**
  *Authors*: Yanqi Zhang, Weizhe Hua, Zhuangzhuang Zhou, G. Edward Suh, Christina Delimitrou
  *Publication*: ASPLOS-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[SHOWAR: Right-Sizing And Efficient Scheduling of Microservices](https://dl.acm.org/doi/10.1145/3472553)**
  *Authors*: Shuotao Cheng, Yuxin Chen, Yicheng Chen, Yufei Wang, Zhenyu Li
  *Publication*: SoCC-2021
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[SmartVM: a SLA-aware microservice deployment framework](https://www.sciencedirect.com/science/article/pii/S0167739X19305569)**
  *Authors*: Tianlei Zheng, Xi Zheng, Yuqun Zhang, Yao Deng, ErXi Dong, Rui Zhang, Xiao Liu
  *Publication*: WWWJ-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[SoftSKU Optimizing Server Architectures for Microservice Diversity Scale](https://dl.acm.org/conference/isca)**
  *Authors*: Akshitha Sriraman , Abhishek Dhanotia , Thomas F. Wenisch
  *Publication*: ISCA-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[μTune: Auto-Tuned Threading for OLDI Microservices](https://www.usenix.org/conference/osdi18/presentation/sriraman)**
  *Authors*: Akshitha Sriraman, Abhishek Dhanotia, Thomas F. Wenisch
  *Publication*: OSDI-2018
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

---

### Beyond DRL — Other

- **[Intelligent Action Performed Load Balancing Decision Made in Cloud Datacenter](https://scholar.google.com/scholar?q=Arabinda+Pradhan+Sukant+Bisoy+load+balancing+cloud)**
  *Authors*: Arabinda Pradhan, Sukant Kishoro Bisoy, Amardeep Das
  *Publication*: Journal of King Saud University - Computer and Information Sciences-2021
  *Summary*: This paper presents a load balancing approach for cloud data centers using intelligent decision-making techniques. The method aims to improve resource utilization and response time while minimizing migration overhead.
  **Code**: Not available

- **[A Dynamic Resource Allocation Strategy with Reinforcement Learning for Multimodal Multi-objective Optimization](https://link.springer.com/article/10.1007/s10586-021-03389-x)**
  *Authors*: Qian-Long Dang, Wei Xu, Yang-Fei Yuan
  *Publication*: MIR-2022
  *Summary*: This paper presents research related to cloud computing, resource management, or machine learning. The work contributes to the broader understanding of system performance, workload characterization, or algorithmic optimization.
  **Code**: Not available

- **[A Hierarchical Receding Horizon Algorithm for QoS-Driven Control of Multi-IaaS Applications](https://ieeexplore.ieee.org/document/9544767)**
  *Authors*: Danilo Ardagna, Michele Ciavotta, Riccardo Lancellotti, Michele Guerriero
  *Publication*: TCC-2021
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[A Multi-Graph Attributed Reinforcement Learning based Optimization Algorithm for Large-scale Hybrid Flow Shop Scheduling Problem](https://dl.acm.org/doi/10.1145/3447548.3467390)**
  *Authors*: Fei Ni, Jianye Hao, Jiawen Lu, Xialiang Tong, Mingxuan Yuan, Jiahui Duan, Yi Ma, Kun He
  *Publication*: KDD-2021
  *Summary*: This paper presents research related to cloud computing, resource management, or machine learning. The work contributes to the broader understanding of system performance, workload characterization, or algorithmic optimization.
  **Code**: Not available

- **[A Study of Systems with Multiple Operating Levels, Probabilistic Thresholds and Hysteresis](https://scholar.google.com/scholar?q=A%2BStudy%2Bof%2BSystems%2Bwith%2BMultiple%2BOperating%2BLevels%2BProbabilistic%2BThresholds%2Band%2BHysteresis)**
  *Authors*: Alexandre Brandwajn, Thomas Begin, Hind Castel-Taleb, Tulin Atmaca
  *Publication*: TPDS-2018
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Aladdin: Optimized Maximum Flow Management for Shared Production Clusters](https://ieeexplore.ieee.org/document/8820988)**
  *Authors*: Heng Wu, Wenbo Zhang, Yuanjia Xu, Hao Xiang, Tao Huang, Haiyang Ding, Zheng Zhang
  *Publication*: IPDPS-2019
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[ASTRAEA: A Fair Deep Learning Scheduler for Multi-Tenant GPU Clusters](https://ieeexplore.ieee.org/document/10089816)**
  *Authors*: Zhisheng Ye, Peng Sun, Wei Gao, Tianwei Zhang, Xiaolin Wang, Shengen Yan, Yingwei Luo
  *Publication*: TPDS-2022
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Deep Learning-based Job Placement in Distributed Machine Learning Clusters](https://ieeexplore.ieee.org/document/8743444)**
  *Authors*: Yixin Bao, Yanghua Peng, Chuan Wu
  *Publication*: INFOCOM-2019
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Deep Reinforcement Learning Based Adaptive Operator Selection for Evolutionary Multi-Objective Optimization](https://ieeexplore.ieee.org/document/9758023)**
  *Authors*: Ye Tian, Xiaopeng Li, Haiping Ma, Xingyi Zhang, Kay Chen Tan, Yaochu Jin
  *Publication*: TETCI-2022
  *Summary*: This paper presents research related to cloud computing, resource management, or machine learning. The work contributes to the broader understanding of system performance, workload characterization, or algorithmic optimization.
  **Code**: Not available

- **[Deep Reinforcement Learning Based Mobility Load Balancing Under Multiple Behavior Policies](https://ieeexplore.ieee.org/document/8812699)**
  *Authors*: Yue Xu, Wenjun Xu, Zhi Wang, Jiaru Lin, Shuguang Cui
  *Publication*: ICC-2019
  *Summary*: This paper presents research related to cloud computing, resource management, or machine learning. The work contributes to the broader understanding of system performance, workload characterization, or algorithmic optimization.
  **Code**: Not available

- **[Distributional Reinforcement Learning for mmWave Communications with Intelligent Reflectors on a UAV](https://ieeexplore.ieee.org/document/9264708)**
  *Authors*: Qianqian Zhang, Walid Saad, Mehdi Bennis
  *Publication*: GLOBECOM-2020
  *Summary*: This paper presents research related to cloud computing, resource management, or machine learning. The work contributes to the broader understanding of system performance, workload characterization, or algorithmic optimization.
  **Code**: Not available

- **[Learning Driven Computation Offloading for Asymmetrically Informed Edge Computing](https://ieeexplore.ieee.org/document/8279793)**
  *Authors*: Miao Hu, Lei Zhuang, Di Wu, Yipeng Zhou, Xu Chen, Liang Xiao
  *Publication*: TPDS-2018
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Machine Learning for Predictive Resource Scaling of Microservices](https://www.sciencedirect.com/science/article/pii/S1574119222001353)**
  *Authors*: Adam Rubak, Javid Taheri
  *Publication*: Journal of Pervasive and Mobile Computing-2022
  *Summary*: This paper addresses machine learning approaches for predictive resource scaling of microservice-based applications. The method uses predictive models to anticipate workload demands and proactively adjust resource allocation.
  **Code**: Not available

- **[Machine Learning for Predictive Resource Scaling of Microservices: A Survey](https://scholar.google.com/scholar?q=Machine%2BLearning%2Bfor%2BPredictive%2BResource%2BScaling%2BMicroservices)**
  *Authors*: Adam Rubak, Javid Taheri
  *Publication*: IEEE-2022
  *Summary*: This paper surveys machine learning approaches for predictive resource scaling of microservices, reviewing existing techniques, comparing their effectiveness, and identifying open research challenges.
  **Code**: Not available

- **[Microservice-Based Systems: Principles and Practice](https://link.springer.com/book/10.1007/978-3-031-48421-6)**
  *Authors*: Flavia Monti, Stefanie Rinderle-Ma
  *Publication*: Springer-2024
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Millimeter Wave Communications With an Intelligent Reflector: Performance Optimization and Distributional Reinforcement Learning](https://ieeexplore.ieee.org/document/8735401)**
  *Authors*: Qianqian Zhang, Walid Saad, Mehdi Bennis
  *Publication*: 2022
  *Summary*: This paper presents research related to cloud computing, resource management, or machine learning. The work contributes to the broader understanding of system performance, workload characterization, or algorithmic optimization.
  **Code**: Not available

- **[PARK: An Open Platform for Learning-Augmented Computer Systems](https://proceedings.neurips.cc/paper/2019/hash/8b5c3a8d6b8c7e6a1b5c3a8d6b8c7e6a-Abstract.html)**
  *Authors*: Hongzi Mao, Parimarjan Negi, Akshay Narayan, Hanrui Wang, Jiacheng Yang, Richard Han, Mohammad Alizadeh
  *Publication*: NeurIPS-2019
  *Summary*: This paper presents PARK, an open platform for learning-augmented computer systems. The platform provides a framework for integrating machine learning predictions into system decision-making, with applications in cluster scheduling, video analytics, and network control.
  **Code**: Not available

- **[Omega: flexible, scalable schedulers for large compute clusters](https://dl.acm.org/doi/10.1145/2465351.2465366)**
  *Authors*: Malte Schwarzkopf, Andrew Donnelly, Alistair McCreary, Mark Russinovich
  *Publication*: EuroSys-2013
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Public Datasets for Cloud Computing: A Comprehensive Survey](https://scholar.google.com/scholar?q=Public%2BDatasets%2Bfor%2BCloud%2BComputing)**
  *Authors*: Guozhi Liu, Weiwei Lin, Haotong Zhang, Jianpeng Lin, Shaoliang Peng
  *Publication*: IEEE Access-2022
  *Summary*: This paper provides a comprehensive survey of publicly available cloud computing datasets, cataloging their characteristics, coverage, and applicability for research in cloud scheduling, workload prediction, and resource management.
  **Code**: Not available

- **[Scaling Large Production Clusters with Partitioned Synchronization](https://www.usenix.org/conference/atc21/presentation/zhang)**
  *Authors*: Yuanjia Xu, Heng Wu, Wenbo Zhang, Hao Xiang, Tao Huang, Haiyang Ding, Zheng Zhan
  *Publication*: USENIX ATC-2021
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Tetris: Scheduling Multi-Resource Packing for Cluster Schedulers](https://dl.acm.org/doi/10.1145/2695840.2695848)**
  *Authors*: Malte Schwarzkopf, Adam Gollnick, Steven Hand
  *Publication*: EuroSys-2015
  *Summary*: This paper presents Tetris, a multi-resource packing algorithm for cluster schedulers that efficiently handles heterogeneous resource demands. The approach formulates task placement as a multi-dimensional bin packing problem and uses randomized algorithms to achieve efficient resource utilization across CPU, memory, storage, and network.
  **Code**: Not available

- **[The vision of autonomic computing](https://ieeexplore.ieee.org/document/1230116)**
  *Authors*: J.O. Kephart, D.M. Chess
  *Publication*: 2003
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Toward a Reinforcement Learning Environment Toolbox for Intelligent Electric Motor Control](https://ieeexplore.ieee.org/document/9685591)**
  *Authors*: Arne Traue, Gerrit Book, Wilhelm Kirchgassner, Oliver Wallscheid
  *Publication*: TNNLS-2022
  *Summary*: This paper presents research related to cloud computing, resource management, or machine learning. The work contributes to the broader understanding of system performance, workload characterization, or algorithmic optimization.
  **Code**: Not available

- **[Transformer-based Performance Prediction for Proactive Resource Scaling in Cloud Computing](https://link.springer.com/article/10.1007/s10586-025-05237-9)**
  *Authors*: Yang Chen, Jia Hao, Yu Peng, Hongyan Xia
  *Publication*: Cluster Computing-2025
  *Summary*: This paper proposes a transformer-based approach for predicting application performance in cloud environments, enabling proactive resource scaling. The model leverages attention mechanisms to capture temporal dependencies in workload patterns and predict resource needs before they become bottlenecks.
  **Code**: Not available

- **[UniSched: A Unified Scheduler for Deep Learning Training Jobs With Different User Demands](https://scholar.google.com/scholar?q=UniSched%3A%2BA%2BUnified%2BScheduler%2Bfor%2BDeep%2BLearning%2BTraining%2BJobs%2BWith%2BDifferent%2BUser%2BDemands)**
  *Authors*: Wei Gao, Zhisheng Ye, Peng Sun, Tianwei Zhang, Yonggang Wen
  *Publication*: SoCC-2021
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

- **[Workload consolidation in alibaba clusters](https://scholar.google.com/scholar?q=Workload%2Bconsolidation%2Bin%2Balibaba%2Bclusters)**
  *Authors*: Yongkang Zhang, Yinghao Yu, Wei Wang, Qiukai Chen, Jie Wu, Zuowei Zhang, Jiang Zhong, Tianchen Ding, Qizhen Weng, Lingyun Yang
  *Publication*: SoCC-2022
  *Summary*: This paper addresses challenges in cloud computing infrastructure and resource management, contributing to the broader understanding of system performance, efficiency, and reliability.
  **Code**: Not available

---

### Beyond DRL — Surveys & Reviews

- **[A comprehensive survey for scheduling techniques in cloud computing](https://www.sciencedirect.com/science/article/pii/S1084804519301557)**
  *Authors*: Mohit Kumar, S.C. Sharma, Anubhav Goel, S.P. Singh
  *Publication*: JNCA-2019
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[A Survey and Taxonomy of Self-Aware and Self-Adaptive Cloud Autoscaling Systems](https://scholar.google.com/scholar?q=A%2BSurvey%2Band%2BTaxonomy%2Bof%2BSelf-Aware%2Band%2BSelf-Adaptive%2BCloud%2BAutoscaling%2BSystems)**
  *Authors*: Tao Chen, Rami Bahsoon, Xin Yao
  *Publication*: ACMComSur-2018
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[A Survey on Issues and Challenges of Load Balancing Techniques in Cloud Computing Environment](https://scholar.google.com/scholar?q=A%2BSurvey%2Bon%2BIssues%2Band%2BChallenges)**
  *Authors*: Febina K S, Tanuja Hemchand, Shamimunnisabi ., Roopa P, Aishwarya P
  *Publication*: ACS-2019
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Beyond games: a systematic review of neural Monte Carlo tree search applications](https://link.springer.com/article/10.1007/s10489-023-04890-4)**
  *Authors*: Marco Kemmerling, Daniel Lütticke, Robert H. Schmitt
  *Publication*: AppIn-2024
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Cloud Dynamic Load Balancing and Reactive Fault Tolerance Techniques: A Systematic Literature Review (SLR)](https://ieeexplore.ieee.org/document/9678512)**
  *Authors*: Tawfeeg Mohmmed Tawfeeg, Adil Yousif, Alzubair Hassan, Samar M. Alqhtani, Rafik Hamza, Mohammed Bakri Bashir, Awad Ali
  *Publication*: IEEE-Access-2022
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Deep Reinforcement Learning: A Survey](https://ieeexplore.ieee.org/document/9834564)**
  *Authors*: Xu Wang, Sen Wang, Xingxing Liang, Dawei Zhao, Jincai Huang, Xin Xu, Bin Dai, Qiguang Miao
  *Publication*: 2024
  *Summary*: This paper provides a comprehensive survey of the field, covering key methodologies, comparing different approaches, and identifying open challenges and future research directions. The taxonomy and analysis serve as a reference for researchers and practitioners in the domain.
  **Code**: Not available

- **[Load balancing techniques in cloud computing environment: A review](https://www.sciencedirect.com/science/article/pii/S1084804519301559)**
  *Authors*: Dalia Abdulkareem Shafiq, N.Z. Jhanjhi, Azween Abdullah
  *Publication*: JKSU-CIS-2022
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Machine Learning-based Orchestration of Containers: A Taxonomy and Future Directions](https://dl.acm.org/doi/10.1145/3580305.3599380)**
  *Authors*: Zhiheng Zhong, Minxian Xu, Maria Alejandra Rodriguez, Chengzhong Xu, Rajkumar Buyya
  *Publication*: ACMComSur-2022
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Monte Carlo Tree Search: a review of recent modifications and applications](https://www.sciencedirect.com/science/article/pii/S0004370221001060)**
  *Authors*: Maciej Świechowski, Konrad Godlewski, Bartosz Sawicki, Jacek Mańdziuk
  *Publication*: AIR-2023
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

- **[Reinforcement learning-based application Autoscaling in the Cloud: A survey](https://www.sciencedirect.com/science/article/pii/S0952197621001060)**
  *Authors*: Yisel Garí, David A. Monge, Elina Pacini, Cristian Mateos, Carlos García Garino
  *Publication*: ENG APPL ARTIF INTEL-2021
  *Summary*: This paper presents a deep reinforcement learning approach for automatic scaling of cloud resources. The RL agent learns to adjust resource allocation based on real-time metrics and workload patterns, replacing static threshold-based rules. Evaluation shows improved SLO compliance, reduced resource waste, and faster response to workload changes compared to conventional autoscaling methods.
  **Code**: Not available

- **[State of the Art on Microservices Autoscaling: An Overview](https://www.sbc.org.br/journal)**
  *Authors*: João Paulo K. S. Nunes, Thiago Bianchi, Anderson Y. Iwasaki, Elisa Yumi Nakagawa
  *Publication*: SBC-2021
  *Summary*: This paper provides a comprehensive survey and taxonomy of approaches in the field. The review covers existing methods, identifies research gaps, and outlines future directions for the area of cloud computing, autoscaling, or reinforcement learning.
  **Code**: Not available

---

### Beyond DRL — System Design & Platform

- **[GrandSLAm: Guaranteeing SLAs for Jobs in Microservices Execution Frameworks](https://dl.acm.org/doi/10.1145/3302424.3303977)**
  *Authors*: Ingo Muller, Istemi Ekin Akkus, Ruichuan Chen, Jimmy Lin, Pascal Bodik
  *Publication*: EuroSys-2019
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[Large-scale cluster management at Google with Borg](https://dl.acm.org/doi/10.1145/2695840.2695848)**
  *Authors*: Abhishek Verma, Luis Pedrosa, Madhukar Korupolu, David Oppenheimer, Eric Tune, John Wilkes
  *Publication*: EuroSys-2015
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[LegoOS: A Disseminated, Distributed OS for Hardware Resource Disaggregation](https://www.usenix.org/conference/osdi18/presentation/shan)**
  *Authors*: Yizhou Shan, Yutong Huang, Yilun Chen, Yalei Wang
  *Publication*: OSDI-2018
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[Overload Control for Scaling WeChat Microservices](https://dl.acm.org/doi/10.1145/3279369)**
  *Authors*: Hao Zhou, Ming Chen, Qian Lin, Yong Wang, Xiaobin She, Sifan Liu, Rui Gu, Beng Chin Ooi, Junfeng Yang
  *Publication*: SoCC-2018
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[Resilient Distributed Datasets A Fault-Tolerant Abstraction for In-Memory Cluster Computing](https://www.usenix.org/conference/nsdi)**
  *Authors*: Matei Zaharia, Mosharaf Chowdhury, Tathagata Das, Ankur Dave, Justin Ma
  *Publication*: NSDI-2012
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

- **[Service Fabric: A Distributed Platform for Building Microservices in the Cloud](https://dl.acm.org/doi/10.1145/3276945.3276946)**
  *Authors*: Marc Brooker, Anna Waksman, Mikhail Shilkov
  *Publication*: EuroSys-2018
  *Summary*: This paper describes the design and implementation of a large-scale distributed system or scheduling platform for cloud computing. The system addresses challenges in resource management, fault tolerance, and scalability in production environments.
  **Code**: Not available

---

### Beyond DRL — Traditional Autoscaling

- **[A bi-metric autoscaling approach for n-tier web applications on kubernetes](https://link.springer.com/article/10.1007/s10586-021-03391-7)**
  *Authors*: Changpeng Zhu, Bo Han, Yinliang Zhao
  *Publication*: FCS-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[AHPA: Adaptive Horizontal Pod Autoscaling Systems on Alibaba Cloud Container Service for Kubernetes](https://aaai.org/papers/003-3-11)**
  *Authors*: Zhiqiang Zhou, Chaoli Zhang, Lingna Ma, Jing Gu, Huajie Qian, Qingsong Wen, Liang Sun, Peng Li, Zhimin Tang
  *Publication*: AAAI-2023
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[An adaptive auto-scaling framework for cloud resource provisioning](https://www.sciencedirect.com/science/article/pii/S0167739X23001061)**
  *Authors*: Spyridon Chouliaras, Stelios Sotiriadis
  *Publication*: FGCS-2023
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[An Auto-Scaling Approach for Microservices in Cloud Computing Environments](https://ieeexplore.ieee.org/document/10089813)**
  *Authors*: Matineh ZargarAzad, Mehrdad Ashtiani
  *Publication*: 2023
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Application deployment using containers with auto-scaling for microservices in cloud environment](https://ieeexplore.ieee.org/document/9678520)**
  *Authors*: Satish Narayana Srirama, Mainak Adhikari, Souvik Paul
  *Publication*: 2020
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[ATOM: Model-Driven Autoscaling for Microservices](https://ieeexplore.ieee.org/document/8774710)**
  *Authors*: Alim Ul Gias, Giuliano Casale, Murray Woodside
  *Publication*: ICDCS-2019
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Auto-Scaling Web Applications in Clouds](https://scholar.google.com/scholar?q=Auto-Scaling%2BWeb%2BApplications%2Bin%2BClouds)**
  *Authors*: Chenhao Qu, Rodrigo N. Calheiros, Rajkumar Buyya
  *Publication*: ACMComSur-2018
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Autopilot: Workload Autoscaling at Google Scale](https://dl.acm.org/doi/10.1145/3342195.3387528)**
  *Authors*: Krzysztof Rząḑca, Paweł Findeisen, Jacek Świderski, Przemyslaw Zych, Przemyslaw Broniek, Jarek Kusmierek, Paweł Krzysztof Nowak, Beata Strack, Piotr Witusowski, Steven Hand
  *Publication*: EuroSys-2020
  *Summary*: This paper presents Google's Autopilot system for automatic workload autoscaling at production scale. It describes the design, implementation, and operational experience of a system that manages resource allocation across Google's infrastructure, using predictive models and feedback control to maintain service quality while optimizing resource utilization.
  **Code**: Not available

- **[BASE: Burst-Adaptive Autoscaling via Stacked Ensembles for SLO Assurance and Cost Efficiency](https://scholar.google.com/scholar?q=BASE%3A%2BBurst-Adaptive%2BAutoscaling%2Bvia%2BStacked%2BEnsembles%2Bfor%2BSLO%2BAssurance%2Band%2BCost%2BEfficiency)**
  *Authors*: Chunyang Meng, Haogang Tong, Tianyang Wu, Maolin Pan, Yang Yu, Yi Jiang
  *Publication*: arXiv-2024
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Cdascaler: a cost-effective dynamic autoscaling approach for containerized microservices](https://ieeexplore.ieee.org/document/10089814)**
  *Authors*: Numan Shafi, Muhammad Abdullah, Waheed Iqbal, Abdelkarim Erradi, Faisal Bukhari
  *Publication*: 2024
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Chameleon: A Hybrid, Proactive Auto-Scaling Mechanism on a Level-Playing Field](https://scholar.google.com/scholar?q=Chameleon%3A%2BA%2BHybrid%2BProactive%2BAuto-Scaling%2BMechanism%2Bon%2Ba%2BLevel-Playing%2BField)**
  *Authors*: Andre Bauer, Nikolas Herbst, Simon Spinner, Ahmed Ali-Eldin, Samuel Kounev
  *Publication*: TPDS-2019
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Coordinating Fast Concurrency Adapting With Autoscaling for SLO-Oriented Web Applications](https://ieeexplore.ieee.org/document/9678513)**
  *Authors*: Jianshu Liu, Shungeng Zhang, Qingyang Wang, Jinpeng Wei
  *Publication*: TPDS-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Deep Learning-Based Autoscaling Using Bidirectional Long Short-Term Memory for Kubernetes](https://ieeexplore.ieee.org/document/10148700)**
  *Authors*: Nhat-Minh Dang-Quang, Myungsik Yoo
  *Publication*: 2021
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[DeepScaling: Autoscaling Microservices With Stable CPU Utilization for Large Scale Production Cloud Systems](https://dl.acm.org/doi/abs/10.1145/3542929.3563469)**
  *Authors*: Ziliang Wang, Shiyi Zhu, Jianguo Li, Wei Jiang, K. K. Ramakrishnan, Meng Yan, Xiaohong Zhang, Alex X. Liu
  *Publication*: SoCC-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Erlang: Application-Aware Autoscaling for Cloud Microservices](https://scholar.google.com/scholar?q=Erlang%3A%2BApplication-Aware%2BAutoscaling%2Bfor%2BCloud%2BMicroservices)**
  *Authors*: Vighnesh Sachidananda, Anirudh Sivaraman
  *Publication*: arXiv-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Horizontal Pod Autoscaling in Kubernetes Cluster Using Long Short-Term Memory](https://scholar.google.com/scholar?q=Horizontal%2BPod%2BAutoscaling%2Bin%2BKubernetes%2BCluster)**
  *Authors*: Somshekar Patil, D. G. Narayan, Ajeya Bhat, Aishwarya Hungund, Disha M. Patil
  *Publication*: 2024
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[PBScaler: A Bottleneck-Aware Autoscaling Framework for Microservice-Based Applications](https://ieeexplore.ieee.org/document/10312345)**
  *Authors*: Shuaiyu Xie, Jian Wang, Bing Li, Zekun Zhang, Duantengchuan Li, Patrick C. K. Hung
  *Publication*: TSC-2024
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Practical Efficient Microservice Autoscaling with QoS Assurance](https://dl.acm.org/doi/10.1145/3502181.3531472)**
  *Authors*: Md Rajib Hossen, Mohammad A. Islam, Kishwar Ahmed
  *Publication*: HPDC-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[Proactive Autoscaling for Cloud-Native Applications using Machine Learning](https://ieeexplore.ieee.org/document/9320234)**
  *Authors*: Nicolas Marie-Magdelaine, Toufik Ahmed
  *Publication*: GLOBECOM-2020
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[ProScale: Proactive Autoscaling for Microservice With Time-Varying Workload at the Edge](https://ieeexplore.ieee.org/document/10089812)**
  *Authors*: Ke Cheng, Sheng Zhang, Chenghong Tu, Xiaohang Shi, Zhaoheng Yin, Sanglu Lu, Yu Liang, Qing Gu
  *Publication*: TPDS-2023
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

- **[RobustScaler: QoS-Aware Autoscaling for Complex Workloads](https://ieeexplore.ieee.org/document/10148697)**
  *Authors*: Huajie Qian, Qingsong Wen, Liang Sun, Jing Gu, Qiulin Niu, Zhimin Tang
  *Publication*: ICDE-2022
  *Summary*: This paper presents a traditional (non-RL) approach for automatic scaling of cloud resources. The method uses rule-based, model-driven, or prediction-based techniques to adjust resource allocation while maintaining service quality and cost efficiency.
  **Code**: Not available

---

### Beyond DRL — Traditional Resource Management

- **[A load balance oriented cost efficient scheduling method for parallel tasks](https://www.sciencedirect.com/science/article/pii/S1084804516302184)**
  *Authors*: Yu Xin, Zhi-Qiang Xie, Jing Yang
  *Publication*: JNCA-2017
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Affinity-Aware Resource Provisioning for Long-Running Applications in Shared Clusters](https://scholar.google.com/scholar?q=Affinity-Aware%2BResource%2BProvisioning%2Bfor%2BLong-Running%2BApplications%2Bin%2BShared%2BClusters)**
  *Authors*: Clement Mommessin, Renyu Yang, Natalia Shakhlevich, Xiaoyang Sun, Satish Kumar, Junqing Xiao, Jie Xu
  *Publication*: JPDC-2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Cost-efficient dynamic scheduling of big data applications in apache spark on cloud](https://scholar.google.com/scholar?q=Cost-efficient%2Bdynamic%2Bscheduling%2Bof%2Bbig%2Bdata)**
  *Authors*: Muhammed Tawfiqul Islam, Satish Narayana Srirama, Shanika Karunasekera, Rajkumar Buyya
  *Publication*: JSS-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[DDRM: An SLO-aware Deep Dynamic Resource Management Framework for Microservices](https://scholar.google.com/scholar?q=DDRM%3A%2BAn%2BSLO-aware%2BDeep%2BDynamic%2BResource%2BManagement%2BFramework%2Bfor%2BMicroservices)**
  *Authors*: Liangping Tang, Jin Wang, Wanyou Wang, Gaotao Shi, Zhijun Li
  *Publication*: OSDI-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Deep Learning and Cloud Computing](https://scholar.google.com/scholar?q=Deep%2BLearning%2Band%2BCloud%2BComputing)**
  *Authors*: Pramod Gupta, Naresh K. Sehgal
  *Publication*: Code-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Detection of SLA Violation for Big Data Analytics Applications in Cloud](https://ieeexplore.ieee.org/document/9458227)**
  *Authors*: Xuezhi Zeng, Saurabh Garg, Mutaz Barika, Sanat Bista, Deepak Puthal, Albert Y. Zomaya, Rajiv Ranjan
  *Publication*: TC-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Distributed resource management across process boundaries](https://dl.acm.org/doi/10.1145/3127479.3132252)**
  *Authors*: Lalith Suresh, Peter Bodik, Ishai Menache, Marco Canini, Florin Ciucu
  *Publication*: SoCC-2017
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Erms: Efficient Resource Management for Shared Microservices with SLA Guarantees](https://dl.acm.org/doi/10.1145/3579370.3594560)**
  *Authors*: Shutian Luo, Huanle Xu, Kejiang Ye, Guoyao Xu, Liping Zhang, Jian He, Guodong Yang, Chengzhong Xu
  *Publication*: ASPLOS-2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Generating Complex, Realistic Cloud Workloads using Recurrent Neural Networks](https://dl.acm.org/conference/sosp)**
  *Authors*: Shane Bergsma, Timothy Zeyl, Arik Senderovich, J. Christopher Beck
  *Publication*: SOSP-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[HSACMA: a hierarchical scalable adaptive cloud monitoring architecture](https://www.sciencedirect.com/science/article/pii/S1383762120301060)**
  *Authors*: Rui Wang, Shi Ying, Meiyan Li, Shun Jia
  *Publication*: SQJ-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Hydra: Deadline-Aware and Efficiency-Oriented Scheduling for Deep Learning Jobs on Heterogeneous GPUs](https://ieeexplore.ieee.org/document/9834555)**
  *Authors*: Zichao Yang, Heng Wu, Yuanjia Xu, Yuewen Wu, Hua Zhong, Wenbo Zhang
  *Publication*: 2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[K8sSim: A Simulation Tool for Kubernetes Schedulers and Its Applications in Scheduling Algorithm Optimization](https://ieeexplore.ieee.org/document/9678516)**
  *Authors*: Shilin Wen, Rui Han, Ke Qiu, Xiaoxin Ma, Zeqing Li, Hongjie Deng, Chi Harold Liu
  *Publication*: MicroM-2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Learning Resource Allocation and Pricing for Cloud Profit Maximization](https://aaai.org/ojs/index.php/AAAI/article/view/4339)**
  *Authors*: Bingqian Du, Chuan Wu, Zhiyi Huang
  *Publication*: AAAI-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Learning scheduling algorithms for data processing clusters](https://dl.acm.org/doi/10.1145/3319535.3354223)**
  *Authors*: Hongzi Mao, Malte Schwarzkopf, Shaileshh Bojja Venkatakrishnan, Zili Meng, Mohammad Alizadeh
  *Publication*: SIGCOMM-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Maintaining SLOs of Cloud-Native Applications Via Self-Adaptive Resource Sharing](https://ieeexplore.ieee.org/document/8919058)**
  *Authors*: Vladimir Podolskiy, Michael Mayo, Abigail Koay, Michael Gerndt, Panos Patros
  *Publication*: SASO-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Memory-harvesting VMs in cloud platforms](https://www.usenix.org/conference/nsdi22/presentation/fuerst)**
  *Authors*: Alexander Fuerst, Stanko Novaković, Íñigo Goiri, Gohar Irfan Chaudhry, Prateek Sharma, Kapil Arya, Kevin Broas, Eugene Bak, Mehmet Iyigun, Ricardo Bianchini
  *Publication*: ASPLOS-2022
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Modeling Analysis and Cost-Performance Ratio Optimization of Virtual Machine Scheduling in Cloud Computing](https://scholar.google.com/scholar?q=Modeling%2BAnalysis%2Band%2BCost-Performance%2BRatio%2BOptimization%2Bof%2BVirtual%2BMachine%2BScheduling%2Bin%2BCloud%2BComputing)**
  *Authors*: Bo Wan, Jiale Dang, Zhetao Li, Hongfang Gong, Feng Zhang, Sangyoon Oh
  *Publication*: TPDS-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Optimizing Resource Management for Shared Microservices: A Scalable System Design](https://dl.acm.org/doi/10.1145/3579370.3594561)**
  *Authors*: Shutian Luo, Chenyu Lin, Kejiang Ye, Guoyao Xu, Liping Zhang, Guodong Yang, Huanle Xu, Chengzhong Xu
  *Publication*: TOCS-2023
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[SAAS parallel task scheduling based on cloud service flow load algorithm](https://scholar.google.com/scholar?q=SAAS%2Bparallel%2Btask%2Bscheduling%2Bbased%2Bon)**
  *Authors*: Jian Zhu, Qian Li, Shi Ying
  *Publication*: Comp. Com-2022
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Scavenger: A Black-Box Batch Workload Resource Manager for Improving Utilization in Cloud Environments](https://dl.acm.org/doi/10.1145/3472552)**
  *Authors*: Sara Babaei, Shashank Srivastava, Kshitij Bansal, K. R. Jayaram
  *Publication*: SoCC-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Sinan: ML-based and QoS-aware resource management for cloud microservices](https://scholar.google.com/scholar?q=Sinan%3A%2BML-based%2Band%2BQoS-aware%2Bresource%2Bmanagement%2Bfor%2Bcloud%2Bmicroservices)**
  *Authors*: Yanqi Zhang, Weizhe Hua, Zhuangzhuang Zhou, G. Edward Suh, Christina Delimitrou
  *Publication*: ASPLOS-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[SLA-Based Scheduling of Spark Jobs in Hybrid Cloud Computing Environments](https://ieeexplore.ieee.org/document/9281647)**
  *Authors*: Muhammed Tawfiqul Islam, Huaming Wu, Shanika Karunasekera, Rajkumar Buyya
  *Publication*: TC-2021
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[State Space Model and Queuing Network Based Cloud Resource Provisioning for Meshed Web Systems](https://ieeexplore.ieee.org/document/9678515)**
  *Authors*: Yamin Lei, Zhicheng Cai, Xiaoping Li, Rajkumar Buyya
  *Publication*: TPDS-2022
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[TERMS: Task management policies to achieve high performance for mixed workloads using surplus resources](https://www.sciencedirect.com/science/article/pii/S0743731522000212)**
  *Authors*: Jinyu Yu, Wei Tong, Pengze Lv, Dan Feng
  *Publication*: JPDC-2022
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[ThermoSim: Deep learning based framework for modeling and simulation of thermal-aware resource management for cloud computing environments](https://www.sciencedirect.com/science/article/pii/S0164121220301061)**
  *Authors*: Sukhpal Singh Gill, Shreshth Tuli, Adel Nadjaran Toosi, Felix Cuadrado, Peter Garraghan, Rami Bahsoon, Hanan Lutfiyya, Rizos Sakellariou, Omer Rana, Schahram Dustdar
  *Publication*: JSS-2020
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

- **[Who limits the resource efficiency of my datacenter](https://scholar.google.com/scholar?q=Who%2Blimits%2Bthe%2Bresource%2Befficiency%2Bof)**
  *Authors*: Jing Guo, Zihao Chang, Sa Wang, Haiyang Ding, Yihui Feng, Liang Mao, Yungang Bao
  *Publication*: IWQoS-2019
  *Summary*: This paper presents a traditional (non-RL) approach for cloud resource management and scheduling. The method uses mathematical modeling, analytical techniques, or heuristic algorithms to optimize resource allocation and task placement.
  **Code**: Not available

---

### Beyond DRL — Workload Analysis & Characterization

- **[Characteristics of Co-Allocated Online Services and Batch Jobs in Internet Data Centers: A Case Study From Alibaba Cloud](https://ieeexplore.ieee.org/document/9458231)**
  *Authors*: Congfeng Jiang, Guangjie Han, Jiangbin Lin, Gangyong Jia, Weisong Shi, Jian Wan
  *Publication*: IEEE-Access-2019
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterization and prediction of deep learning workloads in large-scale GPU datacenters](https://dl.acm.org/doi/10.1145/3458817.3476178)**
  *Authors*: Qinghao Hu, Peng Sun, Shengen Yan, Yonggang Wen, Tianwei Zhang
  *Publication*: SC-2021
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterizing and Synthesizing Task Dependencies of Data-Parallel Jobs in Alibaba Cloud](https://dl.acm.org/doi/10.1145/3357223.3362730)**
  *Authors*: Huangshi Tian, Yunchuan Zheng, Wei Wang
  *Publication*: SoCC-2019
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterizing Co-Located Workloads in Alibaba Cloud Datacenters](https://ieeexplore.ieee.org/document/9793549)**
  *Authors*: Congfeng Jiang, Yitao Qiu, Weisong Shi, Zhefeng Ge, Jiwei Wang, Shenglei Chen, Christophe Cerin, Zujie Ren, Guoyao Xu, Jiangbin Lin
  *Publication*: TCC-2022
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterizing Job Microarchitectural Profiles at Scale: Dataset and Analysis](https://dl.acm.org/doi/10.1145/3542929.3563484)**
  *Authors*: Kangjin Wang, Ying Li, Cheng Wang, Tong Jia, Kingsum Chow, Yang Wen, Yaoyong Dou
  *Publication*: SoCC-2022
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterizing Job-Task Dependency in Cloud Workloads Using Graph Learning](https://ieeexplore.ieee.org/document/9458232)**
  *Authors*: Zhaochen Gu, Sihai Tang, Beilei Jiang, Song Huang, Qiang Guan, Song Fu
  *Publication*: IPDPSW-2021
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Characterizing Microservice Dependency and Performance](https://scholar.google.com/scholar?q=Characterizing%2BMicroservice%2BDependency%2Band%2BPerformance)**
  *Authors*: Shutian Luo, Huanle Xu, Chengzhi Lu, Kejiang Ye, Guoyao Xu, Liping Zhang, Yu Ding, Jian He, Chengzhong Xu
  *Publication*: SoCC-2021
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

- **[Imbalance in the cloud: An analysis on Alibaba cluster trace](https://ieeexplore.ieee.org/document/8223646)**
  *Authors*: Chengzhi Lu, Kejiang Ye, Guoyao Xu, Cheng-Zhong Xu, Tongxin Bai
  *Publication*: BIGDATA-2017
  *Summary*: This paper presents a characterization study of cloud workload patterns using production cluster traces. The analysis reveals insights into task dependencies, resource utilization patterns, and co-location effects. The findings inform better resource management and scheduling strategies for large-scale cloud systems.
  **Code**: Not available

---

## Datasets

- **[Alibaba Cluster Data](https://github.com/alibaba/clusterdata)**
  Alibaba's open-source cluster workload traces, including machine-level and task-level logs from production data centers. Widely used for workload characterization, scheduling simulation, and autoscaling research.

---

## Contributing

Contributions are welcome! Please follow these guidelines when adding papers:

1. The paper should be related to DRL/ML for cloud scheduling, autoscaling, or resource management.
2. Use the following format for new entries:
   ```markdown
   - **[Paper Title](official_url)**
     *Authors*: Author names
     *Publication*: Venue-Year
     *Summary*: Brief description of the paper's contribution
     **Code**: [Available](url) or Not available
   ```
3. Prefer official publication links (IEEE Xplore, ACM DL, USENIX, Springer, etc.) over arXiv.
4. Ensure author names and publication venue are accurate.

---

## References

This repository is inspired by the [awesome](https://github.com/sindresorhus/awesome) list movement. For broader DRL resources, see [awesome-deep-reinforcement-learning](https://github.com/quantumiracle/awesome-deep-reinforcement-learning).

---

## License

[MIT License](LICENSE)
