# Kaisura AI-Cloud Security Framework (KAICSF)

An enterprise-grade security framework for organizations deploying AI systems in 
cloud environments. Developed as a graduate capstone at Northeastern University.

## What it addresses

Most existing frameworks (NIST, ISO 27001, SOC 2) were designed before AI workloads 
became mainstream. KAICSF extends these standards to cover AI-specific threats like prompt 
injection, model drift, data poisoning in cloud-hosted environments.

## Framework structure

### Governance layer
- 30+ KPIs mapped to MTTD, MTTR, model drift rate, data leakage incidents
- Roles and responsibilities for AI security ownership
- Audit trail requirements for AI model decisions

### Risk layer
- Threat taxonomy: prompt injection, model poisoning, training data leakage, 
  adversarial inputs, supply chain compromise
- Risk scoring methodology aligned with NIST AI RMF
- Vendor risk assessment checklist for third-party AI tools

### Compliance layer
- Control mappings to NIST AI RMF, ISO 27001, OWASP LLM Top 10, HIPAA
- Gap analysis template for organizations adopting AI
- Evidence collection guide for auditors

### Implementation layer
- Zero Trust integration: identity verification for AI API access, 
  least-privilege for model endpoints
- DevSecOps pipeline: security gates at model training, validation, and deployment
- Incident response runbook for AI-specific security events

## Validated use case

The framework was validated through a HIPAA-compliant healthcare scenario:
- Threat model: patient data exposure via LLM prompt injection
- Controls applied: input sanitization, output filtering, audit logging, 
  access controls on model endpoints
- Outcome: mapped 14 AI-specific threats to mitigating controls with KPI tracking

## Standards alignment

| Standard | Coverage area |
|---|---|
| NIST AI RMF | Govern, Map, Measure, Manage functions |
| ISO 27001 | Annex A controls extended for AI assets |
| OWASP LLM Top 10 | All 10 categories addressed |
| HIPAA | PHI protection in AI-assisted workflows |
| Zero Trust | Identity, device, and workload verification |

## Related writing

- [Securing AI in the Cloud](https://medium.com/@samriddhi5/securing-ai-in-the-cloud-236348de1b7c) — Medium article overview
