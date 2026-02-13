# **PhD Research Proposal — Final Draft (Master Version)**
### *Human-Centric Multi-Cloud Governance in Government PaaS/IaaS: Harmonising BSI, ISO/IEC, NIST, GDPR, and NCSC Standards into Actionable Policy-as-Code Guardrails*

**Candidate:** Elias Lenz (MSc InfoSec, ISC2 CC, SSCP)  
**Programme:** PhD in Cybersecurity  
**Institution:** University of Plymouth — Faculty of Science and Engineering  
**Submission:** Full Proposal (Master Draft)

---

# **1. Abstract**
Government organisations in Germany and the United Kingdom increasingly rely on public-cloud PaaS/IaaS to deliver critical services. Simultaneously, they must comply with stringent, heterogeneous, and sometimes overlapping cybersecurity and privacy frameworks including BSI C5/IT‑Grundschutz, ISO/IEC 27001/27017/27018, NIST SP 800‑53 and CSF 2.0, GDPR, and UK NCSC Cloud Security Principles. These frameworks differ in scope, structure, terminology, and control philosophies, creating significant challenges when translating written requirements into technical cloud configurations.

Empirical studies show that misconfigurations, unclear governance responsibilities, and reactive audit-driven compliance remain primary causes of cloud insecurity across public-sector environments. This research therefore proposes a **human‑centric, standards‑harmonised Policy‑as‑Code (PaC) framework** that translates regulatory controls into enforceable guardrails across AWS, Azure, and Google Cloud Platform. Using a design‑science and mixed‑methods approach—combining standards analysis, practitioner interviews, guardrail modelling, prototype implementation, and empirical evaluation—the study aims to produce: (1) a cross‑standard policy‑intent model; (2) a multi‑cloud PaC reference architecture; (3) a prototype guardrail engine; and (4) evidence‑based guidance for government cloud governance.

---

# **2. Introduction & Background**
Public‑sector digital transformation depends increasingly on cloud platforms, yet such platforms introduce new risks and governance complexity. Germany’s regulatory environment emphasises standardised security baselines, sovereignty, and data residency, while the UK ecosystem emphasises risk-based guidance and auditable controls. Both environments must adhere to GDPR and international standards such as ISO/IEC 27001.

Despite this strong regulatory foundation, **cloud misconfigurations remain the leading cause of security breaches**. Extensive research on Kubernetes manifests, IAM configurations, and cloud resource policies consistently highlights systemic weaknesses. Government agencies often operate in multi-cloud environments with siloed governance structures, limited automation, and inconsistent control implementations.

Policy‑as‑Code has emerged as a means of bridging the governance gap, enabling standards-compliant guardrails to be implemented programmatically. Yet its application remains fragmented, with no unified methodology for standards harmonisation or multi-cloud deployment.

---

# **3. Problem Statement & Research Gap**
Government organisations must comply with numerous security frameworks but lack a unified, technically sound method for translating these frameworks into actionable multi‑cloud guardrails. Current approaches rely on manual interpretation, partial standards crosswalks, inconsistent cloud-native governance tools, and retrospective audits.

## **Research Gap Summary**
There is **no existing framework** that:
- harmonises BSI, ISO/IEC, NIST, GDPR, and NCSC requirements into a structured, machine-readable policy‑intent model;
- maps these policy intents into cross‑cloud guardrails across AWS, Azure, and GCP;
- embeds human‑centric governance and decision pathways; and
- demonstrates empirical feasibility in government‑like use cases.

This research addresses this gap by developing and validating a **standards‑grounded, human‑centric PaC governance framework** for the public sector.

---

# **4. Research Aim, Objectives, and Questions**
## **Aim**
To design and validate a standards‑harmonised, human‑centric Policy‑as‑Code framework for the automated enforcement of security and privacy guardrails across multi‑cloud government PaaS/IaaS environments.

## **Objectives**
1. Analyse BSI, ISO/IEC, NIST, GDPR, and NCSC frameworks to derive harmonised policy intents.  
2. Develop a structured, machine‑readable policy‑intent meta‑model.  
3. Map harmonised policy intents to AWS, Azure, and GCP guardrails.  
4. Implement a Policy‑as‑Code prototype to enforce selected guardrails.  
5. Evaluate the framework’s technical effectiveness and organisational usability.

## **Research Questions**
### **Primary Research Question (RQ1)**
**How can BSI, ISO/IEC, NIST, GDPR, and NCSC standards be harmonised into actionable guardrails across AWS, Azure, and GCP for government PaaS/IaaS environments?**

### **Sub‑Questions**
**RQ1.1:** Which cloud-native controls most effectively implement harmonised guardrails?  
**RQ1.2:** How can Policy‑as‑Code automate the deployment, validation, and maintenance of guardrails?  
**RQ1.3:** What governance structures and human‑centric processes support sustainable multi‑cloud guardrail management?  
**RQ1.4:** How can compliance evidence be automatically generated to meet audit and regulatory expectations?

---

# **5. Literature Review (Summary)**
### **5.1 Standards and Regulatory Foundations**
ISO/IEC 27001/27017/27018, NIST SP 800‑53 and CSF 2.0, BSI C5/IT‑Grundschutz, NCSC Cloud Security Principles, and GDPR collectively define mandatory expectations for confidentiality, integrity, availability, privacy, and accountability in cloud environments.

### **5.2 Cloud Misconfigurations and Governance Weaknesses**
Empirical studies reveal widespread configuration drift, excessive permissions, insecure defaults, and inconsistent enforcement in cloud and Kubernetes environments.

### **5.3 Policy‑as‑Code and Cloud Governance Tooling**
AWS SCPs, Azure Policy, and GCP Org Policy offer powerful but heterogeneous control mechanisms. Open-source tools like OPA, Kyverno, and Cloud Custodian enable flexible enforcement but lack direct linkage to regulatory standards.

### **5.4 Public-Sector Sovereignty and Compliance Constraints**
Government workloads must account for jurisdiction, privacy, residency, auditability, and assurance—requirements not fully supported by existing PaC implementations.

### **5.5 Literature Gaps**
- No harmonised model linking standards to actionable PaC guardrails.  
- Insufficient empirical research on PaC in government.  
- Lack of automated, cross‑cloud evidence‑generation mechanisms.

---

# **6. Methodology**
A **design science research (DSR)** methodology is applied across four phases:

## **Phase 1 — Requirements & Standards Analysis**
- Document analysis of BSI, NIST, ISO/IEC, NCSC, GDPR.  
- Semi‑structured interviews with government architects and auditors.

## **Phase 2 — Framework & Meta‑Model Design**
- Development of a harmonised policy‑intent model.  
- Mapping of intents to AWS/Azure/GCP controls.

## **Phase 3 — Prototype Development**
- PaC engine implementation using OPA/Rego, Kyverno, Azure Policy, AWS SCPs, and GCP Org Constraints.
- Application of guardrails to realistic public-sector cloud scenarios.

## **Phase 4 — Evaluation & Validation**
- Technical evaluation: coverage, misconfiguration detection, false positives/negatives.  
- Qualitative evaluation: expert walkthroughs, think‑aloud studies, thematic analysis.

---

# **7. Expected Contributions**
## **Theoretical Contributions**
- First harmonised, cross‑jurisdiction policy‑intent meta‑model for government cloud security.  
- New insights into human factors in Policy‑as‑Code governance.

## **Practical Contributions**
- A reusable multi‑cloud PaC reference architecture.  
- Prototype enforcement engine and guardrail templates.  
- Automated evidence‑generation patterns.

## **Societal Contributions**
- Reduced cloud misconfiguration risk across government.  
- Improved transparency, accountability, and audit readiness.  
- Strengthened digital public-service resilience.

---

# **8. Ethical Considerations**
- GDPR-compliant participant data handling.  
- Secure storage and pseudonymisation of interview data.  
- No real citizen data used in prototype evaluation.  
- Ethics approval obtained prior to empirical activities.

---

# **9. Timeline (Narrative Gantt Summary)**
- **Year 1:** Orientation, literature review, standards analysis, ethics approval.  
- **Year 2:** Interview design, early data collection, meta‑model construction.  
- **Year 3:** Full data collection, framework consolidation.  
- **Year 4:** Prototype development and initial evaluation.  
- **Year 5:** Extended evaluation, refinement, and drafting core thesis chapters.  
-**


---

# **10. References**

*The following reference list has been formatted in Harvard (Cite Them Right) style based on the sources provided so far. This is a working list and can be expanded once the full Zotero library is finalised.*

Amazon Web Services (2023) *AWS Well-Architected Framework*. Available at: https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html.

Amazon Web Services (2024) *Service Control Policies (SCPs) — Best Practices*. Available at: https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html.

Amazon Web Services (2023) *Control Tower Guardrails — Mandatory vs Elective*. Available at: https://docs.aws.amazon.com/controltower/latest/userguide/guardrails.html.

Amazon Web Services (2024) *IAM Access Analyzer — Policy Validation*. Available at: https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-policy-validation.html.

Amazon Web Services (2023) *Security Hub — Foundational Security Best Practices*. Available at: https://aws.amazon.com/security-hub/.

AWS, Google and Microsoft (2023) *Multi-Cloud Zero Trust Patterns*. Whitepaper.

BMI – Bundesministerium des Innern (2024) *German Federal Cloud Strategy*. Berlin: BMI.

BSI (2023) *Cloud Computing Compliance Controls Catalogue (C5)*. Bonn: Bundesamt für Sicherheit in der Informationstechnik.

BSI (2023) *IT-Grundschutz-Kompendium*. Bonn.

BSI (2023) *Digitalstrategie 2030*. Berlin.

BSI (2024) *German Cloud Security Guidance*. Available at: https://www.bsi.bund.de/EN/.

Cabinet Office (2023) *Government Security Policy Framework (SPF)*. Available at: https://www.gov.uk/government/publications/government-security.

Center for Internet Security (2024) *CIS Benchmarks for AWS, Azure, GCP*. Available at: https://www.cisecurity.org/benchmark/.

Cloud Custodian (2025) *Rules Engine Documentation*. Available at: https://cloudcustodian.io/.

Cloud Security Alliance (2024) *Cloud Controls Matrix v4*. Available at: https://cloudsecurityalliance.org/research/cloud-controls-matrix.

CNCF (2023) *Secure Software Supply Chain Guidance*. Available at: https://www.cncf.io/.

CNCF (2024) *OPA Gatekeeper Policy Library*. Available at: https://github.com/open-policy-agent/gatekeeper-library.

CSIRO (2024) *AI for Cloud Security Automation*. Canberra: CSIRO.

Deloitte (2024) *Government Cloud Adoption Insights*. London.

DSIT (2024) *Cyber Security Breaches Survey 2024*. London: GOV.UK.

Dubois, S. (2025) ‘Cloud Security Best Practices: AWS, Azure & GCP’. Available at: https://atlas-advisory.eu.

EDPB (2022) *Guidelines 05/2021 on Data Breach Notification*. Available at: https://edpb.europa.eu.

ENISA (2023) *Guidelines for Securing the Internet of Things (IoT)*. Available at: https://www.enisa.europa.eu.

ENISA (2024) *Threat Landscape 2024*. Athens: ENISA.

ENISA (2024) *Sovereign Cloud Security Requirements*. Athens.

European Commission (2023) *EUCS — EU Cloud Services Cybersecurity Certification Scheme (Draft)*. Brussels.

Gartner (2023) *Cloud Misconfiguration Root Causes*. Stamford, CT.

Google Cloud (2023) *Assured Workloads — Compliance Controls*. Available at: https://cloud.google.com/assured-workloads.

Google Cloud (2023) *Organisation Policy Service*. Available at: https://cloud.google.com/resource-manager/docs/organization-policy.

Google Cloud (2024) *Policy Intelligence*. Available at: https://cloud.google.com/policy-intelligence.

Google Cloud (2024) *VPC Service Controls & Hierarchical Firewall*. Available at: https://cloud.google.com/vpc-service-controls.

HashiCorp (2024) *Terraform Enterprise Governance Features*. Available at: https://developer.hashicorp.com/terraform/enterprise/.

IBM (2023) *Zero Trust Blueprint for Government*. Available at: https://www.ibm.com.

IBM (2024) *Cloud Framework for Financial Services*. Available at: https://www.ibm.com/cloud/.

ICO (2023) *Anonymisation, Pseudonymisation & PETs Guidance*. Available at: https://ico.org.uk.

ISO (2025) *ISO/IEC 27018:2025*. Geneva: ISO.

ISO/IEC (2022) *27001:2022 – Information Security Management Systems*. Geneva.

ISO/IEC (2022) *27002:2022 – Security Controls*. Geneva.

ISO/IEC (2015) *27017:2015 – Cloud Security Controls*. Geneva.

ISO/IEC (2019) *27701:2019 – Privacy Information Management*. Geneva.

Kyverno (2025) *Policy Documentation*. Available at: https://kyverno.io/docs/policies/.

Lunardi, T. et al. (2022) ‘ARCADE: Adversarially Regularized Convolutional Autoencoder’, *arXiv*. Available at: https://arxiv.org.

McKinsey (2023) *Modernising Government Cloud Security*. New York.

Microsoft (2023) *Azure Blueprints — Regulatory Compliance*. Available at: https://learn.microsoft.com.

Microsoft (2024) *Defender for Cloud — Regulatory Compliance*. Available at: https://learn.microsoft.com.

Microsoft (2024) *Entra Permissions Management*. Available at: https://learn.microsoft.com.

Microsoft Learn (2025) *Policy as Code with GitHub & Bicep*. Available at: https://learn.microsoft.com.

Minna, F. et al. (2025) ‘Analysing and mitigating Helm chart misconfigurations’, *Empirical Software Engineering*, 30.

MITRE (2024) *ATT&CK Cloud Matrix Updates*. Available at: https://attack.mitre.org.

NCSC (2023) *Cloud Security Principles*. London.

Nirmata (2024) *Policy-as-Code for Financial Institutions*. Available at: https://nirmata.com.

NIST (2022) *SP 800-53 Rev. 5*. Gaithersburg, MD.

NIST (2023) *SP 800-207 Rev.1 – Zero Trust Architecture*. Gaithersburg, MD.

NIST (2024) *Cybersecurity Framework 2.0*. Gaithersburg, MD.

NIST (2023) *SP 800-204C – Microservices Security*. Gaithersburg, MD.

NIST (2021) *SP 800-218 – Secure Software Development Framework*. Gaithersburg, MD.

OPA (2025) *Policy Language (Rego)*. Available at: https://openpolicyagent.org.

OWASP (2023) *Kubernetes Top 10*. Available at: https://owasp.org.

PCI SSC (2022) *PCI DSS v4.0 — Summary of Changes*. Available at: https://pcisecuritystandards.org.

Rahman, A. & Akond, R. (2022) ‘Security Misconfigurations in Kubernetes Manifests’, *ACM TOSEM*, 31.

Red Hat (2025) *Automate Security Practices with Kyverno*. Available at: https://redhat.com.

SANS Institute (2023) *Cloud Security Observability*. Bethesda, MD.

UK Government Digital Service (2023) *Technology Code of Practice*. Available at: https://www.gov.uk.

USENIX (2024) *Productionizing Policy Engines at Scale*. Available at: https://www.usenix.org.

VMware (2024) *Tanzu Mission Control — Policy Management*. Available at: https://docs.vmware.com.

