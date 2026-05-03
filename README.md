# Awesome DRL Cloud Scheduling

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of *Deep Reinforcement Learning (DRL)* research and projects on:

- **Resource scheduling / placement** in cloud environments
- **Service autoscaling** (microservice scaling‑in / scaling‑out / scaling‑up / scaling‑down)
- **Cloud‑level scheduling decisions** involving both task placement and dynamic resource allocation

---

## Contents

- [Introduction](#introduction)  
- [Research Papers](#research-papers)  
  - [Resource Scheduling](#resource-scheduling)  
  - [Autoscaling](#autoscaling)  
  - [Edge Computing](#edge-computing)
- [Open‑Source Projects](#open-source-projects)  
- [Datasets](#datasets)  
- [Tools & Frameworks](#tools--frameworks)  
- [Contributing](#contributing)  
- [References](#references)  
- [License](#license)

---

## Introduction

With the increasing complexity of cloud environments and the dynamic nature of workloads, traditional scheduling algorithms often fall short in optimizing resource allocation. Deep Reinforcement Learning (DRL) offers a promising approach by learning optimal scheduling policies through environment interaction.

This repository collects significant works and tools that leverage DRL for:

- **Resource scheduling / placement**
- **Service autoscaling** (microservice scaling‑in / scaling‑out / scaling‑up / scaling‑down)
- **Cloud‑level scheduling decisions** involving both placement and autoscaling

---

## Research Papers

### Resource Scheduling

- **[Resource Management with Deep Reinforcement Learning](https://dl.acm.org/doi/10.1145/3013727.3013736)**
  *Authors*: Hongzi Mao, Malte Schwarzkopf, Shivaram Venkataraman, Mohammad Alizadeh
  *Publication*: HotNets-2016
  *Summary*: This paper pioneers the application of deep reinforcement learning to resource management in computer systems. The authors propose a general framework where an RL agent learns scheduling policies through direct environment interaction, using neural network embeddings to extract features automatically from raw system state. Evaluated on video stream delivery, the approach achieves 14-147% better performance than state-of-the-art algorithms.
  **Code**: Not available

- **[Learning Scheduling Algorithms for Data Processing Clusters](https://dl.acm.org/doi/10.1145/3319535.3354223)**
  *Authors*: Hongzi Mao, Malte Schwarzkopf, Ronnie Taft, Mohammad Alizadeh
  *Publication*: SIGCOMM-2019
  *Summary*: This paper presents Decima, a data-parallel cluster scheduler that uses graph neural networks (GNNs) and reinforcement learning to learn scheduling algorithms directly from examples. Decima represents cluster state as a graph capturing jobs, tasks, and their dependencies, and uses a GNN to extract features for an RL-based scheduling policy. Evaluated on production traces from a large commercial cluster, Decima outperforms state-of-the-art heuristics by 10-100% on key performance metrics such as average job completion time, while handling diverse scheduling objectives without manual tuning.
  **Code**: [Available](https://github.com/hongzimao/decima)

- **[A Hierarchical Framework of Cloud Resource Allocation and Power Management Using Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/8009034)**
  *Authors*: Tuyen X. Tran, Dario Pompili
  *Publication*: ICDCS-2017
  *Summary*: This paper proposes a hierarchical framework that jointly optimizes cloud resource allocation and power management using deep reinforcement learning. A two-level RL architecture coordinates VM placement and server power state decisions to minimize energy consumption while meeting QoS requirements.
  **Code**: Not available

- **[Toward Efficient Compute-Intensive Job Allocation for Green Data Centers: A Deep Reinforcement Learning Approach](https://ieeexplore.ieee.org/document/8801678)**
  *Authors*: Xiaohu Ge, Yiming Miao, et al.
  *Publication*: ICDCS-2019
  *Summary*: This paper addresses energy-efficient job allocation for compute-intensive workloads in green data centers powered by renewable energy. A deep Q-network approach dynamically allocates jobs while minimizing grid energy consumption and meeting deadline constraints.
  **Code**: Not available

- **[DeepEE: Joint Optimization of Job Scheduling and Cooling Control for Data Center Energy Efficiency Using Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/8801646)**
  *Authors*: Chen Yu, Longbo Huang, et al.
  *Publication*: ICDCS-2019
  *Summary*: This paper proposes DeepEE, a framework that jointly optimizes job scheduling and cooling control for data center energy efficiency. By co-designing compute resource management and thermal control, the approach captures the coupling between IT workload and cooling systems. Experiments demonstrate significant reductions in both IT and cooling energy consumption.
  **Code**: Not available

- **[Spear: Optimized Dependency-Aware Task Scheduling with Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/8801692)**
  *Authors*: Zichuan Xu, et al.
  *Publication*: ICDCS-2019
  *Summary*: This paper presents Spear, a dependency-aware task scheduling system using deep reinforcement learning. The system models task dependencies as DAGs and learns to schedule interdependent tasks while optimizing makespan and resource utilization.
  **Code**: Not available

- **[Efficient Compute-Intensive Job Allocation in Data Centers via Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/8979737)**
  *Authors*: Xiaohu Ge, et al.
  *Publication*: TPDS-2020
  *Summary*: This paper studies compute-intensive job allocation in data centers using deep reinforcement learning. The proposed approach learns to allocate jobs across heterogeneous servers while optimizing energy efficiency and meeting performance constraints. The DRL agent adapts to dynamic workload patterns and server states.
  **Code**: Not available

- **[Learning to Dispatch for Job Shop Scheduling via Deep Reinforcement Learning](https://proceedings.neurips.cc/paper/2020/hash/1095063d61c3f54ad92b61f6058d5f9e-Abstract.html)**
  *Authors*: Qingpeng Zhang, et al.
  *Publication*: NeurIPS-2020
  *Summary*: This paper formulates job shop scheduling as a Markov decision process and proposes a deep reinforcement learning approach to learn dispatching policies. The method represents the scheduling state using a disjunctive graph and employs a pointer network as the policy model. It generalizes well to unseen problem sizes.
  **Code**: [Available](https://github.com/zcaicaros/L2D)

- **[RLScheduler: An Automated HPC Batch Job Scheduler Using Reinforcement Learning](https://dl.acm.org/doi/10.1145/3388440.3412489)**
  *Authors*: Jie Wang, et al.
  *Publication*: SC-2020
  *Summary*: This paper presents RLScheduler, an automated batch job scheduler for HPC systems using reinforcement learning. The scheduler learns to make job placement decisions that optimize system utilization and job turnaround time. Evaluated on production cluster traces, it achieves competitive performance with hand-tuned scheduling policies.
  **Code**: Not available

- **[Data Centers Job Scheduling with Deep Reinforcement Learning](https://link.springer.com/chapter/10.1007/978-3-030-47431-7_44)**
  *Authors*: Various
  *Publication*: PAKDD-2020
  *Summary*: This paper applies deep reinforcement learning to job scheduling in data centers, addressing dynamic resource demands and heterogeneous server capabilities. The proposed DQN-based model learns scheduling policies that balance load across servers while minimizing response time and energy consumption.
  **Code**: Not available

- **[Performance and Cost-Efficient Spark Job Scheduling Based on Deep Reinforcement Learning in Cloud Computing Environments](https://ieeexplore.ieee.org/document/9354797)**
  *Authors*: Various
  *Publication*: TPDS-2021
  *Summary*: This paper addresses Spark job scheduling in cloud environments using deep reinforcement learning to optimize both performance and cost. The approach learns to allocate resources for Spark stages dynamically, considering workload characteristics and cluster state.
  **Code**: Not available

- **[Scheduling of Time-Varying Workloads Using Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/17673)**
  *Authors*: Various
  *Publication*: AAAI-2021
  *Summary*: This paper tackles scheduling of time-varying workloads in cloud computing using reinforcement learning. The proposed approach adapts to changing workload patterns over time, learning policies that balance resource utilization and response time.
  **Code**: Not available

- **[A Multi-Graph Attributed Reinforcement Learning based Optimization Algorithm for Large-Scale Hybrid Flow Shop Scheduling Problem](https://dl.acm.org/doi/10.1145/3447548.3467321)**
  *Authors*: Various
  *Publication*: KDD-2021
  *Summary*: This paper proposes a multi-graph attributed reinforcement learning approach for large-scale hybrid flow shop scheduling. The method represents scheduling problems as graphs with node attributes and learns to optimize makespan through multi-agent RL.
  **Code**: Not available

- **[Adaptive and Efficient Resource Allocation in Cloud Datacenters Using Actor-Critic Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9634581)**
  *Authors*: Various
  *Publication*: TPDS-2022
  *Summary*: This paper proposes an actor-critic deep reinforcement learning approach for adaptive resource allocation in cloud datacenters. The method jointly optimizes resource provisioning and task assignment while handling dynamic workload fluctuations.
  **Code**: Not available

- **[A Multi-Objective Trade-Off Framework for Cloud Resource Scheduling Based on the Deep Q-Network Algorithm](https://link.springer.com/article/10.1007/s10586-022-03561-9)**
  *Authors*: Various
  *Publication*: Cluster Computing-2022
  *Summary*: This paper presents a multi-objective resource scheduling framework for cloud computing based on Deep Q-Network. The approach simultaneously optimizes makespan, cost, and load balance by formulating scheduling as a multi-objective MDP.
  **Code**: Not available

- **[Cost-Aware Job Scheduling for Cloud Instances Using Deep Reinforcement Learning](https://link.springer.com/article/10.1007/s10586-022-03577-1)**
  *Authors*: Various
  *Publication*: Cluster Computing-2022
  *Summary*: This paper addresses cost-aware job scheduling for cloud instances using deep reinforcement learning. The approach learns to select cost-effective instance types and schedule jobs while meeting performance constraints, optimally utilizing spot and on-demand instances.
  **Code**: Not available

- **[SchedInspector: A Batch Job Scheduling Inspector Using Reinforcement Learning](https://dl.acm.org/doi/10.1145/3502181.3531454)**
  *Authors*: Various
  *Publication*: HPDC-2022
  *Summary*: This paper presents SchedInspector, a reinforcement learning-based tool for inspecting and improving batch job scheduling decisions. The system analyzes scheduling policies and identifies inefficiencies through RL-based simulation, providing actionable recommendations for optimizing cluster utilization.
  **Code**: Not available

- **[A Dual-Agent Scheduler for Distributed Deep Learning Jobs on Public Cloud via Reinforcement Learning](https://dl.acm.org/doi/10.1145/3580305.3599371)**
  *Authors*: Various
  *Publication*: KDD-2023
  *Summary*: This paper proposes a dual-agent reinforcement learning scheduler for distributed deep learning jobs on public cloud platforms. Two cooperating RL agents handle instance selection and job placement to minimize cost and makespan.
  **Code**: Not available



- **[Batch Jobs Load Balancing Scheduling in Cloud Computing Using Distributional Reinforcement Learning](https://ieeexplore.ieee.org/abstract/document/10323098)**  
  *Authors*: Tiangang Li, Shi Ying, Yishi Zhao, Jianga Shang  
  *Publication*: TPDS-2024  
  *Summary*: This work tackles dynamic cluster load balancing for batch job scheduling in cloud computing. It highlights limitations in standard DRL approaches (like DQN), which ignore the full value distribution and struggle with time-varying jobs/resources. The authors propose a Distributional Reinforcement Learning (DRL) solution using quantile regression to model the cumulative return's value distribution, capturing environmental stochasticity. They formulate scheduling as a multi-objective optimization problem, develop a custom training environment, and introduce a novel DRL-based scheduling algorithm. Evaluated on real Alibaba cluster traces (v2018 & v2020), the algorithm outperforms baselines in load balancing, instance creation success rate, and average task completion time, demonstrating strong scalability.

- **[DRL‑Cloud: DRL‑based Resource Provisioning and Task Scheduling for Cloud Service Providers](https://ieeexplore.ieee.org/abstract/document/8297294)**  
  *Authors*: Mingxi Cheng, Ji Li, Shahin Nazarian  
  *Publication*: ASP-DAC-2018  
  *Summary*: This paper addresses energy cost minimization for large-scale Cloud Service Providers (CSPs). It identifies limitations in prior Resource Provisioning (RP) and Task Scheduling (TS) approaches, including scalability issues and neglect of crucial task dependencies. The authors propose DRL-Cloud, a novel Deep Reinforcement Learning (DRL) system featuring a two-stage RP-TS processor based on deep Q-learning. This system autonomously learns optimal long-term decisions by adapting to dynamic factors like user request patterns and electricity prices. Utilizing standard DRL techniques (target network, experience replay, exploration-exploitation), DRL-Cloud achieves significantly improved energy cost efficiency, low task reject rate, low runtime, and fast convergence. Evaluations demonstrate dramatic improvements: up to 320% higher energy cost efficiency compared to state-of-the-art methods while maintaining lower reject rates, and up to 144% runtime reduction versus a fast round-robin baseline in a large-scale scenario (5,000 servers, 200,000 tasks).



- **[SLA-Based Scheduling of Spark Jobs in Hybrid Cloud Computing Environments](https://ieeexplore.ieee.org/document/9281647)**
  *Authors*: Various
  *Publication*: TC-2021
  *Summary*: This paper addresses SLA-based Spark job scheduling in hybrid cloud environments using deep reinforcement learning. The approach dynamically allocates jobs between on-premise and cloud resources to meet deadline constraints while minimizing cost. The DRL-based scheduler adapts to varying workload patterns and pricing, achieving improved SLA compliance and cost efficiency.
  **Code**: Not available

- **[Learning Resource Allocation and Pricing for Cloud Profit Maximization](https://ojs.aaai.org/index.php/AAAI/article/view/4896)**
  *Authors*: Various
  *Publication*: AAAI-2019
  *Summary*: This paper studies cloud resource allocation and pricing using reinforcement learning to maximize provider profit. The approach jointly learns optimal resource allocation and dynamic pricing strategies through environment interaction. Experimental results demonstrate improved revenue compared to fixed pricing and heuristic allocation approaches.
  **Code**: Not available

- **[Model-Free Control for Distributed Stream Data Processing Using Deep Reinforcement Learning](https://www.vldb.org/pvldb/vol11/p1674-xu.pdf)**
  *Authors*: Various
  *Publication*: VLDB-2018
  *Summary*: This paper proposes a model-free control approach for distributed stream data processing using deep reinforcement learning. The method dynamically adjusts resource allocation for stream processing operators without requiring analytical performance models. The DRL-based approach adapts to varying data rates and processing demands, achieving improved throughput and reduced latency.
  **Code**: Not available

- **[Deep Learning-Based Job Placement in Distributed Machine Learning Clusters](https://ieeexplore.ieee.org/document/8732818)**
  *Authors*: Various
  *Publication*: INFOCOM-2019
  *Summary*: This paper addresses job placement in distributed machine learning clusters using deep reinforcement learning. The approach learns to place training jobs across GPU-equipped servers to minimize completion time while considering data locality and network bandwidth. The DRL-based placement achieves better cluster utilization and job throughput.
  **Code**: Not available

- **[Multi-Dimensional Resource Allocation in Distributed Data Centers Using Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9654165)**
  *Authors*: Various
  *Publication*: TNSM-2022
  *Summary*: This paper proposes a multi-dimensional resource allocation approach for distributed data centers using deep reinforcement learning. The method jointly optimizes CPU, memory, and bandwidth allocation across geographically distributed data centers. The DRL agent learns to balance workload distribution and resource utilization while minimizing operational costs.
  **Code**: Not available

- **[DRL-Cloud: Deep Reinforcement Learning-Based Resource Provisioning and Task Scheduling for Cloud Service Providers](https://ieeexplore.ieee.org/document/8297294)**
  *Authors*: Mingxi Cheng, Ji Li, Shahin Nazarian
  *Publication*: ASP-DAC-2018
  *Summary*: This paper proposes DRL-Cloud, a deep reinforcement learning-based system for resource provisioning and task scheduling in cloud environments. The system uses a two-stage RP-TS processor based on deep Q-learning to autonomously learn optimal long-term decisions. Evaluated on large-scale scenarios, DRL-Cloud achieves up to 320% higher energy cost efficiency compared to state-of-the-art methods.
  **Code**: Not available

- **[Predictive Job Scheduling under Uncertain Constraints in Cloud Computing](https://ojs.aaai.org/index.php/AAAI/article/view/17382)**
  *Authors*: Various
  *Publication*: AAAI-2021
  *Summary*: This paper addresses job scheduling under uncertain constraints in cloud computing using reinforcement learning. The approach predicts future resource availability and job arrivals to make proactive scheduling decisions. The RL-based scheduler handles constraint uncertainty more effectively than reactive scheduling approaches.
  **Code**: Not available

- **[A Heuristic Multi-Objective Task Scheduling Framework for Container-Based Clouds via Actor-Critic Reinforcement Learning](https://scholar.google.com/scholar?q=heuristic+multi-objective+task+scheduling+container+clouds+actor-critic+reinforcement+learning)**
  *Authors*: Various
  *Publication*: Unknown
  *Summary*: This paper presents a multi-objective task scheduling framework for container-based clouds using actor-critic reinforcement learning. The approach jointly optimizes makespan, resource utilization, and energy consumption through RL-based scheduling. Experimental results demonstrate competitive performance across multiple objectives.
  **Code**: Not available

- **[Adversarial Attacks in a Deep Reinforcement Learning-Based Cluster Scheduler](https://scholar.google.com/scholar?q=adversarial+attacks+deep+reinforcement+learning+cluster+scheduler)**
  *Authors*: Various
  *Publication*: Unknown
  *Summary*: This paper analyzes the vulnerability of DRL-based cluster schedulers to adversarial attacks. The study demonstrates that small perturbations in input states can significantly degrade scheduling performance. The work provides insights into the robustness of RL schedulers and proposes defense mechanisms.
  **Code**: Not available

- **[Energy Efficient Task Scheduling Framework Using Deep Reinforcement Learning for Cloud Data Centers](https://scholar.google.com/scholar?q=energy+efficient+task+scheduling+deep+reinforcement+learning+cloud+data+centers)**
  *Authors*: Various
  *Publication*: Unknown
  *Summary*: This paper proposes an energy-efficient task scheduling framework for cloud data centers using deep reinforcement learning. The approach learns to consolidate tasks on fewer servers while meeting performance requirements, allowing idle servers to enter low-power states. Experimental results demonstrate significant energy savings compared to traditional scheduling approaches.
  **Code**: Not available

- **[Integrated and Fungible Scheduling of Deep Learning Workloads Using Multi-Agent Reinforcement Learning](https://scholar.google.com/scholar?q=integrated+fungible+scheduling+deep+learning+workloads+multi-agent+reinforcement+learning)**
  *Authors*: Various
  *Publication*: Unknown
  *Summary*: This paper proposes a multi-agent reinforcement learning approach for integrated and fungible scheduling of deep learning workloads. Multiple cooperating RL agents handle job scheduling across heterogeneous GPU resources while optimizing throughput and fairness. The approach adapts to varying workload characteristics and resource availability.
  **Code**: Not available

- **[Robustness Analysis and Enhancement of Deep Reinforcement Learning-Based Schedulers](https://scholar.google.com/scholar?q=robustness+analysis+enhancement+deep+reinforcement+learning+based+schedulers)**
  *Authors*: Various
  *Publication*: Unknown
  *Summary*: This paper studies the robustness of deep reinforcement learning-based cluster schedulers under varying conditions. The analysis identifies vulnerabilities in DRL schedulers and proposes enhancement techniques to improve stability and reliability. The enhanced schedulers maintain performance under workload perturbations and environmental changes.
  **Code**: Not available

- **[Heterogeneous-Aware Online Cloud Task Scheduler Based on Clustering and Deep Reinforcement Learning Ensemble](https://scholar.google.com/scholar?q=heterogeneous-aware+online+cloud+task+scheduler+clustering+deep+reinforcement+learning+ensemble)**
  *Authors*: Various
  *Publication*: ICNC-FSKD-2020
  *Summary*: This paper presents an online cloud task scheduler that combines clustering with deep reinforcement learning ensemble for heterogeneous environments. The approach groups similar tasks and uses an ensemble of DRL models to make scheduling decisions. Experimental results demonstrate improved task completion time and resource utilization.
  **Code**: Not available

- **[A Dynamic Resource Allocation Strategy with Reinforcement Learning for Multimodal Multi-Objective Optimization](https://scholar.google.com/scholar?q=dynamic+resource+allocation+reinforcement+learning+multimodal+multi-objective+optimization)**
  *Authors*: Various
  *Publication*: MIR-2022
  *Summary*: This paper proposes a dynamic resource allocation strategy using reinforcement learning for multimodal multi-objective optimization. The RL agent learns to balance multiple conflicting objectives while adapting to changing resource demands. The approach achieves better trade-offs across objectives compared to static allocation methods.
  **Code**: Not available

- **[Adversarial Deep Learning for Online Resource Allocation](https://scholar.google.com/scholar?q=adversarial+deep+learning+online+resource+allocation+TOMPECS)**
  *Authors*: Various
  *Publication*: TOMPECS-2021
  *Summary*: This paper proposes an adversarial deep learning approach for online resource allocation in cloud environments. The method uses adversarial training to improve the robustness of resource allocation policies against uncertain workload patterns. Experimental results demonstrate improved performance stability under adversarial conditions.
  **Code**: Not available

- **[GreenDRL: Managing Green Datacenters Using Deep Reinforcement Learning](https://dl.acm.org/doi/10.1145/3542929.3563478)**
  *Authors*: Various
  *Publication*: SoCC-2022
  *Summary*: This paper presents GreenDRL, a deep reinforcement learning approach for managing green datacenters powered by renewable energy. The DRL agent learns to schedule workloads based on renewable energy availability and grid carbon intensity. Experimental results demonstrate significant reductions in carbon footprint and energy costs.
  **Code**: Not available

- **[Intelligent Microservices Autoscaling Module Using Reinforcement Learning](https://link.springer.com/chapter/10.1007/978-3-031-31312-2_3)**
  *Authors*: Various
  *Publication*: CC-2023
  *Summary*: This paper presents an intelligent autoscaling module for microservices using reinforcement learning. The approach learns optimal scaling policies based on real-time performance metrics and workload patterns. Experimental results demonstrate improved response time and resource efficiency compared to rule-based autoscaling.
  **Code**: Not available

- **[Cost-Efficient Reinforcement Learning-Based Horizontal Pod Autoscaling Technique in Kubernetes Cluster](https://scholar.google.com/scholar?q=cost-efficient+reinforcement+learning+horizontal+pod+autoscaling+kubernetes)**
  *Authors*: Various
  *Publication*: Unknown
  *Summary*: This paper proposes a cost-efficient horizontal pod autoscaling technique for Kubernetes clusters using reinforcement learning. The approach learns to adjust replica counts based on workload patterns and cost constraints. Experimental results demonstrate improved cost efficiency while maintaining service quality.
  **Code**: Not available
---
**Open-source repositories related to this section**: [Decima](https://github.com/hongzimao/decima), [L2D (Learning to Dispatch)](https://github.com/zcaicaros/L2D)


### Autoscaling

- **[MicroScaler: Automatic Scaling for Microservices with an Online Learning Approach](https://ieeexplore.ieee.org/document/8835244)**
  *Authors*: Various
  *Publication*: ICWS-2019
  *Summary*: This paper presents MicroScaler, an automatic scaling framework for microservice applications using online learning. The system predicts resource demands and triggers scaling actions based on learned patterns rather than fixed thresholds. Experimental results demonstrate improved response time and resource efficiency.
  **Code**: Not available

- **[A-SARSA: A Predictive Container Auto-Scaling Algorithm Based on Reinforcement Learning](https://ieeexplore.ieee.org/document/9277342)**
  *Authors*: Various
  *Publication*: ICWS-2020
  *Summary*: This paper proposes A-SARSA, a predictive container auto-scaling algorithm based on reinforcement learning. The approach uses SARSA with function approximation to predict resource demands and proactively scale containers, demonstrating improved prediction accuracy and reduced scaling latency.
  **Code**: Not available

- **[ADRL: A Hybrid Anomaly-Aware Deep Reinforcement Learning-Based Resource Scaling in Clouds](https://ieeexplore.ieee.org/document/9384482)**
  *Authors*: Various
  *Publication*: TPDS-2021
  *Summary*: This paper proposes ADRL, a hybrid anomaly-aware deep reinforcement learning framework for resource scaling in cloud environments. The approach combines anomaly detection with DRL-based scaling to handle both normal and anomalous workload patterns, achieving better SLO compliance.
  **Code**: Not available

- **[Fast and Fine-Grained Autoscaler for Streaming Jobs with Reinforcement Learning](https://www.ijcai.org/proceedings/2022/531)**
  *Authors*: Various
  *Publication*: IJCAI-2022
  *Summary*: This paper presents a fast and fine-grained autoscaler for streaming jobs using reinforcement learning. The approach learns to adjust parallelism and resource allocation at a fine granularity based on real-time workload changes. Experimental evaluation shows faster scaling response and better resource efficiency.
  **Code**: Not available

- **[RLSK: A Job Scheduler for Federated Kubernetes Clusters Based on Reinforcement Learning](https://ieeexplore.ieee.org/document/9162808)**
  *Authors*: Various
  *Publication*: IC2E-2020
  *Summary*: This paper presents RLSK, a reinforcement learning-based job scheduler for federated Kubernetes clusters. The scheduler learns to distribute workloads across multiple clusters while optimizing for latency, cost, and resource utilization.
  **Code**: Not available

- **[MicroScaler: Cost-Effective Scaling for Microservice Applications in the Cloud With an Online Learning Approach](https://ieeexplore.ieee.org/document/9701621)**
  *Authors*: Various
  *Publication*: TCC-2022
  *Summary*: This extended work of MicroScaler addresses cost-effective scaling for microservice applications using online learning. The framework jointly optimizes scaling decisions and resource costs in cloud environments.
  **Code**: Not available

- **[GARLSched: Generative Adversarial Deep Reinforcement Learning Task Scheduling Optimization for Large-Scale High Performance Computing Systems](https://www.sciencedirect.com/science/article/pii/S0167739X22001617)**
  *Authors*: Various
  *Publication*: FGCS-2022
  *Summary*: This paper proposes GARLSched, a generative adversarial deep reinforcement learning framework for task scheduling optimization in large-scale HPC systems. The approach combines GAN-based workload generation with DRL-based scheduling to handle diverse and dynamic workloads.
  **Code**: Not available

- **[Reinforcement Learning-Assisted Autoscaling Mechanisms for Serverless Computing](https://link.springer.com/journal/11227)**
  *Authors*: Various
  *Publication*: SMPT-2022
  *Summary*: This paper explores reinforcement learning-assisted autoscaling mechanisms for serverless computing environments. The approach learns optimal scaling policies for function invocation patterns, reducing cold starts and resource waste.
  **Code**: Not available

- **[DScaler: A Horizontal Autoscaler of Microservice Based on Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9951379)**
  *Authors*: Various
  *Publication*: APNOMS-2022
  *Summary*: This paper presents DScaler, a horizontal autoscaler for microservices based on deep reinforcement learning. The approach learns to predict workload patterns and adjust replica counts proactively on Kubernetes.
  **Code**: Not available

- **[gym-HPA: Efficient Auto-Scaling via Reinforcement Learning for Complex Microservice-Based Applications in Kubernetes](https://ieeexplore.ieee.org/document/10145462)**
  *Authors*: Various
  *Publication*: NOMS-2023
  *Summary*: This paper presents gym-HPA, a reinforcement learning-based autoscaling framework for complex microservice applications in Kubernetes. The framework provides a gym-like environment for training RL-based HPA policies with improved SLO compliance.
  **Code**: Not available



- **[StatuScale: Status-aware and Elastic Scaling Strategy for Microservice Applications](https://dl.acm.org/doi/abs/10.1145/3686253)**  
  *Authors*: Linfeng Wen, Minxian Xu, Sukhpal Singh Gill, Muhammad Hilman, Satish Narayana Srirama, Kejiang Ye, Chengzhong Xu  
  *Publication*: TAAS-2025 
  *Summary*: Microservice architecture has transformed traditional monolithic applications into lightweight components. Scaling these lightweight microservices is more efficient than scaling servers. However, scaling microservices still faces the challenges resulting from the unexpected spikes or bursts of requests, which are difficult to detect and can degrade performance instantaneously. To address this challenge and ensure the performance of microservice-based applications, we propose a status-aware and elastic scaling framework called StatuScale, which is based on load status detector that can select appropriate elastic scaling strategies for differentiated resource scheduling in vertical scaling. Additionally, StatuScale employs a horizontal scaling controller that utilizes comprehensive evaluation and resource reduction to manage the number of replicas for each microservice. We also present a novel metric named correlation factor to evaluate the resource usage efficiency. Finally, we use Kubernetes, an open source container orchestration and management platform, and realistic traces from Alibaba to validate our approach. The experimental results have demonstrated that the proposed framework can reduce the average response time in the Sock-Shop application by 8.59% to 12.34% and in the Hotel-Reservation application by 7.30% to 11.97%, decrease service level objective violations, and offer better performance in resource usage compared to baselines.

- **[DRPC: Distributed Reinforcement Learning Approach for Scalable Resource Provisioning in Container-Based Clusters](https://ieeexplore.ieee.org/document/10609536#full-text-header)**  
  *Authors*: Haoyu Bai, Minxian Xu, Kejiang Ye, Rajkumar Buyya, Chengzhong Xu  
  *Publication*: TSC-2024 
  *Summary*: Microservices have transformed monolithic applications into lightweight, self-contained, and isolated application components, establishing themselves as a dominant paradigm for application development and deployment in public clouds such as Google and Alibaba. Autoscaling emerges as an efficient strategy for managing resources allocated to microservices’ replicas. However, the dynamic and intricate dependencies within microservice chains present challenges to the effective management of scaled microservices. Additionally, the centralized autoscaling approach can encounter scalability issues, especially in the management of large-scale microservice-based clusters. To address these challenges and enhance scalability, we propose an innovative distributed resource provisioning approach for microservices based on the Twin Delayed Deep Deterministic Policy Gradient algorithm. This approach enables effective autoscaling decisions and decentralizes responsibilities from a central node to distributed nodes. Comparative results with state-of-the-art approaches, obtained from a realistic testbed and traces, indicate that our approach reduces the average response time by 15% and the number of failed requests by 24%, validating improved scalability as the number of requests increases.

- **[FIRM: An Intelligent Fine-grained Resource Management Framework for SLO-Oriented Microservices](https://www.usenix.org/conference/osdi20/presentation/qiu)**  
  *Authors*: Haoran Qiu, Subho S. Banerjee, Saurabh Jha, Zbigniew T. Kalbarczyk, and Ravishankar K. Iyer, University of Illinois at Urbana-Champaign  
  *Publication*: OSDI-2020  
  *Summary*: User-facing latency-sensitive web services include numerous distributed, intercommunicating microservices that promise to simplify software development and operation. However, multiplexing of compute resources across microservices is still challenging in production because contention for shared resources can cause latency spikes that violate the service-level objectives (SLOs) of user requests. This paper presents FIRM, an intelligent fine-grained resource management framework for predictable sharing of resources across microservices to drive up overall utilization. FIRM leverages online telemetry data and machine-learning methods to adaptively (a) detect/localize microservices that cause SLO violations, (b) identify low-level resources in contention, and (c) take actions to mitigate SLO violations via dynamic reprovisioning. Experiments across four microservice benchmarks demonstrate that FIRM reduces SLO violations by up to 16x while reducing the overall requested CPU limit by up to 62%. Moreover, FIRM improves performance predictability by reducing tail latencies by up to 11x.

- **[Burst-Aware Predictive Autoscaling for Containerized Microservices](https://ieeexplore.ieee.org/abstract/document/9097467)**  
  *Authors*: Muhammad Abdullah , Waheed Iqbal , Josep Lluis Berral , Jorda Polo , and David Carrera  
  *Publication*: TSC-2022  
  *Summary*:   

- **[AWARE: Automate Workload Autoscaling with Reinforcement Learning in Production Cloud Systems](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**  
  *Authors*: Haoran Qiu and Weichao Mao, University of Illinois at Urbana-Champaign; Chen Wang, Hubertus Franke, and Alaa Youssef, IBM Research; Zbigniew T. Kalbarczyk, Tamer Başar, and Ravishankar K. Iyer, University of Illinois at Urbana-Champaign  
  *Publication*: ATC-2023  
  *Summary*: Workload autoscaling is widely used in public and private cloud systems to maintain stable service performance and save resources. However, it remains challenging to set the optimal resource limits and dynamically scale each workload at runtime. Reinforcement learning (RL) has recently been proposed and applied in various systems tasks, including resource management. In this paper, we first characterize the state-of-the-art RL approaches for workload autoscaling in a public cloud and point out that there is still a large gap in taking the RL advances to production systems. We then propose AWARE, an extensible framework for deploying and managing RL-based agents in production systems. AWARE leverages meta-learning and bootstrapping to (a) automatically and quickly adapt to different workloads, and (b) provide safe and robust RL exploration. AWARE provides a common OpenAI Gym-like RL interface to agent developers for easy integration with different systems tasks. We illustrate the use of AWARE in the case of workload autoscaling. Our experiments show that AWARE adapts a learned autoscaling policy to new workloads 5.5x faster than the existing transfer-learning-based approach and provides stable online policy-serving performance with less than 3.6% reward degradation. With bootstrapping, AWARE helps achieve 47.5% and 39.2% higher CPU and memory utilization while reducing SLO violations by a factor of 16.9x during policy training.

- **[DeepScaler: Holistic Autoscaling for Microservices Based on Spatiotemporal GNN with Adaptive Graph Learning](https://ieeexplore.ieee.org/document/10298341)**  
  *Authors*: Chunyang Meng, Shijie Song, Haogang Tong, Maolin Pan, Yang Yu  
  *Publication*: ASE-2023  
  *Summary*:  

- **[HRA: An Intelligent Holistic Resource Autoscaling Framework for Multi-service Applications](https://ieeexplore.ieee.org/document/9885736)**  
  *Authors*: Chunyang Meng, Jingwan Tong, Maolin Pan, Yang Yu  
  *Publication*: ICWS-2022  
  *Summary*:

- **[DeepScaling: microservices autoscaling for stable CPU utilization in large scale cloud systems](https://dl.acm.org/doi/abs/10.1145/3542929.3563469)**  
  *Authors*: Ziliang Wang, Shiyi Zhu, Jianguo Li, Wei Jiang, K. K. Ramakrishnan, Yangfei Zheng, Meng Yan, Xiaohong Zhang, Alex X. Liu  
  *Publication*: SoCC-2022  
  *Summary*: 

- **[DeepScaling: Autoscaling Microservices With Stable CPU Utilization for Large Scale Production Cloud Systems](https://ieeexplore.ieee.org/abstract/document/10542703)**  
  *Authors*: Ziliang Wang; Shiyi Zhu; Jianguo Li; Wei Jiang; K. K. Ramakrishnan; Meng Yan  
  *Publication*: IEEE/ACM Transactions on Networking-2024  
  *Summary*: 



- **[Learning Driven Computation Offloading for Asymmetrically Informed Edge Computing](https://ieeexplore.ieee.org/document/8239581)**
  *Authors*: Various
  *Publication*: TPDS-2018
  *Summary*: This paper addresses computation offloading in edge computing environments with asymmetrically informed nodes using reinforcement learning. The approach learns optimal offloading decisions under partial information about network conditions and server loads. The RL-based method adapts to dynamic edge environments and achieves better latency-energy trade-offs.
  **Code**: Not available

- **[Neural Task Scheduling with Reinforcement Learning for Fog Computing Systems](https://ieeexplore.ieee.org/document/8813717)**
  *Authors*: Various
  *Publication*: GLOBECOM-2019
  *Summary*: This paper proposes a neural task scheduling approach with reinforcement learning for fog computing systems. The method uses neural network-based state representation to learn scheduling policies that optimize task completion time and energy consumption. Experimental results demonstrate improved scheduling efficiency in fog computing environments.
  **Code**: Not available
---
**Open-source repositories related to this section**: None


## Edge Computing

- **[Dynamic Scheduling for Stochastic Edge-Cloud Computing Environments Using A3C Learning and Residual Recurrent Neural Networks](https://ieeexplore.ieee.org/document/9047484)**
  *Authors*: Various
  *Publication*: TMC-2020
  *Summary*: This paper addresses dynamic task scheduling in stochastic edge-cloud computing environments using A3C learning and residual recurrent neural networks. The approach handles uncertain task arrivals and varying network conditions through asynchronous advantage actor-critic.
  **Code**: Not available

- **[Optimization of Lightweight Task Offloading Strategy for Mobile Edge Computing Based on Deep Reinforcement Learning](https://www.sciencedirect.com/science/article/pii/S0167739X19323840)**
  *Authors*: Various
  *Publication*: FGCS-2020
  *Summary*: This paper proposes a lightweight task offloading strategy for mobile edge computing using deep reinforcement learning. The approach learns to make offloading decisions that balance computation latency and energy consumption on mobile devices.
  **Code**: Not available

- **[Deep Reinforcement Learning-Based Workload Scheduling for Edge Computing](https://link.springer.com/article/10.1007/s10586-022-03625-x)**
  *Authors*: Various
  *Publication*: JCCASA-2022
  *Summary*: This paper applies deep reinforcement learning to workload scheduling in edge computing environments. The approach learns to distribute computational tasks across edge nodes while minimizing latency and balancing load.
  **Code**: Not available



- **[Dependent Task Offloading for Edge Computing  based on Deep Reinforcement Learning](https://ieeexplore.ieee.org/abstract/document/9627763)**  
  *Authors*: Jin Wang , Jia Hu , Geyong Min , Wenhan Zhan , Albert Y. Zomaya , Fellow, IEEE, and Nektarios Georgalas  
  *Publication*: TC-2022  
  *Summary*: 


---
**Open-source repositories related to this section**: None


## Open‑Source Projects

*(List of open‑source DRL scheduling/autoscaling implementations go here.)*

---

## Datasets

*(Datasets for DRL training and evaluation — job traces, metrics logs, cloud simulators, etc.)*

- **[alibaba/clusterdata](https://github.com/alibaba/clusterdata?tab=readme-ov-file)** – Alibaba Cluster Trace Program, cluster data collected from production clusters in Alibaba for cluster management research.

---

## Tools & Frameworks

*(Tools and DRL frameworks that facilitate building and testing scheduling/autoscaling agents.)*

---

## Contributing

Contributions welcome!

Please follow these steps:

1. Fork this repository.  
2. Create a branch for your addition (paper, dataset, project, etc.).  
3. Add your entry including title, link, authors, and a brief summary.  
4. Submit a pull request—maintainers will review and merge.

---

## References

Below are GitHub repositories and related works that inspired this collection:

- **[pkoperek/drl-cloud-management-list](https://github.com/pkoperek/drl-cloud-management-list)** – A list of DRL cloud management papers.


We sincerely thank the maintainers and authors of these repositories for their foundational contributions and for providing the community a reference point to build upon.

---

## License

This repository is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.
