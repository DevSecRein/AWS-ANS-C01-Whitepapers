### **Summary Table**

[AWS Certified Advanced Networking – Specialty (ANS-C01): Ultimate 2025 Study & Exam Prep Guide](https://www.youtube.com/watch?v=W_KPkGs0mj0) - A current (2025) breakdown of the ANS-C01 exam structure and specifically highlights which whitepapers and domains are carrying the most weight in the current exam version

|**Whitepaper / Topic**|**Networking Specialty**|**Solutions Architect Pro**|
|---|---|---|
|**Multi-VPC Architecture**|⭐⭐⭐⭐⭐|⭐⭐⭐⭐⭐|
|**VPC Connectivity Options**|⭐⭐⭐⭐⭐|⭐⭐⭐⭐⭐|
|**Hybrid (DX/VPN) Resiliency**|⭐⭐⭐⭐⭐|⭐⭐⭐⭐|
|**DNS / Route 53 Resolver**|⭐⭐⭐⭐⭐|⭐⭐⭐|
|**IPv6 Adoption**|⭐⭐⭐⭐|⭐|
|**Geneve / GWLB / Traffic Mirroring**|⭐⭐⭐⭐|⭐|

The papers that are also essential reading for the **AWS Certified Solutions Architect - Professional (SAP-C02)** are marked with a **\[SAP]** tag. The overlap between these two exams is significant, particularly in the domains of hybrid connectivity (Direct Connect/VPN) and multi-account strategy.

### **1. The "Holy Grail" Network Architecture Papers**

These are the foundational documents. If you only read three papers, make them these.

- **\[SAP] Building a Scalable and Secure Multi-VPC AWS Network Infrastructure**
    
    - **Why it's critical:** This is arguably the single most important whitepaper for both exams. It moves beyond simple VPC peering into Transit Gateway, Shared VPCs, and centralized egress/ingress patterns.
        
    - **Link:** [Building a Scalable and Secure Multi-VPC AWS Network Infrastructure](https://docs.aws.amazon.com/whitepapers/latest/building-scalable-secure-multi-vpc-network-infrastructure/welcome.html)

- **\[SAP] Amazon VPC Connectivity Options**
    
    - **Why it's critical:** A classic whitepaper that details every possible way to connect VPCs (Peering, Transit Gateway, PrivateLink, VPN). You must know the pros, cons, and bandwidth limits of each method by heart.
        
    - **Link:** [Amazon VPC Connectivity Options](https://docs.aws.amazon.com/whitepapers/latest/aws-vpc-connectivity-options/welcome.html)

- **\[SAP] AWS Well-Architected Framework - Networking Pillar**
    
    - **Why it's critical:** The Professional and Specialty exams focus heavily on _why_ you choose a solution (Cost vs. Performance vs. Reliability). This framework provides the "AWS thinking" required to answer scenario-based questions.
        
    - **Link:** [Networking Pillar - AWS Well-Architected Framework](https://www.google.com/search?q=https://docs.aws.amazon.com/wellarchitected/latest/networking-pillar/welcome.html)

---
### **2. Hybrid Connectivity (Direct Connect & VPN)**

This is the hardest section of the Networking Specialty and a major component of the SAP exam.

- **\[SAP] AWS Direct Connect User Guide (Selections)**
    
    - **Note:** While technically a "User Guide," the _Resiliency Recommendations_ and _Public/Private VIF_ sections are treated as whitepaper-level theory on the exam. Focus specifically on **Failover scenarios** (Active/Active, Active/Passive).
        
    - **Link:** [AWS Direct Connect Resiliency Recommendations](https://www.google.com/search?q=https://docs.aws.amazon.com/directconnect/latest/UserGuide/resiliency-recommendations.html)

- **Hybrid Connectivity using AWS Transit Gateway**
    
    - **Why it's critical:** Explains how to attach VPNs and Direct Connect Gateways to a Transit Gateway, a pattern that appears frequently in complex networking scenarios.
        
    - **Link:** [Hybrid Connectivity](https://docs.aws.amazon.com/whitepapers/latest/hybrid-connectivity/welcome.html)

---
### **3. Advanced Network Services & Security**

These are vital for the Networking Specialty but appear less frequently or in less depth on the SAP exam.

- **\[SAP] Practicing Safe DNS (Route 53)**
    
    - **Why it's critical:** DNS is a massive part of the Networking exam. You need to understand Split-horizon DNS, Route 53 Resolver (Inbound/Outbound endpoints), and how to resolve DNS across hybrid environments.
        
    - **Link:** [Hybrid Cloud DNS Options for AWS](https://www.google.com/search?q=https://docs.aws.amazon.com/whitepapers/latest/hybrid-cloud-dns-options-for-aws/welcome.html)

- **AWS Network Firewall Architecture**
    
    - **Why it's critical:** The ANS-C01 exam loves "traffic inspection" scenarios. You must understand how to route traffic through a firewall using Gateway Load Balancer endpoints (GWLB).
        
    - **Link:** [Deployment models for AWS Network Firewall](https://www.google.com/search?q=https://docs.aws.amazon.com/whitepapers/latest/deployment-models-for-aws-network-firewall/welcome.html)

- **IPv6 on AWS**
    
    - **Why it's critical:** The Networking Specialty requires deep IPv6 knowledge (Egress-Only Internet Gateways, Dual-stack VPCs). The SAP exam rarely goes this deep into IPv6.
        
    - **Link:** [IPv6 on AWS](https://d1.awsstatic.com/whitepapers/IPv6-on-AWS.pdf)

---
### **4. Diagram: Centralized Inspection**

The concept of "[Centralized Inspection](https://aws.amazon.com/blogs/networking-and-content-delivery/centralized-inspection-architecture-with-aws-gateway-load-balancer-and-aws-transit-gateway/)" using Transit Gateway is a top candidate for exam questions in both certifications.

---
