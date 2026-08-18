# EU AI Act Approval Pack

## Executive Summary

Four client AI use cases were reviewed against the EU AI Act based on their intended purpose, the people affected, the AI system's behaviour, and the context in which it is deployed.

The assessment identified four different regulatory situations:

- **Case 1:** High-risk use case with a potential prohibited-practice issue
- **Case 2:** High-risk employment/recruitment use case
- **Case 3:** Customer-facing AI system where transparency is the primary concern
- **Case 4:** Minimal-risk product recommendation system

The recommended decisions are therefore different:

- **Case 1:** Deny and redesign
- **Case 2:** Approve with controls
- **Case 3:** Approve with controls
- **Case 4:** Approve

> **Consulting note:** These are first-pass classifications based on the facts provided. Final legal approval should verify the system's exact intended purpose, technical design, data processing, contractual roles, and applicable EU AI Act requirements.

---

## 1. Risk Overview

| Case | First-pass classification | Decision |
|---|---|---|
| Case 1 — Remote examination monitoring | High-risk with potential prohibited-practice issue | **Deny and redesign** |
| Case 2 — Recruitment screening | High-risk | **Approve with controls** |
| Case 3 — Customer service chatbot | Limited risk / transparency | **Approve with controls** |
| Case 4 — Product recommendations | Minimal risk | **Approve** |

---

# 2. Case 1 — Remote Examination Monitoring

## Classification

**Prohibited-practice concern — deny and redesign.**

The system is used in an education/examination context to monitor students and identify unusual behaviour during tests. Prohibited-practice concern in an education/examination context; deny as proposed and redesign.

## Proposed AI Architecture

**Student exam → webcam/technical signals → AI analysis → anomaly/stress/engagement flag → human invigilator review → human follow-up decision**

The AI should not automatically accuse or sanction students. Human review should remain part of the process.

## Roles

| Role | Responsibility |
|---|---|
| **Provider** | Company developing and placing the AI proctoring system on the market or putting it into service |
| **Deployer** | Online higher-education platform using the system |
| **Third-party vendor** | External AI/proctoring technology provider, if applicable |
| **Human oversight** | Invigilator team reviews flags before follow-up |

## Obligations / Controls

The system would require appropriate risk management, human oversight, logging, documentation, accuracy and robustness controls, and cybersecurity measures if deployed as a high-risk system.

The emotion/stress inference component requires specific legal assessment before deployment.

## Decision

**DENY AND REDESIGN**

### Recommended Redesign

Remove the emotion/stress inference component and focus the system on permitted indicators of potential examination misconduct.

AI-generated flags should be reviewed by an invigilator before any student is contacted or action is taken.

---

# 3. Case 2 — Recruitment Screening

## Classification

**High-risk.**

The AI system analyses and ranks candidates during recruitment and selection. Recruitment and selection of natural persons is an employment-related high-risk use under Annex III.

Human recruiters can review and override the AI ranking, but human review does not remove the system from the high-risk category.

## Proposed AI Architecture

**Job vacancy → candidate CV/application data → AI analysis → candidate ranking → recruiter review → recruiter override if appropriate → final recruitment decision**

## Roles

| Role | Responsibility |
|---|---|
| **Provider** | Company developing and placing the AI recruitment system on the market or putting it into service |
| **Deployer** | Recruitment company or employer using the system |
| **Third-party vendor** | External AI/recruitment technology provider, if applicable |
| **Human oversight** | Recruiters review and challenge the AI-generated ranking |

## Obligations / Controls

The deployment should include:

- Risk management
- Appropriate data governance
- Technical documentation
- Logging and record-keeping
- Human oversight
- Accuracy and robustness controls
- Cybersecurity
- Clear procedures for recruiters using and monitoring the system

Recruiters should not treat the AI ranking as an automatic decision.

## Decision

**APPROVE WITH CONTROLS**

The system can potentially be deployed, but the required high-risk controls and documentation must be established before launch.

---

# 4. Case 3 — Skincare Customer Service Chatbot

## Classification

**Limited risk / transparency.**

The system communicates directly with customers and generates responses to customer questions.

The main AI Act issue is transparency: customers should understand that they are interacting with an AI system.

The friendly name and human-like conversational style make clear disclosure particularly important.

## Proposed AI Architecture

**Customer visits website → customer starts chat → AI assistant answers questions → customer continues interaction or requests human support → human agent takes over when requested**

## Roles

| Role | Responsibility |
|---|---|
| **Provider** | Company developing and providing the AI chatbot |
| **Deployer** | Skincare brand using the chatbot on its website |
| **Third-party vendor** | External AI/chatbot provider, if applicable |
| **Human support** | Customer service employee takes over when requested |

## Obligations / Controls

The organisation should:

- Clearly disclose that the customer is interacting with an AI system
- Avoid deliberately misleading customers into believing they are communicating with a human
- Consider GDPR and data-protection requirements
- Consider consumer-protection requirements
- Monitor the accuracy of customer-facing responses

## Decision

**APPROVE WITH CONTROLS**

The chatbot can potentially be deployed provided appropriate transparency measures are implemented and the conversational design does not mislead customers about the nature of the interaction.

---

# 5. Case 4 — Personalised Grocery Recommendations

## Classification

**Minimal risk.**

The system recommends products based on customers' previous purchases and browsing activity.

The scenario does not indicate a prohibited practice or an identified high-risk use. It functions as a conventional personalised product-recommendation tool.

## Proposed AI Architecture

**Customer visits website → recommendation system analyses purchase/browsing history → AI generates product suggestions → recommendations displayed → customer decides whether to purchase**

## Roles

| Role | Responsibility |
|---|---|
| **Provider** | Company providing the recommendation technology, or the grocery company if it develops the system itself |
| **Deployer** | Grocery e-commerce company |
| **Third-party vendor** | External recommendation/AI technology provider, if applicable |
| **Human involvement** | Customer makes the final purchasing decision |

## Obligations / Controls

No specific AI Act risk-tier obligations arise from the minimal-risk classification described here.

However, the company should still consider:

- GDPR and data-protection requirements
- Consumer-protection requirements
- Accuracy of recommendations
- Potentially misleading or deceptive recommendations

## Decision

**APPROVE**

The recommendation feature can generally proceed from an AI Act risk-classification perspective, subject to applicable data-protection, consumer-protection and other relevant legal requirements.

---

# 6. Overall Consulting Recommendation

The four systems should **not be treated as having the same compliance pathway**.

| Case | Recommendation |
|---|---|
| **Case 1 — Examination monitoring** | **Deny and redesign** |
| **Case 2 — Recruitment screening** | **Approve with controls** |
| **Case 3 — Customer chatbot** | **Approve with controls** |
| **Case 4 — Product recommendations** | **Approve** |

### Final Recommendation

**Case 1** should be redesigned before deployment because its proposed emotion/stress inference creates a significant prohibited-practice concern.

**Case 2** can potentially proceed as a high-risk system, but only with appropriate controls, documentation, and effective human oversight.

**Case 3** can proceed with appropriate transparency measures so that customers understand they are interacting with AI.

**Case 4** can generally proceed as a minimal-risk application, while remaining subject to other applicable legal requirements.

---

## Consultant Conclusion

The assessment demonstrates that AI systems must be classified according to their **intended purpose, context, behaviour, and impact**, rather than simply because they use AI.

The appropriate consulting response therefore ranges from **redesigning a potentially prohibited practice**, to **controlled deployment of high-risk systems**, to **transparency measures**, and finally to **approval of a minimal-risk application**.