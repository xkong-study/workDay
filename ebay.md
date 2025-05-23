# eBay Cloud SRE 岗位 HR 初轮面试问题与准备建议

---

<img width="744" alt="Screenshot 2025-05-19 at 19 47 20" src="https://github.com/user-attachments/assets/277df7aa-e0e2-4502-95b5-b4c4bf12be0d" />



## 一、常见 HR 面试问题（技术岗位）

### 1. 请您简单介绍一下自己。
Hi, I’m Xiangrui Kong, based in Dublin with a Master’s in Computer Science from Trinity College and about 3 years of experience in backend and infrastructure engineering.

At Velocity Global, I worked on AWS Lambda and DynamoDB to support a contractor CMS. In one incident, contract status became inconsistent due to a silent Lambda failure. I traced it via DynamoDB streams and CloudWatch, then wrote a Python script to scan, patch, and restore state transitions—cutting recovery time and preventing similar issues with added alerts.

At Energy Elephant, I built Python-based data pipelines for energy reports. I used Redis to schedule batch jobs and added S3 upload validation with retries and logging. I also maintained GitLab CI/CD and improved visibility through metrics and log alerts.

I love using code to improve system reliability and reduce operational pain.

### 2. 你为什么选择这个职位或来到 eBay 应聘？ 
What draws me to eBay is how it powers real economic opportunity for millions globally. Personally, I’ve used eBay for tech collectibles, and I’m fascinated by how its platform handles high-traffic, long-tail search, and seller tools.     

I’m excited by the challenge of supporting such large-scale, latency-sensitive systems. The Cloud SRE role offers the chance to work on critical systems that directly impact buyer and seller experience.          

My experience with AWS, Kubernetes, and CI/CD maps well to this role. I’ve enjoyed tackling similar problems—like autoscaling, failover design, and observability—and I look forward to doing that at global scale.      

I also appreciate eBay’s engineering culture, especially its support for open-source contribution and its focus on reliability and automation. That’s the kind of environment where I know I’ll learn and grow fast.        

### 3. 你的职业规划是什么？未来三到五年想实现什么目标？
- **回答思路/准备建议**：
  - 提出技术成长目标，例如成为资深 SRE 或平台架构师；
  - 强调持续学习新技术；
  - 可结合 TCD 项目经历说明快速学习能力。
- **面试意图**：
  - 了解职业目标是否清晰、是否具备成长意愿。

### 6. 为什么离开上一份工作？
- **回答思路/准备建议**：
  - 说明 Velocity Global 因组织结构调整导致团队关闭；
  - 强调自己寻求新成长机会；
  - 表达对过往工作的感激。
- **面试意图**：
  - 判断职业稳定性和离职原因合理性。


### 8. 你的薪资期望是多少？
- **回答思路/准备建议**：
  - 提前了解市场行情；
  - 给出范围，如“60k–75k EUR/年”；
  - 强调发展空间和岗位契合度也同样重要。
- **面试意图**：
  - 确认预算匹配性、谈判合理性。

### 10. 你还有什么想了解我们的地方吗？
- **回答思路/准备建议**：
  - 准备几个问题，比如：
    - 团队的工作流程？
    - 技术栈有哪些发展方向？
    - 公司对员工成长的支持机制？
- **面试意图**：
  - 观察主动性和对岗位的深度兴趣。

---

## 二、针对 eBay Cloud SRE 岗位及简历的预测问题

### 1. 什么是 SRE？你对这个岗位的理解？
- **回答思路/准备建议**：
  - 说明 SRE 是通过编程手段提升系统稳定性与运维效率；
  - 提到服务等级目标（SLO）和错误预算；
  - SRE 兼具开发与运维责任，常使用 Go/Python 做自动化；
  - 举例自己参与过日志监控、系统设计的经验。
- **面试意图**：
  - 验证候选人是否了解 SRE 核心理念和实践方式。

### 2. 你在 AWS/Azure/GCP 等云平台上有哪些实践经验？
- **回答思路/准备建议**：
  - 结合简历介绍具体服务如 S3、Lambda、DynamoDB、CloudFormation；
  - 强调部署自动化、数据处理、权限控制等细节；
  - 补充理解如弹性伸缩、安全性设计等。
- **面试意图**：
  - 评估对云平台的实际操作熟练度和理解深度。

### 3. 请介绍一下你使用 Kubernetes 的经验。
- **回答思路/准备建议**：
  - 举例 TCD 毕业项目中如何部署前后端服务；
  - 使用的对象（Pods, Services, Deployments）；
  - 说明如何调试和配置容器。
- **面试意图**：
  - 验证是否能适应 cloud-native 环境。

### 4. 你有使用 CI/CD 工具的经验吗？
- **回答思路/准备建议**：
  - 举出使用 GitLab CI/CD、Jenkins 的例子；
  - 涉及自动构建、测试、部署流程；
  - 强调代码质量控制如单元测试（Jest/QUnit）。
- **面试意图**：
  - 确认是否熟悉自动化流程和 DevOps 实践。

### 5. 你的技术栈包括 Go、Python、TypeScript 等，你最擅长哪一种？
- **回答思路/准备建议**：
  - 明确主要语言，如 Python 用于后端，Go 用于服务开发；
  - 强调语言迁移能力，如从 TS/React 到 Go；
  - 表现出对语言本质的理解和适应能力。
- **面试意图**：
  - 判断语言深度和适应新技术的速度。

### 6. 请描述一次你在项目中应用微服务架构的经历。
- **回答思路/准备建议**：
  - 举例 Energy Elephant 的数据处理服务或毕业项目；
  - 拆分服务、异步处理、跨服务通信等；
  - 谈及挑战如数据一致性、部署复杂度等。
- **面试意图**：
  - 评估系统架构理解与真实项目经验。

### 7. 你在项目中如何保证系统稳定性？有没有使用过监控或告警工具？
- **回答思路/准备建议**：
  - 举例使用 CloudWatch、Prometheus 或日志工具；
  - 设置指标监控和自动报警；
  - 强调测试覆盖、异常处理流程。
- **面试意图**：
  - 判断是否具备可靠性工程的基本素养。

### 8. 请谈谈你的硕士论文项目。
- **回答思路/准备建议**：
  - 简介项目目标、技术栈；
  - 说明自己负责的部分，如 Kubernetes 配置、API 设计；
  - 结合云部署和前后端集成讲述。
- **面试意图**：
  - 判断候选人的独立项目能力和技术综合实力。

### 9. 你怎么看 eBay 这样的大型平台的技术挑战？
- **回答思路/准备建议**：
  - 提出电商平台的高并发、低延迟、稳定性等挑战；
  - 分享自己对这些问题的理解和应对思路；
  - 表达乐于解决复杂问题的意愿。
- **面试意图**：
  - 看是否愿意投身技术挑战多的企业环境。

### 10. 你如何与来自不同文化背景的人协作？
- **回答思路/准备建议**：
  - 举例在 TCD 或公司中与国际同事合作的经历；
  - 强调倾听、适应、协作工具的使用；
  - 表现对多元文化的尊重和开放性。
- **面试意图**：
  - 验证是否能融入 eBay 的国际化团队。

---

> **建议：**  
> 最好在面试前用英文将这些回答结构整理一遍，确保讲述时流畅、自然；如果需要，我可以帮你把中文回答翻译成面试用英文版本。

---

