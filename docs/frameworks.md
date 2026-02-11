# Introduction
## Governance

This is the “Constitution” for your AI project. It outlines how your organization should approach risk, ethics, and legal issues.

- [NIST AI Risk Management Framework](#nists-ai-risk-management-framework-ai-rmf): The most important, universal foundation. A good place to start to understand the whole process.
- [AI Controls Matrix (AICM)](#ai-controls-matrix-aicm): A very detailed checklist when you need to meet ISO standards.

## Strategy and Technical Security
A practical approach to securing systems against attacks and failures.

- [Google SAIF](#googles-secure-ai-framework-saif): A strategy from a giant – how to build secure systems “by design.”
- [SAIL Framework](#sail-framework): Focuses on ensuring security throughout the model's life cycle.
- [CAI Framework](#cai-cyber-ai-framework): A specialized tool if you work with robots or autonomous systems.

## Risk and Attack Knowledge Bases
Encyclopedias of problems. You look here to know what can go wrong.

- [MIT AI Risk Repository](#mit-ai-risk-repository): A huge list of risks (e.g., biases, technical errors).
- [IBM AI Risk Atlas](#ibm-ai-risk-atlas): Taxonomy of risks – helps you “name” the problem you are facing.
- [MITRE ATLAS](#mitre-atlas): Knowledge base on how hackers attack AI (tactics and techniques).

# Frameworks

## NIST’s AI Risk Management Framework (AI RMF)

Source: [https://www.nist.gov/itl/ai-risk-management-framework](https://www.nist.gov/itl/ai-risk-management-framework)

A voluntary, high-level framework to help organizations systematically identify, assess, and manage risks in AI systems across their lifecycle. It emphasizes governance, transparency, accountability, and trustworthiness.

✅ Pros:

- Provides comprehensive risk management guidance across all AI lifecycle phases.
- Aligns well with global standards like ISO and EU AI Act, aiding multinational compliance.
- Encourages transparency and accountability, fostering trust and stakeholder confidence.
- Flexible and adaptable for varied sectors and AI maturity levels.

❌ Cons:

- Voluntary and non-certifiable - organizations aren’t compelled to adopt it.
- High-level guidance lacks detailed operational steps (“what” vs. “how”).
- Resource and expertise requirements can be burdensome, especially for small teams.
- Requires tailoring to specific contexts; one-size-fits-all use can feel bureaucratic.

## AI Controls Matrix (AICM)

Link: [https://cloudsecurityalliance.org/artifacts/ai-controls-matrix](https://cloudsecurityalliance.org/artifacts/ai-controls-matrix)

A detailed control objectives framework defining 243 AI security and governance controls across 18 domains, mapping to standards like ISO 42001, ISO 27001, and NIST AI RMF to support secure and responsible AI deployments.

✅ Pros:

- Vendor-agnostic, comprehensive set of controls tailored for AI risk and security.
- Mapped to multiple international standards enabling alignment and audit readiness.
- Helps operationalize governance through concrete control objectives.

❌ Cons:

- Large and complex - may be overwhelming without tooling or advanced expertise.
- Primarily focused on cloud environments - may need adaptation for on-premise/edge use.
- Maturity varies across domains and guidance - some controls may lack deep AI-specific examples. 

## Google’s Secure AI Framework (SAIF)

Source: [https://safety.google/intl/en_in/safety/saif/](https://safety.google/intl/en_in/safety/saif/)

A strategic security framework addressing AI risks such as model compromise, data poisoning, and privacy issues by integrating security principles into AI design, development, and deployment stages.

✅ Pros:

- Security-oriented focus tailored to real AI/ML risks like data poisoning and tampering.
- Expands AI governance beyond compliance to cover technical vulnerabilities.
- Helps unify security with product risk management and privacy principles.

❌ Cons:

- Not widely standardized or certifiable outside Google’s ecosystem. (inferred)
- High-level — more of a conceptual risk map than a full controls framework.

## MIT AI Risk Repository

Source: [https://airisk.mit.edu](https://airisk.mit.edu)

A curated repository of documented AI risks, failure modes, and mitigation patterns to support research and risk assessment practices. (General resource for AI risk knowledge.)

✅ Pros:

- Collective risk insights and documented real-world failure cases.
- Useful for research and comparative risk studies.

❌ Cons:

- Does not prescribe a formal governance or control framework.
- Not designed as a compliance standard.

## IBM AI Risk Atlas

Source: [https://ibm.github.io/ai-atlas-nexus/](https://ibm.github.io/ai-atlas-nexus/)

A structured taxonomy and knowledge base of AI risks, helping organizations identify, classify, and plan mitigations throughout the AI lifecycle.

✅ Pros:

- Rich taxonomy supports systematic risk identification.
- Practical for enterprise risk assessments.

❌ Cons:

- Not by itself a governance framework with controls.
- May require integration with other standards (ISO, NIST) for full compliance use.

## MITRE ATLAS

Source: [https://atlas.mitre.org/matrices/ATLAS](https://atlas.mitre.org/matrices/ATLAS)

An adversarial knowledge base cataloguing real-world tactics, techniques, and procedures used to attack AI systems, designed to support red-teaming, threat modeling, and defense testing.

✅ Pros:

- Provides concrete adversary techniques for practical testing.
- Useful for security teams building proactive defenses.

❌ Cons:

- Not a governance or risk management framework.
- Focused on adversarial threats, not organizational compliance.

## OWASP Top 10 for LLM Applications

Source: [https://owasp.org/www-project-top-10-for-large-language-model-applications/](https://owasp.org/www-project-top-10-for-large-language-model-applications/)

A community-driven list of the most prevalent security vulnerabilities in LLM applications (e.g., prompt injection, sensitive information disclosure) with guidance for mitigation.

✅ Pros:

- Highly practical and developer-friendly focus on concrete vulnerabilities.
- Widely referenced by security practitioners.

❌ Cons:

- Narrow in scope — does not provide holistic governance or lifecycle risk management.
- Must be paired with broader frameworks (e.g., NIST) to manage enterprise AI risk.

## SAIL Framework

Source: [https://www.pillar.security/sail](https://www.pillar.security/sail)

A security-assurance framework addressing lifecycle security controls and governance for AI deployments.

✅ Pros:

- Emphasizes lifecycle security and assurance practices.

❌ Cons:

- Less established/standardized compared with NIST or CSA frameworks.
- Implementation guidance may be less mature.

## CAI (Cyber-AI) Framework

Source: [https://github.com/aliasrobotics/cai](https://github.com/aliasrobotics/cai)

A cybersecurity-oriented framework focused on AI threats, threats vectors, and mitigations—especially for robotics and autonomous systems.

✅ Pros:

- Practical focus on real AI threat scenarios.

❌ Cons:

- Niche focus; not a complete governance or compliance structure.
