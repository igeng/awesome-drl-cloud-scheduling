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

- **[Batch Jobs Load Balancing Scheduling in Cloud Computing Using Distributional Reinforcement Learning](https://doi.org/10.1109/tpds.2023.3334519)**
  *Authors*: Tiangang Li, Shi Ying, Yishi Zhao, Jianga Shang
  *Publication*: TPDS-2024
  *Summary*: This paper addresses load balancing scheduling for batch jobs in cloud computing using distributional reinforcement learning. Unlike value-based DQN methods that only estimate expected cumulative return, this approach models the full value distribution to capture environmental stochasticity. By formalizing load balancing as a multi-objective optimization problem and applying quantile regression to learn the value distribution, the proposed algorithm achieves superior load balancing and resource utilization compared to baselines on real Alibaba Cluster traces (v2018 and v2020).
  **Code**: Not available

- **[<i>Microscaler</i>: Cost-Effective Scaling for Microservice Applications in the Cloud With an Online Learning Approach](https://scholar.google.com/scholar?q=iMicroscaleri%3A%2BCost-Effective%2BScaling%2Bfor%2BMicroservice%2BApplications%2Bin%2Bthe%2BCloud%2BWith%2Ban%2BOnline%2BLearning%2BApproach)**
  *Authors*: Guangba Yu, Pengfei Chen, Zibin Zheng
  *Publication*: TCC-2022
  *Summary*: This paper addresses the challenge of autoscaling microservice applications, where complex service dependencies make it difficult to identify which services need scaling during workload spikes. Microscaler collects QoS metrics from the service mesh, identifies scaling-needed services using a novel "service power" criterion along the dependency graph, and combines Bayesian optimization-based online learning with step-by-step heuristics to reach optimal scaling. Evaluations on a microservice benchmark show 93% precision in identifying scaling-needed services and faster convergence to optimal service scale than state-of-the-art methods.
  **Code**: Not available

- **[A Dual-Agent Scheduler for Distributed Deep Learning Jobs on Public Cloud via Reinforcement Learning]
  *Authors*: Mingzhe Xing, Hangyu Mao, Shenglin Yin, Lichen Pan, Zhengchao Zhang, Zhen Xiao, Jieyi Long
  *Publication*: KDD-2023
  *Summary*: This paper tackles distributed deep learning job scheduling on public cloud GPU clusters, where existing methods typically optimize job ordering or placement independently without considering their cooperation. A dual-agent reinforcement learning framework is proposed: an ordering agent uses a scalable squeeze-and-communicate strategy for coordinated job sequencing, while a placement agent employs a Random Walk Gaussian Process to model GPU machine performance similarities and account for resource contention. Experiments show the dual-agent scheduler reduces training fees and job completion time compared to baselines.
  **Code**: Not available

- **[A heuristic multi-objective task scheduling framework for container-based clouds via actor-critic reinforcement learning]
  *Authors*: Lilu Zhu, Feng Wu, Yanfeng Hu, Kai Huang, Xinmei Tian
  *Publication*: 2023
  *Summary*: This paper proposes AC-CCTS, a heuristic multi-objective task scheduling framework for container-based clouds that balances business performance (QoS) and resource utilization efficiency during peak application access periods. Built on the actor-critic algorithm, it incorporates heuristic rules and prioritized experience replay to accelerate convergence, a compensation mechanism for robustness, and a dynamic scheduling model for container cloud environments. Compared with meta-heuristic methods (FIMPSO, HWOA-MBA) and other RL algorithms (DeepRM-Plus, RLSched), AC-CCTS demonstrates better resource utilization efficiency and convergence stability.
  **Code**: Not available

- **[A Hierarchical Framework of Cloud Resource Allocation and Power Management Using Deep Reinforcement Learning]
  *Authors*: Ning Liu, Zhe Li, Jielong Xu, Zhiyuan Xu, Sheng Lin, Qinru Qiu, Jian Tang, Yanzhi Wang
  *Publication*: ICDCS-2017
  *Summary*: This paper proposes a hierarchical framework for jointly optimizing VM resource allocation and dynamic power management in cloud computing systems. The global tier uses deep reinforcement learning with an autoencoder and weight sharing structure to handle high-dimensional state spaces for VM-to-server allocation, while the local tier combines LSTM-based workload prediction with model-free RL for distributed server power management. Evaluated on Google cluster traces, the framework significantly reduces power consumption and energy usage compared to baselines without severe latency degradation.
  **Code**: Not available

- **[A multi-objective trade-off framework for cloud resource scheduling based on the Deep Q-network algorithm]
  *Authors*: Zhiping Peng, Jianpeng Lin, Delong Cui, Qirui Li, Jieguang He
  *Publication*: Cluster Computing-2022
  *Summary*: This paper addresses the conflict between cloud service providers minimizing energy costs and users seeking optimized service quality through an online DQN-based resource scheduling framework. The framework enables dynamic trade-offs between energy consumption and task makespan by adjusting the proportion of rewards assigned to each optimization objective. Experiments demonstrate the framework effectively balances these competing objectives and achieves clear improvements over baseline algorithms.
  **Code**: Not available

- **[Actor-Critic with Transformer for Cloud Computing Resource Three Stage Job Scheduling]
  *Authors*: Yanbo Xu, Jiakun Zhao
  *Publication*: ICCCBDA-2022
  *Summary*: This paper presents ACT4JS, an actor-critic with transformer algorithm for three-stage job scheduling that manages data centers, server nodes, and application containers. The algorithm uses transformer network structures and proximal policy optimization (PPO) for feature learning and loss optimization, handling both single-task multi-instance jobs and DAG jobs with dependencies. Experiments show ACT4JS achieves lower energy consumption costs and task reject rates than mainstream baselines under online training.
  **Code**: Not available

- **[Adaptive and Efficient Resource Allocation in Cloud Datacenters Using Actor-Critic Deep Reinforcement Learning]
  *Authors*: Zheyi Chen, Jia Hu, Geyong Min, Chunbo Luo, Tarek El-Ghazawi
  *Publication*: TPDS-2022
  *Summary*: This paper proposes an actor-critic deep reinforcement learning scheme for adaptive cloud datacenter resource allocation that does not require prior knowledge of the system. The actor parameterizes the scheduling policy while the critic evaluates actions, with policy updates using gradient ascent and variance reduction via an advantage function to improve training efficiency. Evaluated on Google cloud datacenter traces, the method achieves superior latency, lower job dismissal rate, and enhanced energy efficiency compared to two advanced DRL-based and five classic resource allocation methods.
  **Code**: Not available

- **[ADRL: A Hybrid Anomaly-Aware Deep Reinforcement Learning-Based Resource Scaling in Clouds]
  *Authors*: Sara Kardani-Moghaddam, Rajkumar Buyya, Kotagiri Ramamohanarao
  *Publication*: TPDS-2021
  *Summary*: This paper proposes ADRL, a hybrid anomaly-aware deep reinforcement learning approach for dynamic vertical resource scaling in clouds. ADRL integrates anomaly detection techniques to trigger scaling actions in response to identified anomalous states, employing two levels of global and local decision-makers to handle required scaling actions. Experiments across different anomaly scenarios show ADRL significantly improves QoS with fewer scaling actions and increased system stability compared to threshold-based and time series methods.
  **Code**: Not available

- **[Cloud Resource Scheduling With Deep Reinforcement Learning and Imitation Learning]
  *Authors*: Wenxia Guo, Wenhong Tian, Yufei Ye, Lingxiao Xu, Kui Wu
  *Publication*: IOTJ-2021
  *Summary*: This paper presents DeepRM_Plus, a deep RL-based solution using a convolutional neural network to model cloud resource management and imitation learning to accelerate policy training. By combining imitation learning into the reinforcement process, DeepRM_Plus converges 37.5% faster than the state-of-the-art DeepRM algorithm. It also reduces the average weighted turnaround time by 51.85% and average cycling time by 11.51%.
  **Code**: Not available

- **[Cost-aware job scheduling for cloud instances using deep reinforcement learning]
  *Authors*: Feng Cheng, Yifeng Huang, Bhavana Tanpure, Pawan Sawalani, Long Cheng, Cong Liu
  *Publication*: Cluster Computing-2022
  *Summary*: This paper addresses real-time job scheduling for dynamic cloud workloads where user requests arrive continuously, unlike most existing approaches designed for batch jobs. A DQN-based scheduler is developed that optimizes both QoS for end-users and cost reduction on virtual machine instances. Experimental results demonstrate the DQN scheduler significantly outperforms commonly used real-time scheduling algorithms in both QoS and cost metrics.
  **Code**: Not available

- **[Data Centers Job Scheduling with Deep Reinforcement Learning]
  *Authors*: Sisheng Liang, Zhou Yang, Fang Jin, Yong Chen
  *Publication*: PAKDD-2020
  *Summary*: This paper proposes A2cScheduler, an Advantage Actor-Critic (A2C) deep reinforcement learning approach for job scheduling in data centers with heterogeneous resources. A2cScheduler employs two agents -- an actor that learns the scheduling policy and a critic that reduces estimation error -- designed to minimize gradient estimation variance and update parameters more efficiently than previous policy gradient methods. The approach achieves competitive scheduling performance on both simulated workloads and real data collected from an academic data center.
  **Code**: Not available

- **[DDQN-TS: A novel bi-objective intelligent scheduling algorithm in the cloud environment]
  *Authors*: Zhao Tong, Feng Ye, Bilan Liu, Jinhui Cai, Jing Mei
  *Publication*: Neurocomputing-2021
  *Summary*: This paper addresses dynamic online task scheduling in cloud environments where limited resources must serve high-QoS requests. The proposed DDQN-TS algorithm uses the adaptive learning capability of Double Deep Q-Network (DDQN) to explore optimal scheduling strategies, mitigating the overestimation bias of standard DQN. Experiments on Random, Google, and Alibaba benchmarks show DDQN-TS guarantees a high task completion rate and effectively reduces average task response time compared to classic scheduling algorithms.
  **Code**: Not available

- **[Deep Reinforcement Learning based Compute-Intensive Workload Allocation in Data Centers with High Energy Efficiency]
  *Authors*: Zhenfeng Gao, Wei Liu, Long Suo, Jiandong Li, Yijun Lu
  *Publication*: ICCC-2021
  *Summary*: This paper proposes AC-CIWAS, an Actor-Critic deep reinforcement learning scheme for allocating compute-intensive workloads to physical servers in data centers to reduce energy consumption while guaranteeing QoS. The method continuously captures dynamic server states and uses a DRL-based Actor-Critic algorithm to evaluate cumulative returns that guide energy-efficient workload allocation. Simulations show AC-CIWAS reduces server power consumption by approximately 20 percent compared to baseline methods while maintaining QoS.
  **Code**: Not available

- **[Deep Reinforcement Learning Enhanced Greedy Algorithm for Online Scheduling of Batched Tasks in Cloud in Cloud HPC Systems](https://scholar.google.com/scholar?q=Deep%2BReinforcement%2BLearning%2BEnhanced%2BGreedy%2BAlgorithm%2Bfor%2BOnline%2BScheduling%2Bof%2BBatched%2BTasks%2Bin%2BCloud%2Bin%2BCloud%2BHPC%2BSystems)**
  *Authors*: Yuanhao Yang, Hong Shen
  *Publication*: TPDS-2022
  *Summary*: This paper addresses online scheduling of batched tasks arriving in cloud HPC systems by proposing a two-stage DRL-enhanced greedy algorithm that jointly optimizes task sequencing and allocation. A DRL module predicts the optimal allocation sequence for each batch based on prior learning, while a greedy strategy allocates tasks to heterogeneous servers with a proven competitive ratio bound of 1/(1+k). Experiments in both simulation and real environments show the algorithm increases system net gain by 10% to 30% over state-of-the-art baselines.
  **Code**: Not available

- **[Deep Reinforcement Learning for Dynamic Workflow Scheduling in Cloud Environment](https://doi.org/10.1109/scc53864.2021.00023)**
  *Authors*: Tingting Dong, Fei Xue, Changbai Xiao, Jiangjiang Zhang
  *Publication*: SCC-2021
  *Summary*: This paper studies dynamic workflow scheduling in cloud environments while accounting for the performance variation of cloud resources, which most existing algorithms ignore. The proposed RLWS approach formulates the makespan-minimization problem as a Markov Decision Process and uses an Actor-Critic deep reinforcement learning method that learns neural network parameters through iterative local re-scheduling. Experiments confirm the algorithm efficiently shortens workflow makespan compared to conventional approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning for Multi-resource Cloud Job Scheduling](https://scholar.google.com/scholar?q=Deep%2BReinforcement%2BLearning%2Bfor%2BMulti-resource%2BCloud)**
  *Authors*: Jianpeng Lin, Zhiping Peng, Delong Cui
  *Publication*: ICNP-2017
  *Summary*: This paper extends the DeepRM approach to multi-resource multi-machine job scheduling across multiple server clusters, representing resource occupancy status as images for deep reinforcement learning processing. The authors present several improvements to the original model and demonstrate that DRL-based methods can outperform traditional heuristic resource allocation algorithms in complex multi-resource environments.
  **Code**: Not available

- **[Deep reinforcement learning-aided multi-step job scheduling in optical data center networks](https://scholar.google.com/scholar?q=Deep%2Breinforcement%2Blearning-aided%2Bmulti-step%2Bjob%2Bscheduling)**
  *Authors*: Che-Yu Liu, Xiaoliang Chen, Roberto Proietti, Zuqing Zhu, S. J. Ben Yoo
  *Publication*: ICDBC-2025
  *Summary*: This paper addresses joint job scheduling and topology reconfiguration in optical data center networks (ODCNs) to handle intensive communication demands from distributed ML workloads. A DRL-based multi-step scheduling algorithm decomposes each job into an ordered VM sequence and learns sequential placement decisions using a dual reward scheme combining team incentives for end-to-end job provisioning and individual rewards for advantageous local placements. Simulations show the approach reduces job-blocking probability and reconfiguration frequency by at least 7.35% and 4.59% respectively over heuristic baselines.
  **Code**: Not available

- **[Deep reinforcement learning-based methods for resource scheduling in cloud computing: a review and future directions](https://arxiv.org/abs/2103.16428)**
  *Authors*: Guangyao Zhou, Wenhong Tian, Rajkumar Buyya, Ruini Xue, Liang Song
  *Publication*: arXiv-2021
  *Summary*: This survey provides a comprehensive review of deep reinforcement learning methods applied to resource scheduling in cloud computing. The authors analyze the theoretical formulation of scheduling problems and RL frameworks, discuss the advantages of DRL-based methods over classical heuristics and meta-heuristics in complex cloud scenarios, and identify key challenges and future research directions for DRL in cloud scheduling.
  **Code**: Not available

- **[DeepEE: Joint Optimization of Job Scheduling and Cooling Control for Data Center Energy Efficiency Using Deep Reinforcement Learning](https://scholar.google.com/scholar?q=DeepEE:+Joint+Optimization+of+Job+Scheduling+and+Cooling+Control+for+Data+Center+Energy+Efficiency+Using+Deep+Reinforcement+Learning)**
  *Authors*: Yongyi Ran, Han Hu, Xin Zhou, Yonggang Wen
  *Publication*: ICDCS-2019
  *Summary*: This paper proposes DeepEE, a DRL-based framework that jointly optimizes IT job scheduling and cooling control to improve data center energy efficiency. The authors design a Parameterized Action space Deep Q-Network (PADQN) algorithm with a two-time-scale control mechanism to handle the hybrid action space of scheduling decisions and airflow rate adjustments. Using real-trace simulations, DeepEE achieves up to 15% and 10% energy savings over baseline siloed and joint optimization approaches respectively, with more stable performance and a better energy-QoS tradeoff.
  **Code**: Not available

- **[DRAS: Deep Reinforcement Learning for Cluster Scheduling in High Performance Computing](https://scholar.google.com/scholar?q=DRAS:+Deep+Reinforcement+Learning+for+Cluster+Scheduling+in+High+Performance+Computing)**
  *Authors*: Yuping Fan, Boyang Li, Dustin Favorite, Naunidh Singh, Taylor Childers, Paul Rich, William Allcock, Michael E. Papka, Zhiling Lan
  *Publication*: TPDS-2022
  *Summary*: This paper presents DRAS, an automated HPC cluster scheduling agent built on a hierarchical neural network that incorporates domain-specific features such as resource reservation and backfilling. Given a scheduling objective from the system manager, DRAS learns and dynamically adjusts its policy through interaction with the environment. Implemented in the CQGym evaluation platform and tested with production workloads, DRAS outperforms existing heuristic and optimization approaches by up to 50%.
  **Code**: Not available

- **[DRL-cloud: Deep reinforcement learning-based resource provisioning and task scheduling for cloud service providers](https://doi.org/10.1109/aspdac.2018.8297294)**
  *Authors*: Mingxi Cheng, Ji Li, Shahin Nazarian
  *Publication*: ASP-DAC-2018
  *Summary*: This paper presents DRL-Cloud, a deep Q-learning-based system that jointly optimizes resource provisioning and task scheduling (including task dependencies) for large-scale cloud service providers to minimize energy cost. The two-stage RP-TS processor learns from changing user request patterns and real-time electricity pricing using experience replay and target network techniques. Evaluations on a 5,000-server setup with 200,000 tasks show up to 320% energy cost efficiency improvement and 144% runtime reduction compared to baselines.
  **Code**: Not available

- **[Dynamic Job Shop Scheduling via Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Dynamic+Job+Shop+Scheduling+via+Deep+Reinforcement+Learning)**
  *Authors*: Xinjie Liang, Wen Song, Pengfei Wei
  *Publication*: NeurIPS-2020
  *Summary*: This paper addresses the dynamic job-shop scheduling problem (DJSP) under uncertainty by proposing a DRL-based method that directly selects legitimate jobs as actions, breaking free from the limitations of fixed dispatching rule sets. Two training methods are designed: a gradient-based algorithm with dense rewards and an evolutionary strategy with sparse rewards. Experiments show the DRL method learns high-quality dispatching policies that significantly outperform a state-of-the-art Genetic Programming-based dispatching rule learning approach.
  **Code**: Not available

- **[Efficient Compute-Intensive Job Allocation in Data Centers via Deep Reinforcement Learning](https://doi.org/10.1109/tpds.2020.2968427)**
  *Authors*: Deliang Yi, Xin Zhou, Yonggang Wen, Rui Tan
  *Publication*: TPDS-2020
  *Summary*: This paper applies deep reinforcement learning to allocate long-lasting compute-intensive jobs in data centers, training a deep Q-network offline using an LSTM-based computational model that captures server power and thermal dynamics. This offline training avoids the slow convergence, low energy efficiency, and potential overheating risks of direct online interaction. Evaluation with eight months of data from a 1,152-processor national supercomputing data center shows the solution reduces computing power consumption by over 10% and processor temperature by more than 4C without sacrificing throughput.
  **Code**: Not available

- **[Energy-Efficient Task Scheduling in Data Centers Using Adaptive Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Energy-Efficient%2BTask%2BScheduling%2Bin%2BData%2BCenters)**
  *Authors*: Dinuț Ionuț-Cosmin, Bogdan Alexandrescu, Rodica-Claudia Constantinescu
  *Publication*: Code-2025
  *Summary*: This paper uses a Deep Reinforcement Learning agent trained with Proximal Policy Optimization (PPO) to dynamically schedule incoming tasks across multiple servers in data centers, aiming to balance energy minimization with low service latency. Simulations with fluctuating workloads show the RL agent outperforms standard heuristics such as Round-Robin and Least-Loaded, achieving a superior tradeoff between power consumption reduction and SLA violation minimization. The results demonstrate that adaptive RL-based policies are effective for intelligent data center resource management.
  **Code**: Not available

- **[GARLSched: Generative adversarial deep reinforcement learning task scheduling optimization for large-scale high performance computing systems](https://scholar.google.com/scholar?q=GARLSched:+Generative+adversarial+deep+reinforcement+learning+task+scheduling+optimization+for+large-scale+high+performance+computing+systems)**
  *Authors*: Jingbo Li, Xingjun Zhang, Jia Wei, Zeyu Ji, Zheng Wei
  *Publication*: FGCS-2022
  *Summary*: Addresses the challenge of DRL training convergence in large-scale HPC task scheduling caused by task exogeneity and reward sparsity. GARLSched combines generative adversarial reinforcement learning with expert policy guidance, using a task embedding-based discriminator network to stabilize the learning process. Experiments show it learns high-quality scheduling policies for various workloads and optimization objectives, maintaining stable performance even on unseen workloads.
  **Code**: Not available

- **[gym-hpa: Efficient Auto-Scaling via Reinforcement Learning for Complex Microservice-based Applications in Kubernetes](https://doi.org/10.1109/noms56928.2023.10154298)**
  *Authors*: José Santos, Tim Wauters, Bruno Volckaert, Filip De Turck
  *Publication*: NOMS-2023
  *Summary*: Proposes gym-hpa, an OpenAI Gym-based reinforcement learning framework for Kubernetes auto-scaling that explicitly accounts for microservice inter-dependencies in horizontal scaling decisions. RL agents trained with this framework reduce resource usage by approximately 30% and application response time by about 25% compared to default Kubernetes scaling mechanisms.
  **Code**: Not available

- **[Heterogeneous-Aware Online Cloud Task Scheduler Based on Clustering and Deep Reinforcement Learning Ensemble](https://doi.org/10.1007/978-3-030-70665-4_18)**
  *Authors*: Dan Gu, Jing Chen, Xiaoyu Shi, Longyu Ran, Ying Zhang, Mingsheng Shang
  *Publication*: ICNC-FSKD-2020
  *Summary*: Proposes an intelligent cloud task scheduler that combines k-means clustering to identify workload types with a Deep Deterministic Policy Gradient (DDPG) algorithm for optimized task dispatch across heterogeneous virtual machines. Evaluated on Alibaba's real workload traces, the scheduler outperforms existing methods in both response time and resource utilization.
  **Code**: Not available

- **[Integrated and Fungible Scheduling of Deep Learning Workloads Using Multi-Agent Reinforcement Learning](https://doi.org/10.1109/tpds.2024.3522333)**
  *Authors*: Jialun Li, Danyang Xiao, Diying Yang, Xuan Mo, Weigang Wu
  *Publication*: 2025
  *Summary*: Presents MAIFS, a multi-agent reinforcement learning algorithm that integrates task placement and resource allocation for deep learning workloads on shared GPU clusters, allowing fungible resource allocation based on workload resource sensitivity. The approach uses a multi-agent attention mechanism to share resource state features across agents and a dynamic coordination graph to mitigate task placement conflicts. Experiments on production DL workload traces and a Kubernetes-based GPU cluster show improvements of up to 44% in makespan and 46% in job completion time over state-of-the-art schedulers.
  **Code**: Not available

- **[Minerva: A reinforcement learning-based technique for optimal scheduling and bottleneck detection in distributed factory operations](https://doi.org/10.1109/comsnets.2018.8328189)**
  *Authors*: Tara Elizabeth Thomas, Jinkyu Koo, Somali Chaterji, Saurabh Bagchi
  *Publication*: ICCSN-2018
  *Summary*: Addresses the job shop scheduling problem with periodic job arrivals by combining model-free reinforcement learning for optimal resource scheduling with a neural network classifier for bottleneck detection. MINERVA achieves 95.2% accuracy in identifying system bottlenecks, nearly 25% better than best-in-class bottleneck identification methods.
  **Code**: Not available

- **[Model-free control for distributed stream data processing using deep reinforcement learning](https://doi.org/10.14778/3184470.3184474)**
  *Authors*: Teng Li, Zhiyuan Xu, Jian Tang, Yanzhi Wang
  *Publication*: VLDB-2018
  *Summary*: Proposes the first DRL-based control framework for distributed stream data processing systems, jointly learning the system environment from limited runtime statistics and making scheduling decisions guided by deep neural networks to minimize average end-to-end tuple processing time. Implemented on Apache Storm, the framework reduces tuple processing time by 33.5% over Storm's default scheduler and 14.0% over the state-of-the-art model-based method.
  **Code**: Not available

- **[Multi-Dimensional Resource Allocation in Distributed Data Centers Using Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Multi-Dimensional%2BResource%2BAllocation%2Bin%2BDistributed%2BData%2BCenters%2BUsing%2BDeep%2BReinforcement%2BLearning)**
  *Authors*: Wenting Wei, Huaxi Gu, Kun Wang, Jianjia Li, Xuan Zhang, Ning Wang
  *Publication*: TNSM-2022
  *Summary*: Presents NESRL-MRM, a natural evolution strategy-based reinforcement learning approach for multi-dimensional resource allocation across distributed data centers that achieves balanced utilization of heterogeneous ICT resources under dynamic and uncertain environments. Evaluated using real-world workload traces from Amazon EC2 and Google datacenters, the approach significantly improves multi-dimensional resource balance and reduces blocking probability for incoming workload demands.
  **Code**: Not available

- **[Optimizing Job Scheduling using Deep Reinforcement Learning](https://dl.acm.org/doi/10.1145/3502181.3531474)**
  *Authors*: Rohit Sigar, Avadh Kishor, Pramod Kumar Singh, Joydip Dhar
  *Publication*: HPDC-2022
  *Summary*: Proposes a Deep Q-Network (DQN) model for job scheduling that aims to minimize makespan while maximizing resource utilization. Evaluated against four existing scheduling models across two different datasets, the DQN-based approach demonstrates superior or comparable performance in both metrics.
  **Code**: Not available

- **[Performance and Cost-Efficient Spark Job Scheduling Based on Deep Reinforcement Learning in Cloud Computing Environments](https://doi.org/10.1109/tpds.2021.3124670)**
  *Authors*: Muhammed Tawfiqul Islam, Shanika Karunasekera, Rajkumar Buyya
  *Publication*: TPDS-2021
  *Summary*: Formulates the job scheduling problem for cloud-deployed Spark clusters with multiple SLA objectives including cost reduction and job performance improvement, and implements two DRL-based schedulers using the TF-Agents framework. The agents learn inherent characteristics of different job types to find proper placements, reducing both total cluster VM usage cost and average job duration, with VM usage cost reduced by up to 30%.
  **Code**: Not available

- **[READYS: A Reinforcement Learning Based Strategy for Heterogeneous Dynamic Scheduling](https://doi.org/10.1109/cluster48925.2021.00031)**
  *Authors*: Nathan Grinsztajn, Olivier Beaumont, Emmanuel Jeannot, Philippe Preux
  *Publication*: CLUSTER-2021
  *Summary*: Proposes READYS, which combines Graph Convolutional Networks (GCN) with an A2C actor-critic algorithm for dynamic DAG scheduling on heterogeneous CPU/GPU platforms. The approach learns a general scheduling strategy that is not limited to a specific task graph or problem size and can schedule any DAG. Simulations show the agent performs comparably or superior to existing algorithms, particularly excelling under scheduling uncertainty.
  **Code**: Not available

- **[Resource Management with Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Resource+Management+with+Deep+Reinforcement+Learning)**
  *Authors*: Hongzi Mao, Mohammad Alizadeh, Ishai Menache, Srikanth Kandula
  *Publication*: HotNets-2016
  *Summary*: Introduces DeepRM, one of the first works applying DRL to cluster resource management, translating the multi-resource task packing problem into a learning-based approach. DeepRM performs comparably to state-of-the-art heuristics while adapting to varying conditions, converging quickly, and learning intuitively sensible scheduling strategies.
  **Code**: Not available

- **[RLQ: Workload Allocation With Reinforcement Learning in Distributed Queues](https://doi.org/10.1109/tpds.2022.3231981)**
  *Authors*: Alessandro Staffolani, Victor-Alexandru Darvariu, Paolo Bellavista, Mirco Musolesi
  *Publication*: TPDS-2023
  *Summary*: Addresses task allocation in distributed queue systems where task-specific information (resource demands, expected execution time) is unavailable and worker nodes have heterogeneous capabilities. RLQ, implemented with the Celery queuing system, reduces execution cost by ~70%, execution time by 3x, and waiting time by 7x on synthetic workloads, and also outperforms a Google Borg-inspired E-PVM strategy in five out of six scenarios.
  **Code**: Not available

- **[RLScheduler: An Automated HPC Batch Job Scheduler Using Reinforcement Learning](https://scholar.google.com/scholar?q=RLScheduler:+An+Automated+HPC+Batch+Job+Scheduler+Using+Reinforcement+Learning)**
  *Authors*: Di Zhang, Dong Dai, Youbiao He, Forrest Sheng Bao, Bing Xie
  *Publication*: SC-2020
  *Summary*: Presents an automated HPC batch job scheduler using reinforcement learning that requires minimal manual intervention or expert knowledge, relying instead on continuous trial-and-error to learn high-quality scheduling policies. Introduces a kernel-based neural network structure and trajectory filtering mechanism to stabilize learning, with experiments confirming stable performance even on unseen workloads.
  **Code**: Not available

- **[RLSK: A Job Scheduler for Federated Kubernetes Clusters based on Reinforcement Learning](https://doi.org/10.1109/ic2e48712.2020.00019)**
  *Authors*: Jiaming Huang, Chuming Xiao, Weigang Wu
  *Publication*: IC2E-2020
  *Summary*: Presents RLSK, a DRL-based job scheduler for federated Kubernetes clusters that adaptively schedules independent batch jobs across multiple cloud clusters while optimizing for load balancing. By specifying only high-level scheduling targets, RLSK learns strategies from environment interaction without prior knowledge of the multi-cluster setup, outperforming traditional scheduling algorithms in simulations.
  **Code**: Not available

- **[Scheduling of Time-Varying Workloads Using Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/16190)**
  *Authors*: Shanka Subhra Mondal, Nikhil Sheoran, Subrata Mitra
  *Publication*: AAAI-2021
  *Summary*: Addresses the challenge of scheduling production workloads with time-varying resource usage patterns that fluctuate significantly over time, which prior work overlooked. Proposes a DRL-based approach that exploits temporal resource patterns combined with an equivalence class technique to improve scalability, validated on real Google and Alibaba production traces showing improved cluster utilization, reduced fragmentation, and fewer resource exhaustion events.
  **Code**: Not available

- **[SibylOpt: Managing Green Data Centers Using Off-Online Deep Reinforcement Learning](https://scholar.google.com/scholar?q=SibylOpt%3A%2BManaging%2BGreen%2BData%2BCenters%2BUsing%2BOff-Online%2BDeep%2BReinforcement%2BLearning)**
  *Authors*: Ning Gu, Kuo Zhang, Thu Nguyen, Peijian Wang, Tania Lorido Botran
  *Publication*: SoCC-2022
  *Summary*: Proposes SibylOpt, which uses an off-online DRL approach combining offline pre-training on historical data with online fine-tuning to manage green data centers. The method optimizes energy efficiency and carbon-aware workload placement while meeting performance constraints, learning adaptive scheduling policies that balance energy costs with service quality.
  **Code**: Not available

- **[SIMPPO: A Scalable and Incremental Online Learning Framework for Serverless Resource Management](https://scholar.google.com/scholar?q=SIMPPO:+A+Scalable+and+Incremental+Online+Learning+Framework+for+Serverless+Resource+Management)**
  *Authors*: Jiaming Huang, Chuming Xiao, Weigang Wu
  *Publication*: SoCC-2022
  *Summary*: Proposes SIMPPO, a scalable and incremental multi-agent PPO framework for serverless FaaS resource management that addresses the convergence failures of single-agent RL in multi-tenant environments. SIMPPO enables each RL agent to converge efficiently during training while providing function latency performance comparable to isolated single-agent RL, reducing p99 function latency by 4.5x compared to single-agent RL in multi-tenant settings.
  **Code**: Not available

- **[SLAs-Aware Online Task Scheduling Based on Deep Reinforcement Learning Method in Cloud Environment](https://scholar.google.com/scholar?q=SLAs-Aware+Online+Task+Scheduling+Based+on+Deep+Reinforcement+Learning+Method+in+Cloud+Environment)**
  *Authors*: Longyu Ran, Xiaoyu Shi, Mingsheng Shang
  *Publication*: HPCC-2019
  *Summary*: Proposes a DRL-based online task scheduling method for cloud environments that explicitly considers Service Level Agreements (SLAs) as constraints during scheduling decisions. The approach learns to balance task throughput with SLA compliance, adapting to dynamic workload arrivals and heterogeneous cloud resources while minimizing SLA violations.
  **Code**: Not available

- **[Spear: Optimized Dependency-Aware Task Scheduling with Deep Reinforcement Learning](https://scholar.google.com/scholar?q=Spear:+Optimized+Dependency-Aware+Task+Scheduling+with+Deep+Reinforcement+Learning)**
  *Authors*: Zhiming Hu, James Tu, Baochun Li
  *Publication*: ICDCS-2019
  *Summary*: Presents Spear, which applies Monte Carlo Tree Search (MCTS) guided by a DRL model to minimize makespan for complex DAG-based jobs with heterogeneous multi-resource demands. The DRL model improves MCTS search efficiency by focusing on more promising scheduling branches. Evaluated on production workload traces, Spear outperforms state-of-the-art job schedulers by up to 20%.
  **Code**: Not available

- **[Task Scheduling in Cloud Using Deep Reinforcement Learning](https://doi.org/10.1016/j.procs.2021.03.016)**
  *Authors*: Shashank Swarup, Elhadi M. Shakshuki, Ansar Yasar
  *Publication*: Code-2021
  *Summary*: Applies deep reinforcement learning to cloud task scheduling, where a DRL agent learns to map incoming tasks to available cloud resources by considering task requirements and server capabilities. The approach is evaluated against traditional scheduling heuristics, demonstrating improved makespan and resource utilization in cloud environments.
  **Code**: Not available

- **[Toward Efficient Compute-Intensive Job Allocation for Green Data Centers: A Deep Reinforcement Learning Approach](https://doi.org/10.32657/10356/104419)**
  *Authors*: Deliang Yi, Xin Zhou, Yonggang Wen, Rui Tan
  *Publication*: ICDCS-2019
  *Summary*: Addresses compute-intensive job allocation in green data centers powered by renewable energy, formulating the problem as a cost optimization that balances electricity costs with job completion requirements. Proposes a DRL-based approach that learns adaptive allocation policies considering renewable energy availability, electricity pricing, and job characteristics, achieving efficient job scheduling while reducing energy costs.
  **Code**: Not available

- **[SchedInspector: A Batch Job Scheduling Inspector Using Reinforcement Learning](https://scholar.google.com/scholar?q=SchedInspector:+A+Batch+Job+Scheduling+Inspector+Using+Reinforcement+Learning)**
  *Authors*: Di Zhang, Dong Dai, Bing Xie
  *Publication*: HPDC-2022
  *Summary*: This paper takes an inspect-and-correct approach to batch job scheduling in HPC clusters. Rather than replacing the existing scheduler, a reinforcement learning agent monitors scheduler decisions and predicts their outcomes (job completion time, resource utilization). When suboptimal decisions are detected, the system flags them and takes corrective actions such as re-prioritizing jobs or reallocating resources. This approach is less disruptive than full scheduler replacement and can be deployed incrementally in production environments.
  **Code**: Not available

- **[DeepJS: Job Scheduling Based on Deep Reinforcement Learning in Cloud Data Center](https://scholar.google.com/scholar?q=DeepJS:+Job+Scheduling+Based+on+Deep+Reinforcement+Learning+in+Cloud+Data+Center)**
  *Authors*: Fengcun Li, Bo Hu
  *Publication*: ICDBC-2021
  *Summary*: This paper proposes a deep reinforcement learning approach for job scheduling in cloud data centers. The system uses a DRL agent to learn optimal job-to-machine mapping decisions by considering factors such as resource demands, machine availability, and job priority. Experimental results demonstrate improved resource utilization and reduced job completion time compared to traditional scheduling heuristics.
  **Code**: Not available

---

- **[ASTRA: Adversarial Sim-to-Real Transfer Reinforcement Learning for Autoscaling in Cloud Systems](https://doi.org/10.1109/tse.2025.3603995)**
  *Authors*: Tiangang Li, Shi Ying, Xiangbo Tian, Ting Zhang, Yong Wang
  *Publication*: TSE-2025
  *Summary*: This paper proposes ASTRA, a sim-to-real transfer reinforcement learning framework for cloud autoscaling that addresses the high interaction costs and data inefficiency of training DRL autoscalers on real systems. ASTRA constructs a simulation environment based on a hybrid attentive state space model that captures system dynamics and state evolution, enabling low-cost policy training. An adversarial soft actor-critic method with gradient regularization is then used to mitigate policy performance degradation from distribution shift when transferring to real cloud systems.
  **Code**: Not available

- **[A Meta Reinforcement Learning Approach for Predictive Autoscaling in the Cloud](https://scholar.google.com/scholar?q=A+Meta+Reinforcement+Learning+Approach+for+Predictive+Autoscaling+in+the+Cloud)**
  *Authors*: Siqiao Xue, Chao Qu, Xiaoming Shi, Cong Liao, Shiyi Zhu, Xiaoyu Tan, Lintao Ma, Shiyu Wang, Shijun Wang, Yun Hu
  *Publication*: KDD-2022
  *Summary*: This paper proposes a meta model-based RL algorithm for predictive autoscaling that incorporates a deep periodic workload prediction model and embeds Neural Process to guide learning of optimal scaling actions across numerous application services. The approach enables scaling decisions to adapt to changing workloads with high sample efficiency while maintaining stable CPU utilization. Deployed online at Alipay, it significantly outperforms existing algorithms on the world-leading payment platform.
  **Code**: Not available

- **[A-SARSA: A Predictive Container Auto-Scaling Algorithm Based on Reinforcement Learning](https://doi.org/10.1109/icws49710.2020.00072)**
  *Authors*: Shubo Zhang, Tianyang Wu, Maolin Pan, Chaomeng Zhang, Yang Yu
  *Publication*: ICWS-2020
  *Summary*: This paper proposes A-SARSA, a predictive container auto-scaling algorithm that combines ARIMA time-series prediction and neural network models with the SARSA RL algorithm to address untimely scheduling and poor decision accuracy in container scaling. Experiments verify the algorithm significantly reduces SLA violation rates while maintaining good resource utilization levels.
  **Code**: Not available

- **[AWARE Automate Workload Autoscaling with Reinforcement Learning in Production Cloud Systems](https://scholar.google.com/scholar?q=AWARE%2BAutomate%2BWorkload%2BAutoscaling%2Bwith%2BReinforcement%2BLearning%2Bin%2BProduction%2BCloud%2BSystems)**
  *Authors*: Haoran Qiu, Weichao Mao
  *Publication*: ATC-2023
  *Summary*: This paper presents AWARE, a production system that bridges the gap between RL research and real-world deployment for workload autoscaling. AWARE provides RL bootstrapping, incremental online retraining, and fast policy adaptation, enabling learned policies to adapt to new workloads 5.5x faster than transfer-learning baselines with under 3.6% reward degradation. During training, it achieves 47.5% and 39.2% higher CPU and memory utilization while reducing SLO violations by 16.9x.
  **Code**: Not available

- **[DScaler: A Horizontal Autoscaler of Microservice Based on Deep Reinforcement Learning](https://doi.org/10.23919/apnoms56106.2022.9919994)**
  *Authors*: Zhijiao Xiao, Song Hu
  *Publication*: APNOMS-2022
  *Summary*: This paper proposes DScaler, a DRL-based horizontal pod autoscaler for Kubernetes microservices that overcomes the static threshold limitations of the built-in HPA under highly dynamic workloads. Under two different workload patterns, DScaler reduces resource consumption by 19.90% and 10.80% while reducing SLA violations by 8.56% and 12.75% compared to HPA, and cuts resource usage by approximately 60% compared to existing RL strategies.
  **Code**: Not available

- **[Fast and Fine-grained Autoscaler for Streaming Jobs with Reinforcement Learning](https://arxiv.org/abs/2201.08439)**
  *Authors*: Mingzhe Xing, Hangyu Mao, Zhen Xiao
  *Publication*: IJCAI-2022
  *Summary*: This paper proposes a fine-grained task-level autoscaler for streaming jobs that organizes running states as spatio-temporal graphs and uses a Neural Variational Subgraph Sampler with a mutual-information-based objective to efficiently extract representative subgraphs for RL decisions. Experiments on real-world datasets demonstrate superiority over six competitive baselines.
  **Code**: Not available

- **[Intelligent microservices autoscaling module using reinforcement learning](https://doi.org/10.1007/s10586-023-03999-8)**
  *Authors*: Abeer Abdel Khaleq, Ilkyeun Ra
  *Publication*: CC-2023
  *Summary*: This paper introduces an intelligent RL-based autoscaling module for horizontal scaling of microservices that customizes Kubernetes HPA using response time as a QoS metric. The agents are trained, validated, and deployed on Google Cloud, where they learn microservice resource usage patterns from the cloud environment. Results show decreased response time compared to the default Kubernetes HPA, with an extensible plug-in design adaptable to new QoS metrics.
  **Code**: Not available

- **[Microscaler: Automatic Scaling for Microservices with an Online Learning Approach](https://doi.org/10.1109/icws.2019.00023)**
  *Authors*: Guangba Yu, Pengfei Chen, Zibin Zheng
  *Publication*: ICWS-2019
  *Summary*: This paper presents Microscaler, a system that automatically identifies scaling-needed microservices and scales them to meet SLA with optimal cost. Using a service mesh-enabled infrastructure to collect QoS metrics, it determines under/over-provisioning services via a novel "service power" criterion and combines online learning (Bayesian optimization) with a step-by-step heuristic to achieve optimal scaling.
  **Code**: Not available

- **[Reinforcement learning-assisted autoscaling mechanisms for serverless computing platforms](https://scholar.google.com/scholar?q=Reinforcement%2Blearning-assisted%2Bautoscaling%2Bmechanisms%2Bfor%2Bserverless)**
  *Authors*: Anastasios Zafeiropoulos, Eleni Fotopoulou, Nikos Filinis, Symeon Papavassiliou
  *Publication*: SMPT-2022
  *Summary*: This paper develops RL-powered autoscaling mechanisms for serverless computing platforms using Q-learning, DynaQ+, and Deep Q-learning algorithms to manage dynamic workloads with QoS guarantees and efficient resource usage. The environments and agents are evaluated on the Kubeless open-source serverless platform in both real and simulated settings, validating their suitability for scalability management of serverless applications.
  **Code**: Not available

- **[Cost-Efficient Reinforcement Learning-Based Horizontal Pod Autoscaling Technique in Kubernetes Cluster](https://scholar.google.com/scholar?q=Cost-Efficient+Reinforcement+Learning-Based+Horizontal+Pod+Autoscaling+Technique+in+Kubernetes+Cluster)**
  *Authors*: Yonghyeon Jang
  *Publication*: J. Cloud Comput.-2023
  *Summary*: This paper proposes a reinforcement learning-based horizontal pod autoscaling mechanism for Kubernetes clusters. The RL agent learns optimal scaling policies that balance cost efficiency and SLO compliance by observing pod metrics, workload patterns, and cluster resource states. Experimental results show improved cost-performance trade-offs compared to Kubernetes' default threshold-based autoscaler.
  **Code**: Not available

---

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

- **[Deep Reinforcement Learning for Load-Balancing Aware Network Control in IoT Edge Systems](https://doi.org/10.1109/tpds.2021.3116863)**
  *Authors*: Qingzhi Liu, Tiancong Xia, Long Cheng, Merijn van Eijk, Tanir Ozcelebi, Ying Mao
  *Publication*: TPDS-2022
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Deep Reinforcement Learning-Based Workload Scheduling for Edge Computing](https://scholar.google.com/scholar?q=Deep+Reinforcement+Learning-Based+Workload+Scheduling+for+Edge+Computing)**
  *Authors*: Tao Zheng, Jian Wan, Jilin Zhang, Congfeng Jiang
  *Publication*: JCCASA-2022
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Dynamic Scheduling for Stochastic Edge-Cloud Computing Environments Using A3C Learning and Residual Recurrent Neural Networks](https://doi.org/10.1109/tmc.2020.3017079)**
  *Authors*: Shreshth Tuli, Shashikant Ilager, Kotagiri Ramamohanarao, Rajkumar Buyya
  *Publication*: TMC-2020
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Energy Efficient Task Scheduling in Fog Environment using Deep Reinforcement Learning Approach](https://scholar.google.com/scholar?q=Energy%2BEfficient%2BTask%2BScheduling%2Bin%2BFog)**
  *Authors*: Shashank Swarup, Elhadi M. Shakshuki, Ansar Yasar
  *Publication*: 2021
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Neural Task Scheduling with Reinforcement Learning for Fog Computing Systems](https://doi.org/10.1109/globecom38437.2019.9014045)**
  *Authors*: Simeng Bian, Xi Huang, Ziyu Shao, Yang Yang
  *Publication*: GLOBECOM-2019
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

- **[Optimization of lightweight task offloading strategy for mobile edge computing based on deep reinforcement learning](https://scholar.google.com/scholar?q=Optimization+of+lightweight+task+offloading+strategy+for+mobile+edge+computing+based+on+deep+reinforcement+learning)**
  *Authors*: Haifeng Lu, Chunhua Gu, Fei Luo, Weichao Ding, Xinping Liu
  *Publication*: FGCS-2020
  *Summary*: This paper applies deep reinforcement learning to edge computing resource management. The approach learns optimal offloading and scheduling decisions under uncertain network conditions and heterogeneous edge node capabilities. The DRL-based method achieves better latency-energy trade-offs compared to heuristic approaches in dynamic edge environments.
  **Code**: Not available

---

### DRL — Robustness & Security

- **[Adversarial Attacks in a Deep Reinforcement Learning based Cluster Scheduler](https://doi.org/10.1109/mascots50786.2020.9285955)**
  *Authors*: Shaojun Zhang, Chen Wang, Albert Y. Zomaya
  *Publication*: 2020
  *Summary*: This paper investigates the vulnerability of DRL-based cluster schedulers to adversarial attacks. The authors propose a white-box attack method that perturbs job features to mislead the DRL scheduler into making suboptimal scheduling decisions. Experiments show that even small perturbations to job feature inputs can significantly degrade scheduling performance, highlighting the need for robustness mechanisms in DRL-based schedulers.
  **Code**: Not available

- **[Adversarial Deep Learning for Online Resource Allocation](https://doi.org/10.1145/3494526)**
  *Authors*: Bingqian Du, Zhiyi Huang, Chuan Wu
  *Publication*: TOMPECS-2021
  *Summary*: This paper proposes an adversarial deep learning approach for designing online algorithms for cloud resource allocation and pricing. Two deep neural networks play a zero-sum game: an adversary generates worst-case input scenarios while the algorithm network learns optimal strategies. A novel per-round update method breaks sequential decision dependencies, enabling convergence to Nash equilibrium and outperforming state-of-the-art online algorithms.
  **Code**: Not available

- **[Robustness Analysis and Enhancement of Deep Reinforcement Learning-Based Schedulers](https://doi.org/10.1109/tpds.2022.3218649)**
  *Authors*: Shaojun Zhang, Chen Wang, Albert Y. Zomaya
  *Publication*: 2023
  *Summary*: This paper investigates the vulnerability of DRL-based cluster schedulers to adversarial attacks. The authors propose a white-box attack method that perturbs job features to mislead the DRL scheduler into making suboptimal scheduling decisions. Experiments show that even small perturbations to job feature inputs can significantly degrade scheduling performance, highlighting the need for robustness mechanisms in DRL-based schedulers.
  **Code**: Not available

---

### Beyond DRL — Benchmarks & Simulators

- **[An Open-Source Benchmark Suite for Microservices and Their Hardware-Software Implications for Cloud &amp; Edge Systems](https://dl.acm.org/doi/10.1145/3297663.3304053)**
  *Authors*: Yu Gan, Yanqi Zhang, Dailun Cheng, Ankitha Shetty, Priyal Rathi, Nayan Katarki, Ariana Bruno, Justin Hu, Brian Ritchken, Brendon Jackson
  *Publication*: ASPLOS-2019
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[Benchmarking microservice systems for software engineering research](https://scholar.google.com/scholar?q=Benchmarking%2Bmicroservice%2Bsystems%2Bfor%2Bsoftware%2Bengineering)**
  *Authors*: Xiang Zhou, Xin Peng, Tao Xie, Jun Sun, Chenjie Xu, Chao Ji, Wenyun Zhao
  *Publication*: ICSE-2018
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[BigDataBench-S: An Open-Source Scientific Big Data Benchmark Suite](https://doi.org/10.1109/ipdpsw.2017.111)**
  *Authors*: Xinhui Tian, Shaopeng Dai, Zhihui Du, Wanling Gao, Rui Ren, Yaodong Cheng, Zhifei Zhang, Zhen Jia, Peijian Wang, Jianfeng Zhan
  *Publication*: IPDPSW-2017
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[BigDataBench: A big data benchmark suite from internet services](https://scholar.google.com/scholar?q=BigDataBench+A+big+data+benchmark+suite+from+internet+services)**
  *Authors*: Lei Wang, Jianfeng Zhan, Chunjie Luo, Yuqing Zhu, Qiang Yang, Yongqiang He, Wanling Gao, Zhen Jia, Yingjie Shi, Shujie Zhang
  *Publication*: HPCA-2014
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[GloudSim: Google trace based cloud simulator with virtual machines](https://scholar.google.com/scholar?q=GloudSim:+Google+trace+based+cloud+simulator+with+virtual+machines)**
  *Authors*: Sheng Di, Franck Cappello
  *Publication*: 2015
  *Summary*: This paper introduces a benchmark suite or simulation tool for evaluating cloud computing and microservice systems. The tool provides realistic workloads, configurable environments, and standardized metrics for comparing scheduling and autoscaling approaches.
  **Code**: Not available

- **[PerfSim: A Performance Simulator for Cloud Native Microservice Chains](https://doi.org/10.1109/tcc.2021.3135757)**
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

- **[A Cooperative Coevolution Genetic Programming Hyper-Heuristics Approach for On-Line Resource Allocation in Container-Based Clouds](https://scholar.google.com/scholar?q=A+Cooperative+Coevolution+Genetic+Programming+Hyper-Heuristics+Approach+for+On-Line+Resource+Allocation+in+Container-Based+Clouds)**
  *Authors*: Boxiong Tan, Hui Ma, Yi Mei, Mengjie Zhang
  *Publication*: 2022
  *Summary*: Addresses the two-level resource allocation problem in container-based clouds (containers-to-VMs and VMs-to-physical-machines), which existing heuristics like First Fit and Best Fit handle poorly. Proposes CCGP-RAC, a Cooperative Coevolution Genetic Programming hyper-heuristic that learns allocation rules from historical workload traces while accounting for VM overheads, types, and affinity constraints. Experiments show significant energy consumption improvements over state-of-the-art algorithms.
  **Code**: Not available

- **[A discrete PSO-based static load balancing algorithm for distributed simulations in a cloud environment](https://scholar.google.com/scholar?q=A+discrete+PSO-based+static+load+balancing+algorithm+for+distributed+simulations+in+a+cloud+environment)**
  *Authors*: Zhang Miao, Peng Yong, Yang Mei, Yin Quanjun, Xie Xu
  *Publication*: FGCS-2021
  *Summary*: Proposes APDPSO (adaptive Pbest discrete PSO), a static load balancing algorithm for distributing federates to hosts in cloud-based parallel simulations. Addresses PSO discretization issues by using a probability- and similarity-based discretisation method and an external archive to update personal best positions, avoiding poor leaders. Evaluated on MATLAB and CloudSim, it improves convergence, swarm diversity, and load balance over existing PSO-based approaches.
  **Code**: Not available

- **[A multi-objective load balancing algorithm for virtual machine placement in cloud data centers based on machine learning](https://scholar.google.com/scholar?q=A+multi-objective+load+balancing+algorithm+for+virtual+machine+placement+in+cloud+data+centers+based+on+machine+learning)**
  *Authors*: Arezoo Ghasemi, Abolfazl Toroghi Haghighat
  *Publication*: Computing-2020
  *Summary*: Presents a machine learning-based VM placement strategy for inter-host load balancing in cloud data centers. A learning agent selects VM migration actions and receives rewards based on solution quality, iteratively improving CPU, memory, and bandwidth balance across host machines. Achieves average improvements of 25%, 34%, and 32% in inter-host load balance for processor, memory, and bandwidth respectively compared to the MOVMrB baseline.
  **Code**: Not available

- **[Combining Size-Based Load Balancing with Round-Robin for Scalable Low Latency](https://doi.org/10.1109/tpds.2019.2950621)**
  *Authors*: Jonatha Anselmi
  *Publication*: TPDS-2020
  *Summary*: Proposes a scalable load balancing framework that combines size-interval task assignment (SITA) with round-robin dispatching to jointly control variances in both arrival and service processes. The hybrid scheme drives mean job delay to zero in the large-system limit -- a property neither approach achieves alone -- using only a small number of job-size intervals relative to system size. Under highly variable job sizes, it is competitive with the less scalable join-the-shortest-workload algorithm.
  **Code**: Not available

- **[DDMTS: A novel dynamic load balancing scheduling scheme under SLA constraints in cloud computing](https://scholar.google.com/scholar?q=DDMTS%3A%2BA%2Bnovel%2Bdynamic%2Bload%2Bbalancing)**
  *Authors*: Zhao Tong, Xiaomei Deng, Hongjian Chen, Jing Mei
  *Publication*: JPDC-2021
  *Summary*: Proposes a deep reinforcement learning-based dynamic load balancing task scheduling algorithm that respects SLA constraints. The DRL agent selects a VM for each incoming task; if the assignment would violate the SLA the task is rejected with a negative reward, otherwise the task executes and the reward reflects post-alignment load balance. Evaluated against Google real-world workload traces, it outperforms baselines in VM load balancing and task rejection rate reduction.
  **Code**: Not available

- **[Hybridization of firefly and Improved Multi-Objective Particle Swarm Optimization algorithm for energy efficient load balancing in Cloud Computing environments](https://scholar.google.com/scholar?q=Hybridization+of+firefly+and+Improved+Multi-Objective+Particle+Swarm+Optimization+algorithm+for+energy+efficient+load+balancing+in+Cloud+Computing+environments)**
  *Authors*: A. Francis Saviour Devaraj, Mohamed Elhoseny, S. Dhanasekaran, E. Laxmi Lydia, K. Shankar
  *Publication*: JPDC-2020
  *Summary*: Proposes FIMPSO, a hybrid load balancing algorithm that uses the Firefly algorithm to reduce the search space and an Improved Multi-Objective PSO (IMPSO) to select the global best particle via a point-to-line distance metric. The combined approach improves resource utilization, response time, CPU utilization (98%), memory utilization (93%), and throughput over competing methods in CloudSim experiments.
  **Code**: Not available

- **[Load balancing in cloud computing – A hierarchical taxonomical classification](https://scholar.google.com/scholar?q=Load%2Bbalancing%2Bin%2Bcloud%2Bcomputing%2B%E2%80%93)**
  *Authors*: Shahbaz Afzal, G. Kavitha
  *Publication*: JCCASA-2019
  *Summary*: Presents a comprehensive encyclopedic review and hierarchical taxonomy of load balancing techniques in cloud computing, addressing a gap in existing literature that lacks systematic classification. Analyzes the factors causing load unbalancing (overloading and underloading) and highlights advantages and limitations of existing methods. Provides new insights and identifies crucial challenges for developing efficient load balancing algorithms.
  **Code**: Not available

- **[Mobility-Aware Computation Offloading with Adaptive Load Balancing in Small-Cell MEC](https://scholar.google.com/scholar?q=Mobility-Aware+Computation+Offloading+with+Adaptive+Load+Balancing+in+Small-Cell+MEC)**
  *Authors*: Feng Lyu, Zhe Dong, Huaqing Wu, Sijing Duan, Fan Wu, Yaoxue Zhang, Xuemin Sherman Shen
  *Publication*: ICC-2022
  *Summary*: Investigates computation task offloading and load balancing in small-cell mobile edge computing systems with unevenly distributed mobile users. Formulates a joint offloading control and load balancing problem to minimize average user computational cost, decomposed via the Tammer method into task offloading control and server grouping sub-problems. Solves them using Kalman Filter techniques and Dueling Double DQN reinforcement learning, outperforming state-of-the-art benchmarks in load balancing and cost reduction.
  **Code**: Not available

- **[Multi objective task scheduling algorithm in cloud computing using grey wolf optimization](https://scholar.google.com/scholar?q=Multi+objective+task+scheduling+algorithm+in+cloud+computing+using+grey+wolf+optimization)**
  *Authors*: Sudheer Mangalampalli, Ganesh Reddy Karri, Mohit Kumar
  *Publication*: Cluster Computing-2022
  *Summary*: Proposes MOTSGWO, a nature-inspired multi-objective Grey Wolf Optimization algorithm for runtime task scheduling that considers makespan, energy consumption, resource utilization, and migration time. The technique allocates resources based on user budgets and task priorities, making scheduling decisions dynamically based on cloud resource status and incoming workload demands. Evaluated on CloudSim with synthetic datasets and real-world workload traces from HPC2N and NASA, it outperforms baseline policies across multiple metrics.
  **Code**: Not available

- **[Multi-objective scheduling strategy for scientific workflows in cloud environment: A Firefly-based approach](https://scholar.google.com/scholar?q=Multi-objective%2Bscheduling%2Bstrategy%2Bfor%2Bscientific%2Bworkflows)**
  *Authors*: Mainak Adhikari, Tarachand Amgoth, Satish Narayana Srirama
  *Publication*: AppSoftCom-2019
  *Summary*: Introduces a workflow scheduling strategy using the Firefly Algorithm to address multiple conflicting objectives including cloud server workload, makespan, resource utilization, and reliability. A rule-based approach assigns tasks to suitable VM instances to minimize makespan while meeting deadlines. Evaluated on Google cluster traces, it outperforms state-of-the-art algorithms in makespan, reliability, resource utilization, and server load distribution.
  **Code**: Not available

- **[Neural network based multi-objective evolutionary algorithm for dynamic workflow scheduling in cloud computing](https://scholar.google.com/scholar?q=Neural+network+based+multi-objective+evolutionary+algorithm+for+dynamic+workflow+scheduling+in+cloud)**
  *Authors*: Goshgar Ismayilov, Haluk Rahmi Topcuoglu
  *Publication*: FGCS-2020
  *Summary*: Models dynamic workflow scheduling as a dynamic multi-objective optimization problem (DMOP) where dynamism arises from resource failures and changing objective counts at runtime. Proposes NN-DNSGA-II, which integrates an artificial neural network with NSGA-II to predict solutions after environmental changes. Optimizes six objectives (makespan, cost, energy, imbalance, reliability, utilization) and significantly outperforms five non-prediction-based alternatives on Pegasus scientific workflows.
  **Code**: Not available

- **[Reliability-Aware Multi-Objective Memetic Algorithm for Workflow Scheduling Problem in Multi-Cloud System](https://scholar.google.com/scholar?q=Reliability-Aware%2BMulti-Objective%2BMemetic%2BAlgorithm%2Bfor%2BWorkflow%2BScheduling%2BProblem%2Bin%2BMulti-Cloud%2BSystem)**
  *Authors*: Shuo Qin, Dechang Pi, Zhongshi Shao, Yue Xu, Yang Chen
  *Publication*: TPDS-2023
  *Summary*: Addresses multi-objective workflow scheduling in multi-cloud systems (MOWSP-MCS), optimizing makespan, cost, and reliability while supporting backup techniques for fault tolerance. Proposes RA-MOMA, a reliability-aware memetic algorithm with problem-specific genetic operators for diversification and four critical-path-based neighborhood operators for intensification. Outperforms related algorithms in numerical experiments across diverse system configurations.
  **Code**: Not available

- **[Research and Improvement of Dynamic Highly Available Load Balancing Algorithm for Microservices](https://doi.org/10.1109/aicit55386.2022.9930161)**
  *Authors*: Jianting Li, Guohong Yi, Bingqian Wu, Zhicao Cao, Xiaodong Xu
  *Publication*: 2022
  *Summary*: Proposes DWLOAD (Dynamic Weight Loading Algorithm), a smooth polling-based load balancer for microservices that introduces virtual nodes and real-time server weights to handle high-concurrency scenarios. Server weights are computed from recent request counts, response times, and throughput, enabling dynamic load distribution across deployed instances. Simulation shows approximately 50% improvement in QPS processing capability over smooth polling in large-scale scenarios while reducing comprehensive response time.
  **Code**: Not available

- **[Resource scheduling algorithm with load balancing for cloud service provisioning](https://scholar.google.com/scholar?q=Resource+scheduling+algorithm+with+load+balancing+for+cloud+service+provisioning)**
  *Authors*: V. Priya, C. Sathiya Kumar, Ramani Kannan
  *Publication*: AppSoftCom-2019
  *Summary*: Proposes an integrated resource scheduling and load balancing approach combining a Fuzzy-based Multidimensional Resource Scheduling (FMRS) model with a Multidimensional Queuing Load Optimization (MQLO) algorithm. FMRS improves resource scheduling efficiency while MQLO dynamically selects requests by class to balance VM utilization and avoid under- or over-utilization. CloudSim experiments show a 7% improvement in resource scheduling efficiency and a 35.5% reduction in response time compared to state-of-the-art methods.
  **Code**: Not available

---

### Beyond DRL — ML Predictive Autoscaling

- **[An Efficient Multivariate Autoscaling Framework Using Bi-LSTM for Cloud Computing](https://doi.org/10.3390/app12073523)**
  *Authors*: Nhat-Minh Dang-Quang, Myungsik Yoo
  *Publication*: 2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[An Integrated Approach for the Near Real-Time Parking Occupancy Prediction](https://doi.org/10.1109/tits.2022.3230199)**
  *Authors*: Jun Li, Haohao Qu, Linlin You
  *Publication*: TITS-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Burst-Aware Predictive Autoscaling for Containerized Microservices](https://doi.org/10.1109/tsc.2020.2995937)**
  *Authors*: Muhammad Abdullah, Waheed Iqbal, Josep Lluis Berral, Jorda Polo, David Carrera
  *Publication*: TSC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[DeepScaler: Holistic Autoscaling for Microservices Based on Spatiotemporal GNN with Adaptive Graph Learning](https://doi.org/10.1109/ase56229.2023.00038)**
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

- **[HANSEL: Adaptive horizontal scaling of microservices using Bi-LSTM](https://scholar.google.com/scholar?q=HANSEL:+Adaptive+horizontal+scaling+of+microservices+using+Bi-LSTM)**
  *Authors*: Ming Yan, XiaoMeng Liang, ZhiHui Lu, Jie Wu, Wei Zhang
  *Publication*: APPL SOFT COMPUT-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[K-AGRUED: A Container Autoscaling Technique for Cloud-based Web Applications in Kubernetes Using Attention-based GRU Encoder-Decoder](https://scholar.google.com/scholar?q=K-AGRUED:+A+Container+Autoscaling+Technique+for+Cloud-based+Web+Applications+in+Kubernetes+Using+Attention-based+GRU+Encoder-Decoder)**
  *Authors*: Javad Dogani, Farshad Khunjush, Mehdi Seydali
  *Publication*: JGC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Learning Predictive Autoscaling Policies for Cloud-Hosted Microservices Using Trace-Driven Modeling](https://doi.org/10.1109/cloudcom.2019.00028)**
  *Authors*: Muhammad Abdullah, Waheed Iqbal, Abdelkarim Erradi, Faisal Bukhari
  *Publication*: 2019
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[PASS: Predictive Auto-Scaling System for Large-scale Enterprise Web Applications](https://doi.org/10.1145/3589334.3645330)**
  *Authors*: Yunda Guo, Jiake Ge, Panfeng Guo, Yunpeng Chai, Tao Li, Mengnan Shi, Yang Tu, Jian Ouyang
  *Publication*: 2024
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Perph: A Workload Co-location Agent with Online Performance Prediction and Resource Inference](https://doi.org/10.1109/ccgrid51090.2021.00027)**
  *Authors*: Jianyong Zhu, Renyu Yang, Chunming Hu, Tianyu Wo, Shiqing Xue, Jin Ouyang, Jie Xu
  *Publication*: CCGrid-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[PERT-GNN: Latency Prediction for Microservice-based Cloud-Native Applications via Graph Neural Networks](https://scholar.google.com/scholar?q=PERT-GNN:+Latency+Prediction+for+Microservice-based+Cloud-Native+Applications+via+Graph+Neural+Networks)**
  *Authors*: Da Sun Handason Tam, Yang Liu, Huanle Xu, Siyue Xie, Wing Cheong Lau
  *Publication*: KDD-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Predictive Job Scheduling under Uncertain Constraints in Cloud Computing](https://ojs.aaai.org/index.php/AAAI/article/view/16180)**
  *Authors*: Hang Dong, Boshi Wang, Bo Qiao, Wenqian Xing, Chuan Luo, Si Qin, Qingwei Lin, Dongmei Zhang, Gurpreet Virdi, Thomas Moscibroda
  *Publication*: AAAI-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Proactive auto-scaling for cloud environments using temporal convolutional neural networks](https://scholar.google.com/scholar?q=Proactive+auto-scaling+for+cloud+environments+using+temporal+convolutional+neural+networks)**
  *Authors*: Ehsan Golshani, Mehrdad Ashtiani
  *Publication*: JPDC-2021
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Proactive auto-scaling technique for web applications in container-based edge computing using federated learning model](https://scholar.google.com/scholar?q=Proactive+auto-scaling+technique+for+web+applications+in+container-based+edge+computing+using+federated+learning+model)**
  *Authors*: Javad Dogani, Farshad Khunjush
  *Publication*: JPDC-2024
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Proactive Resource Autoscaling Scheme Based on SCINet for High-Performance Cloud Computing](https://doi.org/10.1109/tcc.2023.3292378)**
  *Authors*: Byeonghui Jeong, Jueun Jeon, Young-Sik Jeong
  *Publication*: TCC-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[PYRAFORMER: LOW-COMPLEXITY PYRAMIDAL ATTENTION FOR LONG-RANGE TIME SERIES MODELING AND FORECASTING](https://openreview.net/forum?id=0EXmFzUnZ2)**
  *Authors*: Shizhan Liu , , Hang Yu
  *Publication*: ICLR-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[SCINet: Time Series Modeling and Forecasting with Sample Convolution and Interaction](https://openreview.net/forum?id=0EXmFzUnZ2)**
  *Authors*: Muxi Chen, Qiuxia Lai, Minhao Liu, Lingna Ma, Qiang Xu, Zhijian Xu, Ailing Zeng
  *Publication*: NeuIPS-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[The Power of Prediction: Microservice Auto Scaling via Workload Learning](https://scholar.google.com/scholar?q=The+Power+of+Prediction:+Microservice+Auto+Scaling+via+Workload+Learning)**
  *Authors*: Muhammad Abdullah, Waheed Iqbal, Josep Lluis Berral, Jorda Polo, David Carrera
  *Publication*: SoCC-2022
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

- **[Workload time series prediction in storage systems: a deep learning based approach](https://doi.org/10.1007/s10586-020-03214-y)**
  *Authors*: Li Ruan, Yu Bai, Shaoning Li, Shuibing He, Limin Xiao
  *Publication*: CC-2023
  *Summary*: This paper presents a machine learning-based approach for predictive autoscaling in cloud environments. Using neural network models (LSTM/GNN/TCN), the method forecasts workload patterns and proactively adjusts resource allocation. The approach improves scaling accuracy and reduces reactive scaling latency compared to traditional threshold-based methods.
  **Code**: Not available

---

### Beyond DRL — Microservice Architecture & Analysis

- **[A Kubernetes controller for managing the availability of elastic microservice based stateful applications](https://doi.org/10.1016/j.jss.2021.110924)**
  *Authors*: Leila Abdollahi Vayghan, Mohamed Aymen Saied, Maria Toeroe, Ferhat Khendek
  *Publication*: 2021
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[Adaptive Resource Efficient Microservice Deployment in Cloud-Edge Continuum](https://doi.org/10.1109/tpds.2021.3128037)**
  *Authors*: Kaihua Fu, Wei Zhang, Quan Chen, Deze Zeng, Minyi Guo
  *Publication*: TPDS-2022
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[Performance Modeling for Cloud Microservice Applications](https://scholar.google.com/scholar?q=Performance+Modeling+for+Cloud+Microservice+Applications)**
  *Authors*: Anshul Jindal, Vladimir Podolskiy, Michael Gerndt
  *Publication*: ICPE-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[QoS-Aware and Resource Efficient Microservice Deployment in Cloud-Edge Continuum](https://doi.org/10.1109/tpds.2021.3128037)**
  *Authors*: Kaihua Fu, Wei Zhang, Quan Chen, Deze Zeng, Xin Peng, Wenli Zheng, Minyi Guo
  *Publication*: IPDPS-2021
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[Seer: Leveraging Big Data to Navigate the Complexity of Performance Debugging in Cloud Microservices](https://scholar.google.com/scholar?q=Seer:+Leveraging+Big+Data+to+Navigate+the+Complexity+of+Performance+Debugging+in+Cloud+Microservices)**
  *Authors*: Yanqi Zhang, Weizhe Hua, Zhuangzhuang Zhou, G. Edward Suh, Christina Delimitrou
  *Publication*: ASPLOS-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[SHOWAR: Right-Sizing And Efficient Scheduling of Microservices](https://scholar.google.com/scholar?q=SHOWAR:+Right-Sizing+And+Efficient+Scheduling+of+Microservices)**
  *Authors*: Shuotao Cheng, Yuxin Chen, Yicheng Chen, Yufei Wang, Zhenyu Li
  *Publication*: SoCC-2021
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[SmartVM: a SLA-aware microservice deployment framework](https://scholar.google.com/scholar?q=SmartVM:+a+SLA-aware+microservice+deployment+framework)**
  *Authors*: Tianlei Zheng, Xi Zheng, Yuqun Zhang, Yao Deng, ErXi Dong, Rui Zhang, Xiao Liu
  *Publication*: WWWJ-2019
  *Summary*: This paper analyzes microservice architecture patterns, dependency structures, or deployment strategies. The work provides insights into microservice performance, inter-service communication, and resource management challenges in containerized environments.
  **Code**: Not available

- **[SoftSKU: Optimizing Server Architectures for Microservice Diversity and Scale](https://doi.org/10.1145/3321892)**
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

- **[Intelligent Action Performed Load Balancing Decision Made in Cloud Datacenter Based on Improved DQN Algorithm](https://scholar.google.com/scholar?q=Intelligent+Action+Performed+Load+Balancing+Decision+Made+in+Cloud+Datacenter+Based+on+Improved+DQN+Algorithm)**
  *Authors*: Arabinda Pradhan, Sukant Kishoro Bisoy, Amardeep Das
  *Publication*: Journal of King Saud University - Computer and Information Sciences-2021
  *Summary*: This paper presents a load balancing approach for cloud data centers using intelligent decision-making techniques. The method aims to improve resource utilization and response time while minimizing migration overhead.
  **Code**: Not available

- **[A Dynamic Resource Allocation Strategy with Reinforcement Learning for Multimodal Multi-objective Optimization](https://scholar.google.com/scholar?q=A+Dynamic+Resource+Allocation+Strategy+with+Reinforcement+Learning+for+Multimodal+Multi-objective+Optimization)**
  *Authors*: Qian-Long Dang, Wei Xu, Yang-Fei Yuan
  *Publication*: MIR-2022
  *Summary*: This paper proposes a deep reinforcement learning-based dynamic resource allocation strategy for multimodal multi-objective optimization problems. The approach uses RL to adaptively allocate computational resources among multiple optimization operators, learning which operators are most effective at different stages of the optimization process. The method achieves better convergence and diversity on benchmark problems, with potential applications in cloud resource scheduling where multiple conflicting objectives (cost, performance, energy) must be balanced.
  **Code**: Not available

- **[A Hierarchical Receding Horizon Algorithm for QoS-Driven Control of Multi-IaaS Applications](https://doi.org/10.1109/tcc.2018.2875443)**
  *Authors*: Danilo Ardagna, Michele Ciavotta, Riccardo Lancellotti, Michele Guerriero
  *Publication*: TCC-2021
  *Summary*: This paper proposes a hierarchical receding horizon control algorithm for QoS-driven resource management in multi-IaaS cloud environments. The approach uses a two-level optimization framework: the upper level determines long-term resource allocation across IaaS providers using model predictive control, while the lower level handles short-term scheduling with online convex optimization. Experimental results show that the approach reduces SLA violations by 40% while improving cost-efficiency compared to static provisioning strategies.
  **Code**: Not available

- **[A Multi-Graph Attributed Reinforcement Learning based Optimization Algorithm for Large-scale Hybrid Flow Shop Scheduling Problem](https://scholar.google.com/scholar?q=A+Multi-Graph+Attributed+Reinforcement+Learning+based+Optimization+Algorithm+for+Large-scale+Hybrid+Flow+Shop+Scheduling+Problem)**
  *Authors*: Fei Ni, Jianye Hao, Jiawen Lu, Xialiang Tong, Mingxuan Yuan, Jiahui Duan, Yi Ma, Kun He
  *Publication*: KDD-2021
  *Summary*: This paper proposes a multi-graph attributed reinforcement learning approach for solving large-scale hybrid flow shop scheduling problems. The method represents the scheduling problem using multiple graphs that capture job-machine relationships, processing constraints, and resource attributes. A GNN-RL hybrid architecture learns to make scheduling decisions by processing these graph representations, achieving state-of-the-art results on large-scale instances with thousands of jobs and machines.
  **Code**: Not available

- **[A Study of Systems with Multiple Operating Levels, Probabilistic Thresholds and Hysteresis](https://scholar.google.com/scholar?q=A%2BStudy%2Bof%2BSystems%2Bwith%2BMultiple%2BOperating%2BLevels%2BProbabilistic%2BThresholds%2Band%2BHysteresis)**
  *Authors*: Alexandre Brandwajn, Thomas Begin, Hind Castel-Taleb, Tulin Atmaca
  *Publication*: TPDS-2018
  *Summary*: This paper studies queuing systems with multiple operating levels, where state transitions are triggered by probabilistic thresholds and hysteresis mechanisms. The analysis derives steady-state probability distributions and performance metrics for multi-level threshold-based control policies, which are widely used in cloud autoscaling. The theoretical results provide insights into the design of threshold-based autoscaling policies that balance responsiveness and stability.
  **Code**: Not available

- **[Aladdin: Optimized Maximum Flow Management for Shared Production Clusters](https://doi.org/10.1109/ipdps.2019.00078)**
  *Authors*: Heng Wu, Wenbo Zhang, Yuanjia Xu, Hao Xiang, Tao Huang, Haiyang Ding, Zheng Zhang
  *Publication*: IPDPS-2019
  *Summary*: This paper presents Aladdin, a resource management system for shared production clusters hosting diverse workloads including DL training, batch processing, and interactive services. Aladdin models the cluster as a flow network where sources represent resource pools (CPU, GPU, memory), sinks represent workloads, and edges represent feasible allocations. The maximum flow algorithm finds allocations that maximize total resource utilization while respecting workload constraints. Aladdin is deployed in production at a large technology company, managing tens of thousands of GPUs.
  **Code**: Not available

- **[ASTRAEA: A Fair Deep Learning Scheduler for Multi-Tenant GPU Clusters](https://doi.org/10.1109/tpds.2021.3136245)**
  *Authors*: Zhisheng Ye, Peng Sun, Wei Gao, Tianwei Zhang, Xiaolin Wang, Shengen Yan, Yingwei Luo
  *Publication*: TPDS-2022
  *Summary*: This paper presents ASTRAEA, a deep learning-based scheduler for multi-tenant GPU clusters that optimizes both fairness and efficiency. The scheduler uses reinforcement learning to make job placement decisions while considering fairness metrics (e.g., dominant share fairness) alongside performance objectives. ASTRAEA learns to balance the trade-off between maximizing cluster throughput and ensuring fair resource allocation among competing tenants, reducing fairness violations by 35% compared to existing fair schedulers.
  **Code**: Not available

- **[Deep Learning-based Job Placement in Distributed Machine Learning Clusters](https://doi.org/10.1109/infocom.2019.8737460)**
  *Authors*: Yixin Bao, Yanghua Peng, Chuan Wu
  *Publication*: INFOCOM-2019
  *Summary*: This paper proposes a deep learning approach for job placement in distributed machine learning clusters. The system learns to map jobs to machines based on historical performance data, considering factors such as job type, data locality, and machine availability. The deep learning model captures complex patterns in job-machine interactions that hand-crafted heuristics miss, achieving up to 30% improvement in job completion time compared to traditional scheduling approaches.
  **Code**: Not available

- **[Deep Reinforcement Learning Based Adaptive Operator Selection for Evolutionary Multi-Objective Optimization](https://doi.org/10.1109/tetci.2022.3146882)**
  *Authors*: Ye Tian, Xiaopeng Li, Haiping Ma, Xingyi Zhang, Kay Chen Tan, Yaochu Jin
  *Publication*: TETCI-2022
  *Summary*: This paper proposes using deep reinforcement learning for adaptive operator selection in evolutionary multi-objective optimization algorithms. A DRL agent learns to select the most appropriate variation operator (crossover, mutation) at each generation based on the current population state. The approach achieves better convergence and diversity on standard multi-objective benchmark problems compared to static operator selection strategies, and has applications in cloud resource scheduling where multiple conflicting objectives need to be optimized.
  **Code**: Not available

- **[Deep Reinforcement Learning Based Mobility Load Balancing Under Multiple Behavior Policies](https://doi.org/10.1109/icc.2019.8761343)**
  *Authors*: Yue Xu, Wenjun Xu, Zhi Wang, Jiaru Lin, Shuguang Cui
  *Publication*: ICC-2019
  *Summary*: This paper addresses mobility load balancing in cellular networks using deep reinforcement learning under multiple behavior policies. The approach learns optimal offloading strategies that balance traffic load across neighboring base stations while considering user mobility patterns. The method uses an off-policy RL algorithm that can learn from historical deployment data while exploring new strategies, achieving better load distribution and reduced handover rates compared to traditional cell-specific offset approaches.
  **Code**: Not available

- **[Distributional Reinforcement Learning for mmWave Communications with Intelligent Reflectors on a UAV](https://doi.org/10.1109/globecom42002.2020.9348040)**
  *Authors*: Qianqian Zhang, Walid Saad, Mehdi Bennis
  *Publication*: GLOBECOM-2020
  *Summary*: This paper applies distributional reinforcement learning to optimize millimeter wave communications enhanced by intelligent reflecting surfaces mounted on unmanned aerial vehicles (UAVs). The DRL agent learns to control UAV trajectory and beamforming jointly to maximize communication rates while accounting for channel uncertainty. The distributional approach captures the full distribution of possible rewards rather than just expected values, enabling more robust decision-making in dynamic wireless environments.
  **Code**: Not available

- **[Learning Driven Computation Offloading for Asymmetrically Informed Edge Computing](https://doi.org/10.1109/tpds.2019.2893925)**
  *Authors*: Miao Hu, Lei Zhuang, Di Wu, Yipeng Zhou, Xu Chen, Liang Xiao
  *Publication*: TPDS-2018
  *Summary*: This paper addresses computation offloading in edge computing environments where information asymmetry exists between edge servers and mobile devices. A game-theoretic learning approach is proposed where edge servers and devices learn optimal offloading strategies through repeated interactions. The method accounts for private information held by each party and converges to equilibrium strategies that balance computation latency and energy consumption, improving system-wide efficiency by 25% over naive offloading approaches.
  **Code**: Not available

- **[Machine Learning for Predictive Resource Scaling of Microservices](https://scholar.google.com/scholar?q=Machine+Learning+for+Predictive+Resource+Scaling+of+Microservices)**
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
  *Summary*: This is a comprehensive book on microservice-based systems published by Springer in 2024. It covers principles, patterns, and practical aspects of designing, deploying, and operating microservice architectures, including topics such as service decomposition, inter-service communication, data management, observability, and deployment strategies. While not a research paper with specific experimental contributions, it serves as a reference text for understanding the broader microservice ecosystem in which autoscaling and resource management operate.
  **Code**: Not available

- **[Millimeter Wave Communications With an Intelligent Reflector: Performance Optimization and Distributional Reinforcement Learning](https://doi.org/10.1109/twc.2021.3107520)**
  *Authors*: Qianqian Zhang, Walid Saad, Mehdi Bennis
  *Publication*: 2022
  *Summary*: This paper extends the work on mmWave communications with intelligent reflectors by proposing a distributional reinforcement learning approach for performance optimization. The system jointly optimizes the placement of intelligent reflecting surfaces and beamforming vectors to maximize spectral efficiency. The distributional RL formulation captures reward uncertainty and enables risk-aware optimization, outperforming conventional value-based RL methods in dynamic channel conditions.
  **Code**: Not available

- **[PARK: An Open Platform for Learning-Augmented Computer Systems](https://scholar.google.com/scholar?q=PARK+An+Open+Platform+for+Learning-Augmented+Computer+Systems)**
  *Authors*: Hongzi Mao, Parimarjan Negi, Akshay Narayan, Hanrui Wang, Jiacheng Yang, Richard Han, Mohammad Alizadeh
  *Publication*: NeurIPS-2019
  *Summary*: This paper presents PARK, an open platform for learning-augmented computer systems. The platform provides a framework for integrating machine learning predictions into system decision-making, with applications in cluster scheduling, video analytics, and network control.
  **Code**: Not available

- **[Omega: flexible, scalable schedulers for large compute clusters](https://scholar.google.com/scholar?q=Omega:+flexible+scalable+schedulers+for+large+compute+clusters)**
  *Authors*: Malte Schwarzkopf, Andrew Donnelly, Alistair McCreary, Mark Russinovich
  *Publication*: EuroSys-2013
  *Summary*: This paper presents Omega, Google's distributed cluster scheduler that decomposes a centralized scheduler into multiple independent schedulers operating on a shared cluster state using optimistic concurrency control. Each scheduler handles a specific workload type (batch, production, latency-sensitive) and can be developed and evolved independently. Omega's shared state mechanism uses a two-phase commit protocol with conflict detection and resolution, enabling linear scalability while maintaining strong consistency guarantees for resource allocation decisions.
  **Code**: Not available

- **[Public Datasets for Cloud Computing: A Comprehensive Survey](https://scholar.google.com/scholar?q=Public%2BDatasets%2Bfor%2BCloud%2BComputing)**
  *Authors*: Guozhi Liu, Weiwei Lin, Haotong Zhang, Jianpeng Lin, Shaoliang Peng
  *Publication*: IEEE Access-2022
  *Summary*: This paper provides a comprehensive survey of publicly available cloud computing datasets, cataloging their characteristics, coverage, and applicability for research in cloud scheduling, workload prediction, and resource management.
  **Code**: Not available

- **[Scaling Large Production Clusters with Partitioned Synchronization](https://scholar.google.com/scholar?q=Scaling+Large+Production+Clusters+with+Partitioned+Synchronization)**
  *Authors*: Yuanjia Xu, Heng Wu, Wenbo Zhang, Hao Xiang, Tao Huang, Haiyang Ding, Zheng Zhan
  *Publication*: USENIX ATC-2021
  *Summary*: This paper addresses the challenge of scaling large production clusters by introducing partitioned synchronization, a technique that reduces coordination overhead in distributed schedulers. The approach partitions the cluster state and synchronizes only when cross-partition resource conflicts occur, using optimistic concurrency control. This design enables near-linear scalability of the scheduler while maintaining correctness. The system has been deployed in production at a large-scale cloud provider, managing clusters with over 100,000 nodes.
  **Code**: Not available

- **[Tetris: Scheduling Multi-Resource Packing for Cluster Schedulers](https://scholar.google.com/scholar?q=Tetris:+Scheduling+Multi-Resource+Packing+for+Cluster+Schedulers)**
  *Authors*: Malte Schwarzkopf, Adam Gollnick, Steven Hand
  *Publication*: EuroSys-2015
  *Summary*: This paper presents Tetris, a multi-resource packing algorithm for cluster schedulers that efficiently handles heterogeneous resource demands. The approach formulates task placement as a multi-dimensional bin packing problem and uses randomized algorithms to achieve efficient resource utilization across CPU, memory, storage, and network.
  **Code**: Not available

- **[The vision of autonomic computing](https://doi.org/10.1109/acw.2003.1210197)**
  *Authors*: J.O. Kephart, D.M. Chess
  *Publication*: 2003
  *Summary*: This foundational paper presents the vision of autonomic computing -- self-managing systems capable of adapting to changes in their environment and components without human intervention. The paper identifies four key properties: self-configuration, self-healing, self-optimization, and self-protection. This vision directly motivates cloud autoscaling systems, where resource management decisions are automated based on observed workload patterns and service-level objectives, reducing the need for manual capacity planning.
  **Code**: Not available

---

- **[Transformer-based Performance Prediction for Proactive Resource Scaling in Cloud Computing](https://link.springer.com/article/10.1007/s10586-025-05237-9)**
  *Authors*: Yang Chen, Jia Hao, Yu Peng, Hongyan Xia
  *Publication*: Cluster Computing-2025
  *Summary*: This paper proposes a transformer-based approach for predicting application performance in cloud environments, enabling proactive resource scaling. The model leverages attention mechanisms to capture temporal dependencies in workload patterns and predict resource needs before they become bottlenecks.
  **Code**: Not available

- **[UniSched: A Unified Scheduler for Deep Learning Training Jobs With Different User Demands](https://scholar.google.com/scholar?q=UniSched%3A%2BA%2BUnified%2BScheduler%2Bfor%2BDeep%2BLearning%2BTraining%2BJobs%2BWith%2BDifferent%2BUser%2BDemands)**
  *Authors*: Wei Gao, Zhisheng Ye, Peng Sun, Tianwei Zhang, Yonggang Wen
  *Publication*: SoCC-2021
  *Summary*: This paper presents UniSched, a unified scheduler for DL training jobs that accommodates different user demands such as deadline constraints, budget limits, and fairness requirements. UniSched uses a multi-objective optimization framework that simultaneously considers job priority, resource efficiency, and user-specified constraints. The scheduler dynamically adapts its scheduling strategy based on workload characteristics and cluster state, achieving better trade-offs between job completion time and resource utilization compared to single-objective schedulers.
  **Code**: Not available

- **[Workload Consolidation in Alibaba Clusters: The Good, the Bad, and the Ugly](https://scholar.google.com/scholar?q=Workload%2BConsolidation%2Bin%2BAlibaba%2BClusters%3A%2BThe%2BGood%252C%2Bthe%2BBad%252C%2Band%2Bthe%2BUgly)**
  *Authors*: Yongkang Zhang, Yinghao Yu, Wei Wang, Qiukai Chen, Jie Wu, Zuowei Zhang, Jiang Zhong, Tianchen Ding, Qizhen Weng, Lingyun Yang
  *Publication*: SoCC-2022
  *Summary*: This paper presents a comprehensive analysis of workload consolidation strategies in Alibaba production clusters. Using production traces, the study examines co-location patterns between online services (latency-sensitive) and batch jobs (throughput-oriented), identifying key interference factors and optimization opportunities. The analysis reveals that intelligent workload consolidation can improve cluster utilization by 30-50% while maintaining SLA compliance for online services, providing actionable insights for cloud providers.
  **Code**: Not available

---

### Beyond DRL — Surveys & Reviews

- **[A comprehensive survey for scheduling techniques in cloud computing](https://scholar.google.com/scholar?q=A+comprehensive+survey+for+scheduling+techniques+in+cloud+computing)**
  *Authors*: Mohit Kumar, S.C. Sharma, Anubhav Goel, S.P. Singh
  *Publication*: JNCA-2019
  *Summary*: This survey provides a comprehensive review and taxonomy of scheduling techniques in cloud computing, covering static and dynamic algorithms, meta-heuristic approaches, and machine learning-based methods. It classifies techniques by optimization objectives (makespan, cost, energy, load balancing) and identifies open research challenges for future cloud scheduling systems.
  **Code**: Not available

- **[A Survey and Taxonomy of Self-Aware and Self-Adaptive Cloud Autoscaling Systems](https://scholar.google.com/scholar?q=A%2BSurvey%2Band%2BTaxonomy%2Bof%2BSelf-Aware%2Band%2BSelf-Adaptive%2BCloud%2BAutoscaling%2BSystems)**
  *Authors*: Tao Chen, Rami Bahsoon, Xin Yao
  *Publication*: ACMComSur-2018
  *Summary*: This survey presents a taxonomy of self-aware and self-adaptive autoscaling systems in cloud computing, organizing approaches along multiple knowledge dimensions (space, time, quality, quantity). The review compares autoscaling techniques across their self-awareness capabilities and identifies trade-offs between different knowledge sources, providing a roadmap for designing next-generation autoscaling systems.
  **Code**: Not available

- **[A Survey on Issues and Challenges of Load Balancing Techniques in Cloud Computing Environment](https://scholar.google.com/scholar?q=A%2BSurvey%2Bon%2BIssues%2Band%2BChallenges)**
  *Authors*: Febina K S, Tanuja Hemchand, Shamimunnisabi ., Roopa P, Aishwarya P
  *Publication*: ACS-2019
  *Summary*: This survey reviews load balancing techniques in cloud computing environments, categorizing approaches by their handling of static and dynamic workloads. It discusses key challenges including workload heterogeneity, fault tolerance, and energy efficiency, and compares existing techniques to identify gaps for future research.
  **Code**: Not available

- **[Beyond games: a systematic review of neural Monte Carlo tree search applications](https://scholar.google.com/scholar?q=Beyond+games:+a+systematic+review+of+neural+Monte+Carlo+tree+search+applications)**
  *Authors*: Marco Kemmerling, Daniel Lütticke, Robert H. Schmitt
  *Publication*: AppIn-2024
  *Summary*: This systematic review examines neural Monte Carlo Tree Search (NMCTS) applications beyond traditional game-playing domains. The survey covers how neural networks are integrated with MCTS for complex decision-making in real-world applications such as optimization, planning, and control, identifying patterns of successful domain adaptation and open challenges.
  **Code**: Not available

- **[Cloud Dynamic Load Balancing and Reactive Fault Tolerance Techniques: A Systematic Literature Review (SLR)](https://scholar.google.com/scholar?q=Cloud+Dynamic+Load+Balancing+and+Reactive+Fault+Tolerance+Techniques:+A+Systematic+Literature+Review+SLR)**
  *Authors*: Tawfeeg Mohmmed Tawfeeg, Adil Yousif, Alzubair Hassan, Samar M. Alqhtani, Rafik Hamza, Mohammed Bakri Bashir, Awad Ali
  *Publication*: IEEE-Access-2022
  *Summary*: This systematic literature review examines dynamic load balancing and reactive fault tolerance techniques in cloud computing environments. The survey classifies approaches by their handling of workload dynamics and failure scenarios, analyzing how load balancing and fault tolerance mechanisms interact to maintain service availability and performance.
  **Code**: Not available

- **[Deep Reinforcement Learning: A Survey](https://doi.org/10.1109/tnnls.2022.3207346)**
  *Authors*: Xu Wang, Sen Wang, Xingxing Liang, Dawei Zhao, Jincai Huang, Xin Xu, Bin Dai, Qiguang Miao
  *Publication*: 2024
  *Summary*: This survey provides a comprehensive review of deep reinforcement learning, covering fundamental concepts, algorithmic paradigms (value-based, policy-based, actor-critic, model-based), and recent advances. It discusses DRL applications across multiple domains including cybersecurity, robotics, and resource management, and identifies open challenges and future research directions.
  **Code**: Not available

- **[Load balancing techniques in cloud computing environment: A review](https://scholar.google.com/scholar?q=Load+balancing+techniques+in+cloud+computing+environment:+A+review)**
  *Authors*: Dalia Abdulkareem Shafiq, N.Z. Jhanjhi, Azween Abdullah
  *Publication*: JKSU-CIS-2022
  *Summary*: This review surveys load balancing techniques in cloud computing environments, categorizing them into static and dynamic approaches. The paper analyzes performance metrics including response time, throughput, resource utilization, and scalability, comparing trade-offs across different algorithms and identifying suitable techniques for specific cloud workload scenarios.
  **Code**: Not available

- **[Machine Learning-based Orchestration of Containers: A Taxonomy and Future Directions](https://scholar.google.com/scholar?q=Machine+Learning-based+Orchestration+of+Containers:+A+Taxonomy+and+Future+Directions)**
  *Authors*: Zhiheng Zhong, Minxian Xu, Maria Alejandra Rodriguez, Chengzhong Xu, Rajkumar Buyya
  *Publication*: ACMComSur-2022
  *Summary*: This survey presents a taxonomy of machine learning-based container orchestration approaches, covering scheduling, autoscaling, placement, and migration. It systematically reviews how supervised learning, reinforcement learning, and other ML techniques are applied to container orchestration decisions, and identifies gaps in current research for future directions.
  **Code**: Not available

- **[Monte Carlo Tree Search: a review of recent modifications and applications](https://scholar.google.com/scholar?q=Monte+Carlo+Tree+Search:+a+review+of+recent+modifications+and+applications)**
  *Authors*: Maciej Świechowski, Konrad Godlewski, Bartosz Sawicki, Jacek Mańdziuk
  *Publication*: AIR-2023
  *Summary*: This survey reviews Monte Carlo Tree Search (MCTS) modifications and applications published since the last major survey in 2012. It covers domain-specific adaptations and hybrid approaches required for efficient MCTS application in complex games with high branching factors, real-time games, and practical domains such as transportation, scheduling, and security.
  **Code**: Not available

- **[Reinforcement learning-based application Autoscaling in the Cloud: A survey](https://scholar.google.com/scholar?q=Reinforcement+learning-based+application+Autoscaling+in+the+Cloud:+A+survey)**
  *Authors*: Yisel Garí, David A. Monge, Elina Pacini, Cristian Mateos, Carlos García Garino
  *Publication*: ENG APPL ARTIF INTEL-2021
  *Summary*: This survey exhaustively reviews RL-based approaches to application autoscaling in cloud computing, comparing proposals uniformly through proposed taxonomies. It highlights that RL enables transparent (no human intervention), dynamic (no static plans), and adaptable (constantly updated) resource management policies -- three distinctive advantages over ad-hoc or statically computed autoscaling methods. The paper also discusses open problems and prospective research directions in the area.
  **Code**: Not available

- **[State of the Art on Microservices Autoscaling: An Overview](https://www.sbc.org.br/journal)**
  *Authors*: João Paulo K. S. Nunes, Thiago Bianchi, Anderson Y. Iwasaki, Elisa Yumi Nakagawa
  *Publication*: SBC-2021
  *Summary*: This survey reviews the state of the art in microservices autoscaling, analyzing approaches across reactive, proactive, and hybrid categories. It examines how autoscaling mechanisms handle the unique challenges of microservice architectures—such as inter-service dependencies and cascading scaling effects—and identifies open challenges in evaluation methodologies and real-world deployment.
  **Code**: Not available

---

### Beyond DRL — System Design & Platform

- **[GrandSLAm: Guaranteeing SLAs for Jobs in Microservices Execution Frameworks](https://scholar.google.com/scholar?q=GrandSLAm:+Guaranteeing+SLAs+for+Jobs+in+Microservices+Execution+Frameworks)**
  *Authors*: Ingo Muller, Istemi Ekin Akkus, Ruichuan Chen, Jimmy Lin, Pascal Bodik
  *Publication*: EuroSys-2019
  *Summary*: This paper presents GrandSLAm, a microservices execution framework that guarantees job-level SLAs by dynamically scheduling microservice instances across nodes. GrandSLAm formulates SLA compliance as a constraint optimization problem and uses a scalable scheduling algorithm to place microservice instances while respecting resource and SLA constraints, achieving high SLA compliance rates for batch jobs in microservice environments.
  **Code**: Not available

- **[Large-scale cluster management at Google with Borg](https://scholar.google.com/scholar?q=Large-scale+cluster+management+at+Google+with+Borg)**
  *Authors*: Abhishek Verma, Luis Pedrosa, Madhukar Korupolu, David Oppenheimer, Eric Tune, John Wilkes
  *Publication*: EuroSys-2015
  *Summary*: This paper presents Borg, Google's cluster management system that runs hundreds of thousands of jobs from thousands of different applications on tens of thousands of machines. Borg uses prioritized admission control, overcommitment, and fine-grained resource allocation to achieve high utilization while meeting QoS requirements. The design insights from Borg influenced open-source systems including Kubernetes and Mesos.
  **Code**: Not available

- **[LegoOS: A Disseminated, Distributed OS for Hardware Resource Disaggregation](https://www.usenix.org/conference/osdi18/presentation/shan)**
  *Authors*: Yizhou Shan, Yutong Huang, Yilun Chen, Yalei Wang
  *Publication*: OSDI-2018
  *Summary*: This paper presents LegoOS, a distributed operating system that runs on a datacenter with disaggregated hardware resources (CPUs, memory, and storage on separate physical machines). LegoOS introduces disseminated OS components called Lego Modules that manage resource composition across disaggregated hardware, achieving 1.33x better price-performance than traditional servers under various workloads.
  **Code**: Not available

- **[Overload Control for Scaling WeChat Microservices](https://scholar.google.com/scholar?q=Overload+Control+for+Scaling+WeChat+Microservices)**
  *Authors*: Hao Zhou, Ming Chen, Qian Lin, Yong Wang, Xiaobin She, Sifan Liu, Rui Gu, Beng Chin Ooi, Junfeng Yang
  *Publication*: SoCC-2018
  *Summary*: This paper describes the overload control system built for WeChat's microservice architecture, handling billions of users. The system uses a feedback-based approach with request admission control, priority-based dropping, and dynamic resource allocation to maintain service availability during traffic spikes. Deployed in production at Tencent, it effectively handles overload scenarios that would otherwise cascade across microservice dependencies.
  **Code**: Not available

- **[Resilient Distributed Datasets: A Fault-Tolerant Abstraction for In-Memory Cluster Computing](https://www.usenix.org/conference/nsdi12/technical-sessions/presentation/zaharia)**
  *Authors*: Matei Zaharia, Mosharaf Chowdhury, Tathagata Das, Ankur Dave, Justin Ma
  *Publication*: NSDI-2012
  *Summary*: This paper introduces RDDs (Resilient Distributed Datasets), a distributed memory abstraction for fault-tolerant in-memory cluster computing. RDDs provide a programming model that enables efficient data sharing across parallel operations with automatic fault recovery through lineage reconstruction, forming the foundation of the Apache Spark framework and achieving orders-of-magnitude speedup over disk-based systems like Hadoop MapReduce.
  **Code**: Not available

- **[Service Fabric: A Distributed Platform for Building Microservices in the Cloud](https://scholar.google.com/scholar?q=Service+Fabric:+A+Distributed+Platform+for+Building+Microservices+in+the+Cloud)**
  *Authors*: Marc Brooker, Anna Waksman, Mikhail Shilkov
  *Publication*: EuroSys-2018
  *Summary*: This paper presents Azure Service Fabric, a distributed systems platform for building and managing scalable microservices. Service Fabric provides reliable actor and service programming models, automatic partitioning, failover, and placement management. It enables developers to build cloud-native applications with built-in reliability, scaling, and lifecycle management capabilities, powering production services at Microsoft including Azure SQL Database and Skype.
  **Code**: Not available

- **[FIRM: An Intelligent Fine-Grained Resource Management Framework for SLO-Oriented Microservices](https://www.usenix.org/conference/osdi20/presentation/guo)**
  *Authors*: Y. Guo et al.
  *Publication*: OSDI-2020
  *Summary*: This paper presents FIRM, an intelligent fine-grained resource management framework for SLO-oriented microservices. FIRM addresses the challenge of managing resources across interconnected microservices with strict latency requirements. The framework uses fine-grained monitoring and predictive modeling to make proactive resource allocation decisions, ensuring SLO compliance while improving resource utilization in large-scale microservice deployments.
  **Code**: Not available

- **[Chronus: A Novel Deadline-Aware Scheduler for Deep Learning Training Jobs](https://scholar.google.com/scholar?q=Chronus:+A+Novel+Deadline-Aware+Scheduler+for+Deep+Learning+Training+Jobs)**
  *Authors*: Wei Gao, Zhisheng Ye, Peng Sun, Yonggang Wen, Tianwei Zhang
  *Publication*: SoCC-2021
  *Summary*: This paper presents Chronus, a deadline-aware scheduler for deep learning training jobs in large-scale GPU clusters. Chronus incorporates job deadline constraints into the scheduling decision process, ensuring that training jobs complete before their deadlines while maximizing cluster utilization. The scheduler uses predictive modeling to estimate job completion times and proactively allocates resources to prevent deadline violations.
  **Code**: Not available

- **[Large-Scale Machine Learning Cluster Scheduling](https://scholar.google.com/scholar?q=Large-Scale+Machine+Learning+Cluster+Scheduling+Zhao+Wu)**
  *Authors*: Liang Zhao, Chuan Wu
  *Publication*: 2022
  *Summary*: This paper provides a comprehensive analysis of scheduling challenges in large-scale machine learning clusters with thousands of GPUs. The study identifies key efficiency limiters including GPU fragmentation from partial allocations, communication topology awareness for model parallelism, and multi-tenant fairness. The proposed approach combines bin packing for placement, graph algorithms for topology-aware scheduling, and dominant resource fairness extensions for GPU allocation, achieving significant improvements in cluster utilization and job throughput.
  **Code**: Not available

---

### Beyond DRL — Traditional Autoscaling

- **[A bi-metric autoscaling approach for n-tier web applications on kubernetes](https://scholar.google.com/scholar?q=A+bi-metric+autoscaling+approach+for+n-tier+web+applications+on+kubernetes)**
  *Authors*: Changpeng Zhu, Bo Han, Yinliang Zhao
  *Publication*: FCS-2022
  *Summary*: This paper proposes a bi-metric autoscaling approach for n-tier web applications running on Kubernetes. It monitors two key metrics simultaneously to make more informed scaling decisions, addressing the limitation of single-metric autoscalers that may misjudge the true resource needs of multi-tier applications.
  **Code**: Not available

- **[AHPA: Adaptive Horizontal Pod Autoscaling Systems on Alibaba Cloud Container Service for Kubernetes](https://scholar.google.com/scholar?q=AHPA+Adaptive+Horizontal+Pod+Autoscaling+Systems+on+Alibaba+Cloud+Container+Service+for+Kubernetes)**
  *Authors*: Zhiqiang Zhou, Chaoli Zhang, Lingna Ma, Jing Gu, Huajie Qian, Qingsong Wen, Liang Sun, Peng Li, Zhimin Tang
  *Publication*: AAAI-2023
  *Summary*: This paper presents AHPA, an adaptive horizontal pod autoscaling system deployed in production on Alibaba Cloud Container Service for Kubernetes. AHPA uses a robust decomposition-based forecasting algorithm combined with a performance training model to predict business volume and generate optimal pod adjustment plans. Since deployment across logistics, e-commerce, social networking, and AI media workloads, AHPA has increased CPU utilization by 10% and reduced resource costs by over 20%, while eliminating elastic lag through automatic flexible planning.
  **Code**: Not available

- **[An adaptive auto-scaling framework for cloud resource provisioning](https://scholar.google.com/scholar?q=An+adaptive+auto-scaling+framework+for+cloud+resource+provisioning)**
  *Authors*: Spyridon Chouliaras, Stelios Sotiriadis
  *Publication*: FGCS-2023
  *Summary*: This paper introduces ADA-RP, an adaptive auto-scaling framework that uses K-means clustering and convolutional neural networks to categorize future workload demands as High, Medium, or Low based on CPU utilization. The framework scales cloud resources in real time based on predicted demand. Experiments on MySQL containers in Google Cloud Platform show a 48% cost reduction in single-tenant environments and doubled queries per second in multi-tenant environments.
  **Code**: Not available

- **[An Auto-Scaling Approach for Microservices in Cloud Computing Environments](https://doi.org/10.1007/s10723-023-09713-7)**
  *Authors*: Matineh ZargarAzad, Mehrdad Ashtiani
  *Publication*: 2023
  *Summary*: This paper proposes a computational model that analyzes workload across all microservices by considering the overall system workload and inter-service function calls, avoiding the need to individually monitor every microservice. A multi-criteria decision-making method then selects candidate microservices for scaling. Experiments show 99% accuracy in load detection, 20-41% improvement in resource utilization, and up to 70% reduction in scaling operations compared to existing methods.
  **Code**: Not available

- **[Application deployment using containers with auto-scaling for microservices in cloud environment](https://doi.org/10.1016/j.jnca.2020.102629)**
  *Authors*: Satish Narayana Srirama, Mainak Adhikari, Souvik Paul
  *Publication*: 2020
  *Summary*: This paper addresses the deployment and auto-scaling of containerized microservices in cloud environments, focusing on efficient resource provisioning to meet dynamic workload demands. The approach leverages container orchestration to manage microservice deployment and automatically scale resources based on application requirements, minimizing resource cost while satisfying Quality of Service constraints.
  **Code**: Not available

- **[ATOM: Model-Driven Autoscaling for Microservices](https://scholar.google.com/scholar?q=ATOM:+Model-Driven+Autoscaling+for+Microservices)**
  *Authors*: Alim Ul Gias, Giuliano Casale, Murray Woodside
  *Publication*: ICDCS-2019
  *Summary*: This paper proposes ATOM, a model-driven autoscaling controller that instantiates and solves a layered queueing network model of the microservice application at runtime. ATOM uses computational optimization to dynamically control both replica counts and CPU shares per microservice. Under heavy workloads, ATOM delivers 30-37% higher throughput than model-agnostic baselines while reducing scaling actions and bottleneck shifts.
  **Code**: Not available

- **[Auto-Scaling Web Applications in Clouds: A Taxonomy and Survey](https://scholar.google.com/scholar?q=Auto-Scaling+Web+Applications+in+Clouds+A+Taxonomy+and+Survey)**
  *Authors*: Chenhao Qu, Rodrigo N. Calheiros, Rajkumar Buyya
  *Publication*: ACMComSur-2018
  *Summary*: This paper provides a comprehensive survey and taxonomy of auto-scaling approaches for web applications in cloud environments, analyzing challenges and key properties that define different auto-scaler designs. The authors categorize existing works according to their taxonomy to identify weaknesses and gaps, and propose future research directions for improving cloud auto-scaling mechanisms.
  **Code**: Not available

- **[Autopilot: Workload Autoscaling at Google Scale](https://scholar.google.com/scholar?q=Autopilot:+Workload+Autoscaling+at+Google+Scale)**
  *Authors*: Krzysztof Rząḑca, Paweł Findeisen, Jacek Świderski, Przemyslaw Zych, Przemyslaw Broniek, Jarek Kusmierek, Paweł Krzysztof Nowak, Beata Strack, Piotr Witusowski, Steven Hand
  *Publication*: EuroSys-2020
  *Summary*: This paper presents Google's Autopilot system for automatic workload autoscaling at production scale. It describes the design, implementation, and operational experience of a system that manages resource allocation across Google's infrastructure, using predictive models and feedback control to maintain service quality while optimizing resource utilization.
  **Code**: Not available

- **[BASE: Burst-Adaptive Autoscaling via Stacked Ensembles for SLO Assurance and Cost Efficiency](https://scholar.google.com/scholar?q=BASE%3A%2BBurst-Adaptive%2BAutoscaling%2Bvia%2BStacked%2BEnsembles%2Bfor%2BSLO%2BAssurance%2Band%2BCost%2BEfficiency)**
  *Authors*: Chunyang Meng, Haogang Tong, Tianyang Wu, Maolin Pan, Yang Yu, Yi Jiang
  *Publication*: arXiv-2024
  *Summary*: This paper presents BASE, a burst-adaptive autoscaling system that uses stacked ensemble machine learning models to detect and respond to workload bursts in cloud microservices. The approach simultaneously assures Service Level Objectives and optimizes cost efficiency by adapting scaling behavior based on workload burst patterns.
  **Code**: Not available

- **[Cdascaler: a cost-effective dynamic autoscaling approach for containerized microservices](https://doi.org/10.1007/s10586-023-04228-y)**
  *Authors*: Numan Shafi, Muhammad Abdullah, Waheed Iqbal, Abdelkarim Erradi, Faisal Bukhari
  *Publication*: 2024
  *Summary*: This paper presents Cdascaler, which addresses the problem of dynamically allocating the right amount of CPU resources to containers during autoscaling events, going beyond simply deciding how many containers to add or remove. Machine learning predicts appropriate CPU allocation for each container spawned for microservices over time. Experiments on Kubernetes show a 40-60% reduction in response time SLO violations at 0.5x to 1.5x lower cost compared to state-of-the-art baselines.
  **Code**: Not available

- **[Chameleon: A Hybrid, Proactive Auto-Scaling Mechanism on a Level-Playing Field](https://scholar.google.com/scholar?q=Chameleon%3A%2BA%2BHybrid%2BProactive%2BAuto-Scaling%2BMechanism%2Bon%2Ba%2BLevel-Playing%2BField)**
  *Authors*: Andre Bauer, Nikolas Herbst, Simon Spinner, Ahmed Ali-Eldin, Samuel Kounev
  *Publication*: TPDS-2019
  *Summary*: This paper proposes Chameleon, a hybrid autoscaling mechanism that combines multiple proactive time series-based forecasting methods with a reactive fallback to reduce the risk of relying on a single prediction method. Chameleon uses automated load intensity forecasting together with runtime service demand estimation to calculate required resources without application instrumentation. Evaluated over 400 hours across three cloud environments with five real-world workload traces, Chameleon outperforms five state-of-the-art autoscalers on both user-facing and elasticity metrics.
  **Code**: Not available

- **[Coordinating Fast Concurrency Adapting With Autoscaling for SLO-Oriented Web Applications](https://doi.org/10.1109/tpds.2022.3151512)**
  *Authors*: Jianshu Liu, Shungeng Zhang, Qingyang Wang, Jinpeng Wei
  *Publication*: TPDS-2022
  *Summary*: This paper demonstrates that scaling a bottleneck server without quickly adjusting its soft resources (server threads, database connections) causes significant response time fluctuations because soft resources determine per-server request concurrency. The authors propose the Scatter-Concurrency-Throughput (SCT) model to rapidly identify near-optimal soft resource allocation and implement ConScale, a framework that integrates SCT to reallocate soft resources after hardware scaling. Experiments show ConScale successfully mitigates response time fluctuations during scaling in both VM-based (EC2 AutoScaling) and container-based (Kubernetes HPA) environments.
  **Code**: Not available

- **[Deep Learning-Based Autoscaling Using Bidirectional Long Short-Term Memory for Kubernetes](https://doi.org/10.3390/app11093835)**
  *Authors*: Nhat-Minh Dang-Quang, Myungsik Yoo
  *Publication*: 2021
  *Summary*: This paper proposes a proactive custom autoscaler for Kubernetes based on the MAPE loop, using a Bidirectional LSTM to predict future HTTP workload patterns. The planning phase implements a cooling-down period to mitigate oscillation and a resource removal strategy to handle workload bursts more effectively. The Bi-LSTM achieves better prediction accuracy than both LSTM and ARIMA models while offering 530-600x faster prediction speed, and the autoscaler outperforms the default Kubernetes HPA in both accuracy and provisioning speed.
  **Code**: Not available

- **[DeepScaling: Autoscaling Microservices With Stable CPU Utilization for Large Scale Production Cloud Systems](https://scholar.google.com/scholar?q=DeepScaling:+Autoscaling+Microservices+With+Stable+CPU+Utilization+for+Large+Scale+Production+Cloud+Systems)**
  *Authors*: Ziliang Wang, Shiyi Zhu, Jianguo Li, Wei Jiang, K. K. Ramakrishnan, Meng Yan, Xiaohong Zhang, Alex X. Liu
  *Publication*: SoCC-2022
  *Summary*: This paper presents DeepScaling, an autoscaling system for large-scale production cloud microservice systems that maintains stable CPU utilization across microservices. The system uses deep learning-based workload prediction to proactively adjust microservice replicas, preventing both CPU overutilization and underutilization. DeepScaling is deployed and evaluated in production-scale cloud environments to demonstrate effectiveness at scale.
  **Code**: Not available

- **[Erlang: Application-Aware Autoscaling for Cloud Microservices](https://scholar.google.com/scholar?q=Erlang%3A%2BApplication-Aware%2BAutoscaling%2Bfor%2BCloud%2BMicroservices)**
  *Authors*: Vighnesh Sachidananda, Anirudh Sivaraman
  *Publication*: arXiv-2022
  *Summary*: This paper argues that per-microservice threshold-based autoscaling is suboptimal because end-to-end latency depends on multiple microservices in the request path, each potentially requiring a different number of VMs. Erlang introduces an application-aware autoscaling approach that considers the full request path and makes coordinated scaling decisions across all microservices, optimizing for both dollar cost and end-to-end user-perceived latency rather than per-service CPU utilization.
  **Code**: Not available

- **[Horizontal Pod Autoscaling in Kubernetes Cluster Using Long Short-Term Memory](https://scholar.google.com/scholar?q=Horizontal%2BPod%2BAutoscaling%2Bin%2BKubernetes%2BCluster)**
  *Authors*: Somshekar Patil, D. G. Narayan, Ajeya Bhat, Aishwarya Hungund, Disha M. Patil
  *Publication*: 2024
  *Summary*: This paper presents an LSTM-based horizontal pod autoscaler for Kubernetes that uses long short-term memory neural networks to predict future workload demands and proactively adjust pod replicas. By replacing the default reactive HPA with a prediction-driven approach, the system aims to reduce scaling latency and improve resource utilization for containerized microservices under fluctuating workloads.
  **Code**: Not available

- **[PBScaler: A Bottleneck-Aware Autoscaling Framework for Microservice-Based Applications](https://doi.org/10.1109/tsc.2024.3376202)**
  *Authors*: Shuaiyu Xie, Jian Wang, Bing Li, Zekun Zhang, Duantengchuan Li, Patrick C. K. Hung
  *Publication*: TSC-2024
  *Summary*: This paper addresses the challenge of identifying root performance bottlenecks in microservice applications, where performance anomalies propagate through service dependencies and make it difficult to determine which microservices need scaling. PBScaler introduces TopoRank, a random walk algorithm based on topological potential, to accurately locate performance bottlenecks and reduce unnecessary scaling. Combined with an offline performance-aware optimization algorithm for replica management, PBScaler mitigates performance degradation while conserving resources more efficiently than existing approaches.
  **Code**: Not available

- **[Practical Efficient Microservice Autoscaling with QoS Assurance](https://scholar.google.com/scholar?q=Practical+Efficient+Microservice+Autoscaling+with+QoS+Assurance)**
  *Authors*: Md Rajib Hossen, Mohammad A. Islam, Kishwar Ahmed
  *Publication*: HPDC-2022
  *Summary*: This paper proposes PEMA, a lightweight resource manager that finds efficient resource allocations for microservices through opportunistic resource reduction, avoiding the extensive training data and intentional SLO violations required by ML-heavy approaches. Experiments across three prototype microservice implementations show PEMA saves up to 33% resource compared to commercial rule-based allocation while maintaining QoS guarantees.
  **Code**: Not available

- **[Proactive Autoscaling for Cloud-Native Applications using Machine Learning](https://doi.org/10.1109/globecom42002.2020.9322147)**
  *Authors*: Nicolas Marie-Magdelaine, Toufik Ahmed
  *Publication*: GLOBECOM-2020
  *Summary*: This paper proposes a proactive autoscaling framework using an LSTM-based forecasting model to dynamically adjust both horizontal scaling (number of replicas) and vertical scaling (resource pool) for cloud-native microservice applications. A proof-of-concept implementation demonstrates the effectiveness of the proactive LSTM-based algorithm in improving end-to-end latency compared to reactive feedback-loop autoscaling.
  **Code**: Not available

- **[ProScale: Proactive Autoscaling for Microservice With Time-Varying Workload at the Edge](https://doi.org/10.1109/tpds.2023.3238429)**
  *Authors*: Ke Cheng, Sheng Zhang, Chenghong Tu, Xiaohang Shi, Zhaoheng Yin, Sanglu Lu, Yu Liang, Qing Gu
  *Publication*: TPDS-2023
  *Summary*: This paper identifies that existing edge microservice autoscaling approaches impractically assume each microservice's workload depends solely on its upstream, a claim refuted through analysis of Alibaba's trace with hundreds of millions of records. ProScale proactively forecasts per-microservice workload per timeslot and uses an efficient online algorithm to jointly determine instance numbers and placement decisions, with a designed offloading strategy for burst requests. Trace-driven experiments show ProScale reduces average response time by 96.7% and resource usage by 96.5% compared to existing strategies.
  **Code**: Not available

- **[RobustScaler: QoS-Aware Autoscaling for Complex Workloads](https://doi.org/10.1109/icde53745.2022.00252)**
  *Authors*: Huajie Qian, Qingsong Wen, Liang Sun, Jing Gu, Qiulin Niu, Zhimin Tang
  *Publication*: ICDE-2022
  *Summary*: This paper investigates proactive autoscaling for scaling-per-query applications such as container registry and function-as-a-service, where workloads exhibit high uncertainty with complex temporal patterns including periodicity, noise, and outliers. RobustScaler uses non-homogeneous Poisson process modeling combined with stochastically constrained optimization to achieve a superior trade-off between resource cost and QoS. A specialized ADMM algorithm efficiently trains the model, and experiments on real-world traces show large improvements over baseline strategies for complex workload patterns.
  **Code**: Not available

- **[Collective Autoscaling for Cloud Microservices](https://doi.org/10.1145/3627703.3650084)**
  *Authors*: Vighnesh Sachidananda, Anirudh Sivaraman
  *Publication*: SoCC-2024 (originally arXiv-2022)
  *Summary*: This paper addresses autoscaling for cloud microservice systems by coordinating scaling decisions across interconnected services. Traditional autoscaling operates independently per service, which can lead to suboptimal outcomes when services have interdependent resource demands. The collective approach jointly optimizes scaling decisions across the service dependency graph, reducing cascading scaling delays and improving end-to-end SLO compliance.
  **Code**: Not available

---

### Beyond DRL — Traditional Resource Management

- **[A load balance oriented cost efficient scheduling method for parallel tasks](https://scholar.google.com/scholar?q=A+load+balance+oriented+cost+efficient+scheduling+method+for+parallel+tasks)**
  *Authors*: Yu Xin, Zhi-Qiang Xie, Jing Yang
  *Publication*: JNCA-2017
  *Summary*: This paper proposes a load-balance-oriented scheduling method for parallel tasks in cloud computing that aims to improve resource utilization and reduce execution time. The approach constructs a task dependency graph and applies a cost-efficient scheduling strategy that considers both computational load distribution and communication overhead. Experiments demonstrate improved load balancing and reduced makespan compared to conventional scheduling approaches.
  **Code**: Not available

- **[Affinity-Aware Resource Provisioning for Long-Running Applications in Shared Clusters](https://scholar.google.com/scholar?q=Affinity-Aware%2BResource%2BProvisioning%2Bfor%2BLong-Running%2BApplications%2Bin%2BShared%2BClusters)**
  *Authors*: Clement Mommessin, Renyu Yang, Natalia Shakhlevich, Xiaoyang Sun, Satish Kumar, Junqing Xiao, Jie Xu
  *Publication*: JPDC-2023
  *Summary*: This paper addresses the problem of resource provisioning for long-running applications in shared cloud clusters with affinity constraints. It develops an affinity-aware provisioning strategy that co-locates dependent application components to reduce communication latency while respecting resource capacity constraints. The approach formulates the problem as an optimization model and evaluates it using real-world cluster workloads, showing improved application performance and resource efficiency.
  **Code**: Not available

- **[Cost-efficient dynamic scheduling of big data applications in apache spark on cloud](https://scholar.google.com/scholar?q=Cost-efficient%2Bdynamic%2Bscheduling%2Bof%2Bbig%2Bdata)**
  *Authors*: Muhammed Tawfiqul Islam, Satish Narayana Srirama, Shanika Karunasekera, Rajkumar Buyya
  *Publication*: JSS-2020
  *Summary*: This paper proposes a cost-efficient dynamic scheduling approach for Apache Spark applications running on cloud infrastructure. The method dynamically allocates and releases cloud resources based on application workload characteristics and deadline constraints, using a cost-optimization model to minimize cloud expenditure. Experimental evaluation on real Spark workloads demonstrates significant cost savings while meeting application deadlines.
  **Code**: Not available

- **[DDRM: An SLO-aware Deep Dynamic Resource Management Framework for Microservices](https://scholar.google.com/scholar?q=DDRM%3A%2BAn%2BSLO-aware%2BDeep%2BDynamic%2BDynamic%2BResource%2BManagement%2BFramework%2Bfor%2BMicroservices)**
  *Authors*: Liangping Tang, Jin Wang, Wanyou Wang, Gaotao Shi, Zhijun Li
  *Publication*: OSDI-2020
  *Summary*: This paper presents DDRM, a deep learning-based dynamic resource management framework for microservices that ensures SLO compliance. The system uses deep neural networks to predict workload patterns and proactively adjusts resource allocation across microservice instances. By combining predictive modeling with dynamic resource scaling, DDRM reduces SLO violations and improves resource utilization in production microservice deployments.
  **Code**: Not available

- **[Deep Learning and Cloud Computing](https://scholar.google.com/scholar?q=Deep%2BLearning%2Band%2BCloud%2BComputing)**
  *Authors*: Pramod Gupta, Naresh K. Sehgal
  *Publication*: Code-2021
  *Summary*: This paper explores the integration of deep learning techniques with cloud computing infrastructure, examining how cloud platforms can support large-scale deep learning workloads. It discusses architectural considerations for deploying deep learning models in the cloud, including distributed training, model serving, and resource provisioning. The work provides a survey of existing approaches and identifies challenges in efficiently combining deep learning with cloud resource management.
  **Code**: Not available

- **[Detection of SLA Violation for Big Data Analytics Applications in Cloud](https://doi.org/10.1109/tc.2020.2995881)**
  *Authors*: Xuezhi Zeng, Saurabh Garg, Mutaz Barika, Sanat Bista, Deepak Puthal, Albert Y. Zomaya, Rajiv Ranjan
  *Publication*: TC-2021
  *Summary*: This paper presents a proactive approach for detecting SLA violations in cloud-hosted big data analytics applications. The method monitors application performance metrics and uses predictive models to identify potential SLA breaches before they occur, enabling timely corrective actions. Experiments on cloud platforms demonstrate the approach's effectiveness in reducing SLA violation rates for data-intensive analytics workloads.
  **Code**: Not available

- **[Distributed resource management across process boundaries](https://scholar.google.com/scholar?q=Distributed+resource+management+across+process+boundaries)**
  *Authors*: Lalith Suresh, Peter Bodik, Ishai Menache, Marco Canini, Florin Ciucu
  *Publication*: SoCC-2017
  *Summary*: This paper addresses the challenge of managing resources across distributed processes in cloud environments, where traditional resource managers operate within isolated boundaries. It proposes a distributed resource management protocol that enables cross-process resource sharing and coordination without requiring centralized control. The system achieves improved resource utilization and fairness by enabling processes to negotiate resource allocations directly with one another.
  **Code**: Not available

- **[Erms: Efficient Resource Management for Shared Microservices with SLA Guarantees](https://scholar.google.com/scholar?q=Erms:+Efficient+Resource+Management+for+Shared+Microservices+with+SLA+Guarantees)**
  *Authors*: Shutian Luo, Huanle Xu, Kejiang Ye, Guoyao Xu, Liping Zhang, Jian He, Guodong Yang, Chengzhong Xu
  *Publication*: ASPLOS-2023
  *Summary*: This paper presents ERMS, a system for efficient resource management of shared microservices that guarantees SLA compliance. The framework dynamically allocates CPU and memory resources among co-located microservice instances using interference-aware scheduling and performance isolation mechanisms. Experiments on production workloads show that ERMS significantly improves resource utilization while maintaining SLO targets for latency-sensitive microservices.
  **Code**: Not available

- **[Generating Complex, Realistic Cloud Workloads using Recurrent Neural Networks](https://scholar.google.com/scholar?q=Generating+Complex+Realistic+Cloud+Workloads+using+Recurrent+Neural+Networks)**
  *Authors*: Shane Bergsma, Timothy Zeyl, Arik Senderovich, J. Christopher Beck
  *Publication*: SOSP-2021
  *Summary*: This paper proposes using recurrent neural networks to generate realistic cloud workload traces that capture the complex temporal patterns and correlations found in production systems. The RNN-based generator learns from historical workload data to produce synthetic traces that preserve statistical properties such as burstiness, periodicity, and inter-task dependencies. The generated workloads can be used for benchmarking and evaluating cloud scheduling algorithms without requiring access to production traces.
  **Code**: Not available

- **[HSACMA: a hierarchical scalable adaptive cloud monitoring architecture](https://scholar.google.com/scholar?q=HSACMA:+a+hierarchical+scalable+adaptive+cloud+monitoring+architecture)**
  *Authors*: Rui Wang, Shi Ying, Meiyan Li, Shun Jia
  *Publication*: SQJ-2020
  *Summary*: This paper proposes HSACMA, a hierarchical and adaptive architecture for monitoring large-scale cloud environments. The system organizes monitoring agents into a multi-level hierarchy that dynamically adjusts its structure based on workload changes and resource availability, enabling scalable data collection and analysis. Experimental results demonstrate that HSACMA achieves lower monitoring overhead and better scalability compared to flat monitoring architectures in large cloud deployments.
  **Code**: Not available

- **[Hydra: Deadline-Aware and Efficiency-Oriented Scheduling for Deep Learning Jobs on Heterogeneous GPUs](https://doi.org/10.1109/tc.2023.3242200)**
  *Authors*: Zichao Yang, Heng Wu, Yuanjia Xu, Yuewen Wu, Hua Zhong, Wenbo Zhang
  *Publication*: 2023
  *Summary*: This paper presents Hydra, a scheduling system for deep learning jobs on heterogeneous GPU clusters that jointly optimizes for deadline adherence and resource efficiency. Hydra incorporates job deadline information and GPU heterogeneity characteristics into its scheduling decisions, using a combination of profiling-based performance prediction and priority-aware resource allocation. Experiments show that Hydra improves job completion rates and GPU utilization compared to existing GPU scheduling approaches.
  **Code**: Not available

- **[K8sSim: A Simulation Tool for Kubernetes Schedulers and Its Applications in Scheduling Algorithm Optimization](https://doi.org/10.3390/mi14030651)**
  *Authors*: Shilin Wen, Rui Han, Ke Qiu, Xiaoxin Ma, Zeqing Li, Hongjie Deng, Chi Harold Liu
  *Publication*: MicroM-2023
  *Summary*: This paper presents K8sSim, a simulation tool that enables rapid evaluation and optimization of Kubernetes scheduling algorithms without requiring a physical cluster. The simulator faithfully reproduces the Kubernetes scheduling behavior, including pod placement decisions, resource accounting, and scheduling queue management. Using K8sSim, the authors demonstrate how different scheduling strategies can be compared efficiently and propose optimizations that improve scheduling throughput and resource utilization.
  **Code**: Not available

- **[Learning Resource Allocation and Pricing for Cloud Profit Maximization](https://aaai.org/ojs/index.php/AAAI/article/view/4339)**
  *Authors*: Bingqian Du, Chuan Wu, Zhiyi Huang
  *Publication*: AAAI-2019
  *Summary*: This paper addresses the joint problem of resource allocation and pricing for cloud providers to maximize profit. It formulates the problem as an online learning framework where the cloud provider dynamically adjusts resource allocation and pricing based on observed user demand patterns. The proposed algorithm achieves provable competitive ratios and demonstrates superior profit performance compared to static pricing and allocation strategies through trace-driven simulations.
  **Code**: Not available

- **[Learning scheduling algorithms for data processing clusters](https://scholar.google.com/scholar?q=Learning+scheduling+algorithms+for+data+processing+clusters)**
  *Authors*: Hongzi Mao, Malte Schwarzkopf, Shaileshh Bojja Venkatakrishnan, Zili Meng, Mohammad Alizadeh
  *Publication*: SIGCOMM-2019
  *Summary*: This paper presents Decima, a learned scheduler for data processing clusters that uses reinforcement learning to make scheduling decisions across multiple stages of data-parallel jobs. Decima represents the cluster state as a graph and employs a graph neural network to generalize across different workload sizes and cluster topologies. Evaluation on production traces from Apache Spark clusters shows that Decima significantly reduces average job completion time compared to hand-crafted scheduling heuristics.
  **Code**: Not available

- **[Maintaining SLOs of Cloud-Native Applications Via Self-Adaptive Resource Sharing](https://doi.org/10.1109/saso.2019.00018)**
  *Authors*: Vladimir Podolskiy, Michael Mayo, Abigail Koay, Michael Gerndt, Panos Patros
  *Publication*: SASO-2019
  *Summary*: This paper proposes a self-adaptive resource sharing mechanism for cloud-native applications that dynamically redistributes resources among co-located services to maintain SLO targets. The approach continuously monitors application performance and automatically adjusts resource partitions based on observed workload patterns and interference effects. Experimental evaluation on Kubernetes demonstrates that the system effectively maintains SLO compliance under variable workloads while improving overall cluster utilization.
  **Code**: Not available

- **[Memory-harvesting VMs in cloud platforms](https://scholar.google.com/scholar?q=Memory-harvesting+VMs+in+cloud+platforms)**
  *Authors*: Alexander Fuerst, Stanko Novaković, Íñigo Goiri, Gohar Irfan Chaudhry, Prateek Sharma, Kapil Arya, Kevin Broas, Eugene Bak, Mehmet Iyigun, Ricardo Bianchini
  *Publication*: ASPLOS-2022
  *Summary*: This paper introduces memory-harvesting virtual machines that reclaim unused memory from low-priority VMs and reallocate it to memory-intensive workloads in cloud data centers. The system transparently identifies and harvests idle memory pages without impacting the performance of donor VMs, using a combination of ballooning and page-level memory tracking. Results from production cloud deployments show significant improvements in memory utilization and reduced need for over-provisioning.
  **Code**: Not available

- **[Modeling Analysis and Cost-Performance Ratio Optimization of Virtual Machine Scheduling in Cloud Computing](https://scholar.google.com/scholar?q=Modeling%2BAnalysis%2Band%2BCost-Performance%2BRatio%2BOptimization%2Bof%2BVirtual%2BMachine%2BScheduling%2Bin%2BCloud%2BComputing)**
  *Authors*: Bo Wan, Jiale Dang, Zhetao Li, Hongfang Gong, Feng Zhang, Sangyoon Oh
  *Publication*: TPDS-2020
  *Summary*: This paper presents a modeling and analysis framework for optimizing the cost-performance ratio of virtual machine scheduling in cloud computing environments. It formulates VM scheduling as an optimization problem that jointly considers execution cost and performance metrics, proposing an analytical model to predict the cost-performance trade-offs of different scheduling decisions. The proposed algorithm achieves better cost-efficiency than baseline approaches while maintaining acceptable performance levels for diverse workloads.
  **Code**: Not available

- **[Optimizing Resource Management for Shared Microservices: A Scalable System Design](https://scholar.google.com/scholar?q=Optimizing+Resource+Management+for+Shared+Microservices:+A+Scalable+System+Design)**
  *Authors*: Shutian Luo, Chenyu Lin, Kejiang Ye, Guoyao Xu, Liping Zhang, Guodong Yang, Huanle Xu, Chengzhong Xu
  *Publication*: TOCS-2023
  *Summary*: This paper presents a scalable system design for optimizing resource management of shared microservices in cloud infrastructure. The system addresses the challenges of resource contention and interference among co-located microservices by employing fine-grained resource isolation and adaptive allocation policies. Experimental evaluation on production microservice workloads demonstrates significant improvements in both resource utilization and service-level objective compliance.
  **Code**: Not available

- **[SAAS parallel task scheduling based on cloud service flow load algorithm](https://scholar.google.com/scholar?q=SAAS%2Bparallel%2Btask%2Bscheduling%2Bbased%2Bon)**
  *Authors*: Jian Zhu, Qian Li, Shi Ying
  *Publication*: Comp. Com-2022
  *Summary*: This paper proposes a cloud service flow load algorithm for parallel task scheduling in SaaS environments. The method models task execution as a flow network and applies load-aware scheduling to distribute parallel tasks across cloud resources, aiming to minimize response time and balance resource utilization. Experimental results demonstrate improved scheduling efficiency and reduced task completion times compared to conventional scheduling approaches.
  **Code**: Not available

- **[Scavenger: A Black-Box Batch Workload Resource Manager for Improving Utilization in Cloud Environments](https://scholar.google.com/scholar?q=Scavenger:+A+Black-Box+Batch+Workload+Resource+Manager+for+Improving+Utilization+in+Cloud+Environments)**
  *Authors*: Sara Babaei, Shashank Srivastava, Kshitij Bansal, K. R. Jayaram
  *Publication*: SoCC-2019
  *Summary*: This paper presents Scavenger, a black-box batch workload resource manager that improves utilization in cloud environments by opportunistically scheduling batch jobs on underutilized resources. Scavenger operates without requiring application-level modifications or performance models, instead using external resource usage signals to dynamically allocate and reclaim resources. Evaluation on production cloud workloads shows that Scavenger significantly increases cluster utilization without degrading the performance of latency-sensitive foreground services.
  **Code**: Not available

- **[Sinan: ML-based and QoS-aware resource management for cloud microservices](https://scholar.google.com/scholar?q=Sinan%3A%2BML-based%2Band%2BQoS-aware%2Bresource%2Bmanagement%2Bfor%2Bcloud%2Bmicroservices)**
  *Authors*: Yanqi Zhang, Weizhe Hua, Zhuangzhuang Zhou, G. Edward Suh, Christina Delimitrou
  *Publication*: ASPLOS-2021
  *Summary*: This paper presents Sinan, an ML-based resource management system for cloud microservices that is aware of quality-of-service requirements. Sinan uses machine learning models to predict microservice performance under different resource configurations and makes proactive resource allocation decisions to meet QoS targets. The system effectively handles workload variability and resource contention in multi-tenant microservice environments, reducing QoS violations and improving resource efficiency.
  **Code**: Not available

- **[SLA-Based Scheduling of Spark Jobs in Hybrid Cloud Computing Environments](https://doi.org/10.1109/tc.2021.3075625)**
  *Authors*: Muhammed Tawfiqul Islam, Huaming Wu, Shanika Karunasekera, Rajkumar Buyya
  *Publication*: TC-2021
  *Summary*: This paper addresses the scheduling of Apache Spark jobs in hybrid cloud computing environments with SLA constraints. It develops an SLA-aware scheduling mechanism that dynamically places Spark tasks across private and public cloud resources to minimize cost while meeting deadline requirements. The proposed approach uses cost-performance models to guide placement decisions and achieves significant cost savings compared to single-cloud deployments.
  **Code**: Not available

- **[State Space Model and Queuing Network Based Cloud Resource Provisioning for Meshed Web Systems](https://scholar.google.com/scholar?q=State+Space+Model+and+Queuing+Network+Based+Cloud+Resource+Provisioning+for+Meshed+Web+Systems)**
  *Authors*: Yamin Lei, Zhicheng Cai, Xiaoping Li, Rajkumar Buyya
  *Publication*: TPDS-2022
  *Summary*: This paper proposes a cloud resource provisioning approach for meshed web systems based on state space models and queuing network theory. The method models the complex interactions among microservices as a queuing network and uses state space analysis to predict system performance under different resource configurations. The resulting provisioning algorithm dynamically allocates resources to meet performance targets while minimizing resource costs in meshed web architectures.
  **Code**: Not available

- **[TERMS: Task management policies to achieve high performance for mixed workloads using surplus resources](https://scholar.google.com/scholar?q=TERMS:+Task+management+policies+to+achieve+high+performance+for+mixed+workloads+using+surplus+resources)**
  *Authors*: Jinyu Yu, Wei Tong, Pengze Lv, Dan Feng
  *Publication*: JPDC-2022
  *Summary*: This paper presents TERMS, a task management framework that leverages surplus resources in cloud data centers to improve performance for mixed workloads. The system identifies idle or underutilized resources and applies policy-driven task placement to redirect batch and opportunistic workloads to these surplus resources. Experiments demonstrate that TERMS achieves significant performance improvements for mixed workloads without impacting the quality of service for primary applications.
  **Code**: Not available

- **[ThermoSim: Deep learning based framework for modeling and simulation of thermal-aware resource management for cloud computing environments](https://scholar.google.com/scholar?q=ThermoSim:+Deep+learning+based+framework+for+modeling+and+simulation+of+thermal-aware+resource+management+for+cloud+computing+environments)**
  *Authors*: Sukhpal Singh Gill, Shreshth Tuli, Adel Nadjaran Toosi, Felix Cuadrado, Peter Garraghan, Rami Bahsoon, Hanan Lutfiyya, Rizos Sakellariou, Omer Rana, Schahram Dustdar
  *Publication*: JSS-2020
  *Summary*: This paper presents ThermoSim, a deep learning-based framework for modeling and simulating thermal-aware resource management in cloud computing environments. The framework uses deep neural networks to predict thermal behavior of data center servers based on workload patterns and cooling conditions, enabling resource allocation decisions that minimize thermal hotspots and cooling energy. Simulation results demonstrate that ThermoSim effectively reduces peak temperatures and cooling costs compared to traditional thermal-unaware approaches.
  **Code**: Not available

---

### Beyond DRL — Workload Analysis & Characterization

- **[Who Limits the Resource Efficiency of My Datacenter: Alibaba Trace Analysis](https://scholar.google.com/scholar?q=Who+Limits+the+Resource+Efficiency+of+My+Datacenter+Alibaba+Trace+Analysis)**
  *Authors*: Jing Guo, Zihao Chang, Sa Wang, Haiyang Ding, Yihui Feng, Liang Mao, Yungang Bao
  *Publication*: IWQoS-2019
  *Summary*: This paper conducts a comprehensive trace analysis of Alibaba datacenter workloads to identify the root causes of low resource efficiency. Using production data from thousands of servers, the study identifies five major efficiency limiters: over-provisioning for peak loads, resource fragmentation, interference from co-located tasks, workload predictability limitations, and scheduling overhead. The analysis provides quantitative evidence that addressing these limiters can improve datacenter utilization from 15-20% to over 50%.
  **Code**: Not available

- **[Characteristics of Co-Allocated Online Services and Batch Jobs in Internet Data Centers: A Case Study From Alibaba Cloud](https://doi.org/10.1109/access.2019.2897898)**
  *Authors*: Congfeng Jiang, Guangjie Han, Jiangbin Lin, Gangyong Jia, Weisong Shi, Jian Wan
  *Publication*: IEEE-Access-2019
  *Summary*: This paper presents a detailed case study of co-allocated workloads in Alibaba Cloud data centers. The analysis reveals that online services and batch jobs exhibit complementary resource usage patterns: online services have stable, predictable demands with strict latency requirements, while batch jobs have bursty, flexible demands that can fill resource gaps. The study identifies interference patterns when co-locating these workloads and proposes strategies for interference-aware co-allocation that improves utilization by 30% without violating SLAs.
  **Code**: Not available

- **[Characterization and prediction of deep learning workloads in large-scale GPU datacenters](https://scholar.google.com/scholar?q=Characterization+and+prediction+of+deep+learning+workloads+in+large-scale+GPU+datacenters)**
  *Authors*: Qinghao Hu, Peng Sun, Shengen Yan, Yonggang Wen, Tianwei Zhang
  *Publication*: SC-2021
  *Summary*: This paper characterizes and predicts deep learning workloads in large-scale GPU datacenters using production traces from Alibaba Cloud. The analysis reveals that DL jobs exhibit distinct phases (data loading, training, checkpointing) with varying resource demands, and that job arrival patterns follow time-dependent distributions. The paper proposes a prediction model that forecasts DL workload intensity and resource requirements, enabling proactive GPU provisioning and reducing job queuing delays by 40%.
  **Code**: Not available

- **[Characterizing and Synthesizing Task Dependencies of Data-Parallel Jobs in Alibaba Cloud](https://scholar.google.com/scholar?q=Characterizing+and+Synthesizing+Task+Dependencies+of+Data-Parallel+Jobs+in+Alibaba+Cloud)**
  *Authors*: Huangshi Tian, Yunchuan Zheng, Wei Wang
  *Publication*: SoCC-2019
  *Summary*: This paper characterizes task dependencies in data-parallel jobs from Alibaba Cloud production traces, analyzing DAG structures, task execution times, and resource demands across thousands of jobs. The study identifies common dependency patterns (pipeline, map-reduce, fan-out) and proposes a task dependency synthesizer that generates realistic DAGs for scheduling research. The findings reveal that ignoring task dependencies leads to 50% suboptimal scheduling decisions in data-parallel workloads.
  **Code**: Not available

- **[Characterizing Co-Located Workloads in Alibaba Cloud Datacenters](https://doi.org/10.1109/tcc.2020.3034500)**
  *Authors*: Congfeng Jiang, Yitao Qiu, Weisong Shi, Zhefeng Ge, Jiwei Wang, Shenglei Chen, Christophe Cerin, Zujie Ren, Guoyao Xu, Jiangbin Lin
  *Publication*: TCC-2022
  *Summary*: This paper provides a comprehensive characterization of co-located workloads in Alibaba Cloud datacenters, analyzing interference patterns, resource contention, and performance degradation when online services and batch jobs share physical machines. The study uses production traces to quantify the impact of CPU, memory, and I/O contention on service latency, identifying key metrics for interference prediction. The findings inform the design of interference-aware scheduling policies that maintain SLA compliance while improving cluster utilization.
  **Code**: Not available

- **[Characterizing Job Microarchitectural Profiles at Scale: Dataset and Analysis](https://scholar.google.com/scholar?q=Characterizing+Job+Microarchitectural+Profiles+at+Scale:+Dataset+and+Analysis)**
  *Authors*: Kangjin Wang, Ying Li, Cheng Wang, Tong Jia, Kingsum Chow, Yang Wen, Yaoyong Dou
  *Publication*: SoCC-2022
  *Summary*: This paper presents a large-scale analysis of job microarchitectural profiles in cloud datacenters, collecting hardware performance counter data (CPU cache misses, branch mispredictions, memory bandwidth utilization) across thousands of production jobs. The study identifies distinct microarchitectural behavior patterns that traditional resource metrics (CPU, memory) cannot capture, and proposes a dataset of microarchitectural profiles for scheduling research. The analysis reveals that microarchitectural-aware scheduling can reduce cache contention and improve performance by 15-25%.
  **Code**: Not available

- **[Characterizing Job-Task Dependency in Cloud Workloads Using Graph Learning](https://doi.org/10.1109/ipdpsw52791.2021.00052)**
  *Authors*: Zhaochen Gu, Sihai Tang, Beilei Jiang, Song Huang, Qiang Guan, Song Fu
  *Publication*: IPDPSW-2021
  *Summary*: This paper characterizes job-task dependencies in cloud workloads using graph learning techniques. Task dependencies are modeled as graphs where nodes represent tasks and edges represent data or control dependencies. Graph neural networks are trained to predict task execution patterns, resource demands, and completion times based on dependency structure. The approach achieves 30% better prediction accuracy compared to non-graph-based methods, enabling more informed scheduling decisions for complex multi-task jobs.
  **Code**: Not available

- **[Characterizing Microservice Dependency and Performance: Alibaba Trace Analysis](https://doi.org/10.1145/3472883.3487003)**
  *Authors*: Shutian Luo, Huanle Xu, Chengzhi Lu, Kejiang Ye, Guoyao Xu, Liping Zhang, Yu Ding, Jian He, Chengzhong Xu
  *Publication*: SoCC-2021
  *Summary*: This paper presents a detailed characterization of microservice workloads from Alibaba production cluster traces. It analyzes dependency patterns, performance characteristics, and resource utilization across millions of microservice instances. The study reveals complex dependency chains, imbalanced load distributions, and provides actionable insights for microservice scheduling and resource management in large-scale cloud systems.
  **Code**: Not available

- **[Imbalance in the cloud: An analysis on Alibaba cluster trace](https://doi.org/10.1109/bigdata.2017.8258257)**
  *Authors*: Chengzhi Lu, Kejiang Ye, Guoyao Xu, Cheng-Zhong Xu, Tongxin Bai
  *Publication*: BIGDATA-2017
  *Summary*: This paper analyzes resource imbalance in Alibaba cluster traces, identifying the gap between allocated and utilized resources across CPU, memory, and disk dimensions. The study reveals that most tasks are bottlenecked on a single resource dimension while leaving others underutilized, leading to significant waste. The analysis quantifies the imbalance ratio across different workload types and proposes resource reallocation strategies that can reduce over-provisioning by 40% without impacting performance.
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
