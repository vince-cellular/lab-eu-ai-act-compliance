# EU AI Act — Client Discussion & Final Sign-Off

## 1. Classification Comparison

After the consulting review, the partner revealed the intended categories for the four client scenarios.

The comparison showed that the consultant's first-pass classifications were aligned with the intended categories.

| Case | Partner's Intended Category | Consultant Classification | Match |
|---|---|---|---|
| Case 1 — Remote examination monitoring | Prohibited / potential prohibited-practice issue | High-risk with potential prohibited-practice issue | Yes — issue identified |
| Case 2 — Recruitment screening | High-risk | High-risk | Yes |
| Case 3 — Customer service chatbot | Limited risk / transparency | Limited risk / transparency | Yes |
| Case 4 — Grocery recommendations | Minimal risk | Minimal risk | Yes |

---

# 2. Case-by-Case Discussion

## Case 1 — Remote Examination Monitoring

### Intended Category

**Prohibited / potential prohibited-practice issue**

### Consultant Classification

**High-risk use case with a potential prohibited-practice issue**

### Discussion

The consultant identified the education/examination context as a high-risk concern and separately identified the use of emotion or stress inference as a potential prohibited-practice issue.

The client discussion confirmed that the emotion-recognition component was the key issue requiring attention.

### Final Recommendation

**Deny and redesign.**

The proposed emotion/stress inference should be removed. A redesigned system could focus on permitted indicators of potential examination misconduct and retain human review before any action is taken against a student.

---

## Case 2 — Recruitment Screening

### Intended Category

**High-risk**

### Consultant Classification

**High-risk**

### Discussion

The consultant correctly identified recruitment and candidate selection as an employment-related high-risk use under Annex III.

The discussion also confirmed that human review does not remove the system from the high-risk category. Recruiters must retain an effective role in reviewing and challenging AI-generated recommendations.

### Final Recommendation

**Approve with controls.**

The system can potentially be deployed once appropriate high-risk controls, documentation, human oversight and operational procedures are established.

---

## Case 3 — Customer Service Chatbot

### Intended Category

**Limited risk / transparency**

### Consultant Classification

**Limited risk / transparency**

### Discussion

The consultant identified the direct interaction between the AI assistant and customers as the key issue.

The natural conversational style and human-like presentation make it particularly important that customers understand they are interacting with an AI system.

### Final Recommendation

**Approve with controls.**

The company should provide clear transparency to customers and avoid designing the chatbot in a way that deliberately misleads users into believing they are communicating with a human.

---

## Case 4 — Grocery Product Recommendations

### Intended Category

**Minimal risk**

### Consultant Classification

**Minimal risk**

### Discussion

The consultant identified the system as a conventional product-recommendation application based on customer browsing and purchase history.

The system does not make decisions in an identified high-risk area and does not appear to involve a prohibited practice.

### Final Recommendation

**Approve.**

The system can generally proceed from an AI Act risk-classification perspective, while the company should still consider GDPR, data protection, consumer protection and other applicable requirements.

---

# 3. What Changed After the Client Discussion?

The client discussion did not materially change the consultant's classifications. The intended categories revealed by the partner were consistent with the consultant's first-pass assessment.

The discussion nevertheless helped validate several important points:

1. **Human oversight does not automatically change the AI Act risk category.**
   - This was particularly relevant to the recruitment case.
   - Human recruiters can review and override AI outputs, but the recruitment use remains high-risk.

2. **A single AI system can raise more than one regulatory issue.**
   - The examination-monitoring case combines an education context with a potential prohibited emotion-recognition practice.
   - The prohibited component therefore needs to be addressed rather than treating the whole system as an ordinary high-risk deployment.

3. **Transparency can be the main compliance issue even when a system is not high-risk.**
   - The customer-service chatbot does not become high-risk simply because it communicates naturally with customers.
   - The key issue is making the AI interaction sufficiently clear to users.

4. **Not every AI application requires a specific AI Act risk-tier control framework.**
   - The grocery recommendation system remains in minimal-risk territory based on the facts provided.
   - Other legal requirements can still apply independently of the AI Act risk classification.

---

# 4. Final Sign-Off

| Case | Final Decision |
|---|---|
| Case 1 — Remote examination monitoring | **DENY AND REDESIGN** |
| Case 2 — Recruitment screening | **APPROVE WITH CONTROLS** |
| Case 3 — Customer service chatbot | **APPROVE WITH CONTROLS** |
| Case 4 — Grocery recommendations | **APPROVE** |

## Final Consulting Position

The client should not treat all AI systems as having the same regulatory pathway.

The final recommendations are:

- **Case 1:** Do not launch as proposed. Remove or redesign the potentially prohibited emotion-recognition component.
- **Case 2:** Proceed only with the controls required for a high-risk recruitment system.
- **Case 3:** Proceed with appropriate transparency measures and clear communication that the customer is interacting with AI.
- **Case 4:** Proceed as a minimal-risk application, while continuing to address GDPR, data protection, consumer protection and other applicable requirements.

### Closing Note

The exercise demonstrated the importance of moving from a vague client request to:

**Business context → AI behaviour → affected people → AI Act classification → architecture → roles → controls → approval decision.**

The final classification should always be confirmed against the system's actual intended purpose, technical design and deployment context before production use.