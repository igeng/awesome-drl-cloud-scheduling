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
- [Open‑Source Projects](#open-source-projects)  
- [Datasets](#datasets)  
- [Tools & Frameworks](#tools--frameworks)  
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

- **[Batch Jobs Load Balancing Scheduling in Cloud Computing Using Distributional Reinforcement Learning](https://ieeexplore.ieee.org/abstract/document/10323098)**  
  *Authors*: Tiangang Li, Shi Ying, Yishi Zhao, Jianga Shang  
  *Summary*: This work tackles dynamic cluster load balancing for batch job scheduling in cloud computing. It highlights limitations in standard DRL approaches (like DQN), which ignore the full value distribution and struggle with time-varying jobs/resources. The authors propose a Distributional Reinforcement Learning (DRL) solution using quantile regression to model the cumulative return's value distribution, capturing environmental stochasticity. They formulate scheduling as a multi-objective optimization problem, develop a custom training environment, and introduce a novel DRL-based scheduling algorithm. Evaluated on real Alibaba cluster traces (v2018 & v2020), the algorithm outperforms baselines in load balancing, instance creation success rate, and average task completion time, demonstrating strong scalability.

- **[DRL‑Cloud: DRL‑based Resource Provisioning and Task Scheduling for Cloud Service Providers](https://ieeexplore.ieee.org/abstract/document/8297294)**  
  *Authors*: Mingxi Cheng, Ji Li, Shahin Nazarian  
  *Summary*: This paper addresses energy cost minimization for large-scale Cloud Service Providers (CSPs). It identifies limitations in prior Resource Provisioning (RP) and Task Scheduling (TS) approaches, including scalability issues and neglect of crucial task dependencies. The authors propose DRL-Cloud, a novel Deep Reinforcement Learning (DRL) system featuring a two-stage RP-TS processor based on deep Q-learning. This system autonomously learns optimal long-term decisions by adapting to dynamic factors like user request patterns and electricity prices. Utilizing standard DRL techniques (target network, experience replay, exploration-exploitation), DRL-Cloud achieves significantly improved energy cost efficiency, low task reject rate, low runtime, and fast convergence. Evaluations demonstrate dramatic improvements: up to 320% higher energy cost efficiency compared to state-of-the-art methods while maintaining lower reject rates, and up to 144% runtime reduction versus a fast round-robin baseline in a large-scale scenario (5,000 servers, 200,000 tasks).

- *(Additional DRL-based resource scheduling papers can be listed here.)*

### Autoscaling

- **[FIRM: An Intelligent Fine-grained Resource Management Framework for SLO-Oriented Microservices](https://www.usenix.org/conference/osdi20/presentation/qiu)**  
  *Authors*: Haoran Qiu, Subho S. Banerjee, Saurabh Jha, Zbigniew T. Kalbarczyk, and Ravishankar K. Iyer, University of Illinois at Urbana-Champaign  
  *Summary*: User-facing latency-sensitive web services include numerous distributed, intercommunicating microservices that promise to simplify software development and operation. However, multiplexing of compute resources across microservices is still challenging in production because contention for shared resources can cause latency spikes that violate the service-level objectives (SLOs) of user requests. This paper presents FIRM, an intelligent fine-grained resource management framework for predictable sharing of resources across microservices to drive up overall utilization. FIRM leverages online telemetry data and machine-learning methods to adaptively (a) detect/localize microservices that cause SLO violations, (b) identify low-level resources in contention, and (c) take actions to mitigate SLO violations via dynamic reprovisioning. Experiments across four microservice benchmarks demonstrate that FIRM reduces SLO violations by up to 16x while reducing the overall requested CPU limit by up to 62%. Moreover, FIRM improves performance predictability by reducing tail latencies by up to 11x.

- **[AWARE: Automate Workload Autoscaling with Reinforcement Learning in Production Cloud Systems](https://www.usenix.org/conference/atc23/presentation/qiu-haoran)**  
  *Authors*: Haoran Qiu and Weichao Mao, University of Illinois at Urbana-Champaign; Chen Wang, Hubertus Franke, and Alaa Youssef, IBM Research; Zbigniew T. Kalbarczyk, Tamer Başar, and Ravishankar K. Iyer, University of Illinois at Urbana-Champaign  
  *Summary*: Workload autoscaling is widely used in public and private cloud systems to maintain stable service performance and save resources. However, it remains challenging to set the optimal resource limits and dynamically scale each workload at runtime. Reinforcement learning (RL) has recently been proposed and applied in various systems tasks, including resource management. In this paper, we first characterize the state-of-the-art RL approaches for workload autoscaling in a public cloud and point out that there is still a large gap in taking the RL advances to production systems. We then propose AWARE, an extensible framework for deploying and managing RL-based agents in production systems. AWARE leverages meta-learning and bootstrapping to (a) automatically and quickly adapt to different workloads, and (b) provide safe and robust RL exploration. AWARE provides a common OpenAI Gym-like RL interface to agent developers for easy integration with different systems tasks. We illustrate the use of AWARE in the case of workload autoscaling. Our experiments show that AWARE adapts a learned autoscaling policy to new workloads 5.5x faster than the existing transfer-learning-based approach and provides stable online policy-serving performance with less than 3.6% reward degradation. With bootstrapping, AWARE helps achieve 47.5% and 39.2% higher CPU and memory utilization while reducing SLO violations by a factor of 16.9x during policy training.

---

## Open‑Source Projects

*(List of open‑source DRL scheduling/autoscaling implementations go here.)*

---

## Datasets

*(Datasets for DRL training and evaluation — job traces, metrics logs, cloud simulators, etc.)*

---

## Tools & Frameworks

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
