# EU AI Act — Partner Case Review

## Consulting Review

This document contains the four client briefs received from the partner and the consultant's first-pass assessment of each case.

The classifications are based on the facts provided in each client brief and should be validated against the final system design, intended purpose, data processing, and applicable EU AI Act requirements.

---

# Case 1 — Remote Examination Monitoring

## Partner Client Brief

An online higher-ed platform running remote-proctored exams wants to reduce exam misconduct. They’re looking at a webcam-based add-on that scores each student’s engagement and stress levels in real time during the exam and flags anything unusual to the invigilator team for follow-up. Most flags get a quick human look before anyone’s contacted.

## Consultant Review

### Likely Category

**High-risk use case, but the proposed emotion-recognition component raises a potential prohibited-practice issue requiring further assessment.**

### Why This Is My First-Pass Call

The system is used in an education/examination context to monitor students during tests. This creates a high-risk concern.

The proposed inference of students' stress and engagement creates an additional concern that must be assessed against the EU AI Act's prohibited-practice rules concerning emotion recognition.

### Proposed AI Architecture

**Student exam → webcam/technical signals → AI analysis → anomaly flag → human invigilator review → human follow-up decision**

### Provider

The company developing and placing the AI proctoring system on the market or putting it into service.

### Deployer

The online higher-education platform using the system.

### Third-Party Vendor

Any external company supplying the AI/proctoring technology.

### Required Obligations / Controls

- Risk management
- Human oversight
- Logging and record-keeping
- Technical documentation
- Accuracy and robustness
- Cybersecurity
- Assessment of the emotion-recognition component
- Removal or redesign of the emotion-recognition component if it falls within a prohibited practice

### Decision

**DENY AND REDESIGN**

### Redesign

Remove the emotion/stress inference component and focus the system on permitted indicators of potential examination misconduct.

AI-generated flags should be reviewed by an invigilator before any student is contacted or action is taken.

---

# Case 2 — Recruitment Screening

## Partner Client Brief

A national recruitment company wants to help large employers screen candidates for engineering and technical vacancies. The AI system should analyse CVs, application responses, relevant qualifications, and work-history information to rank applicants against the requirements of a vacancy. Recruiters would receive a ranked shortlist and they would review the shortlist and could override the ranking before any candidate is rejected or invited to interview.

## Consultant Review

### Likely Category

**High-risk**

### Why This Is My First-Pass Call

The AI system is being used to analyse, evaluate and rank natural persons during a recruitment and selection process.

Recruitment and selection is an employment-related use covered by the high-risk category in Annex III of the EU AI Act.

The system directly influences which candidates may progress to interviews or be rejected.

The fact that recruiters review the ranked shortlist and can override the AI does not by itself remove the system from the high-risk category.

### Proposed AI Architecture

**Job vacancy requirements → candidate CV/application data → AI analyses qualifications and work history → AI ranks candidates → recruiter reviews ranked shortlist → recruiter can override the ranking → recruiter makes the final decision about interview or rejection**

### Provider

The company that develops and places the AI recruitment system on the market or puts it into service.

### Deployer

The recruitment company or employer using the AI system to screen and rank candidates.

### Third-Party Vendor

An external AI or recruitment technology provider if the recruitment company obtains the system from another company.

### Required Obligations / Controls

- Risk management
- Appropriate data governance
- Technical documentation
- Logging and record-keeping
- Human oversight
- Accuracy and robustness controls
- Cybersecurity measures
- Clear procedures for recruiters on how to use, monitor and challenge the AI output
- The AI ranking should not be treated as an unquestioned automatic decision

### Decision

**APPROVE WITH CONTROLS**

### Why

The proposed recruitment system can potentially be deployed as a high-risk AI system, but approval should depend on the required high-risk controls being implemented and documented.

Human recruiters must have an effective role in reviewing and challenging the AI output rather than simply accepting the ranking automatically.

---

# Case 3 — Customer Service Chatbot

## Partner Client Brief

A skincare brand wants a friendlier shopping experience on their site. They’re building a chat assistant, given a first name and a casual tone, to handle order and product questions so it feels less like “submitting a ticket” and more like chatting with someone on the team. It only hands off to a human if a customer specifically asks for one.

## Consultant Review

### Likely Category

**Limited risk / transparency**

### Why This Is My First-Pass Call

The system is a customer-facing AI assistant that communicates directly with customers.

The main AI Act issue is transparency: customers should be made aware that they are interacting with an AI system.

The fact that the assistant has a first name and uses a casual, human-like tone makes clear disclosure particularly important.

There is no indication that the system is being used for recruitment, employment, education, law enforcement or another Annex III high-risk purpose.

### Proposed AI Architecture

**Customer visits website → customer starts chat → AI assistant answers order/product questions → AI provides response → customer continues interaction or requests human support → human agent takes over when requested**

### Provider

The company that develops and places the AI chatbot on the market or puts it into service, depending on the implementation.

### Deployer

The skincare brand using the chatbot on its website to interact with customers.

### Third-Party Vendor

An external AI/chatbot provider if the skincare brand uses a third-party system or model.

### Required Obligations / Controls

- Clearly disclose that the customer is interacting with an AI system
- Do not deliberately present the chatbot in a way that misleads customers into believing they are communicating with a human
- Consider data-protection requirements
- Consider consumer-protection requirements
- Monitor the accuracy of customer-facing responses

### Decision

**APPROVE WITH CONTROLS**

### Why

The customer-service chatbot can potentially be deployed, but the company should implement appropriate AI transparency measures and ensure that the conversational design does not mislead customers about the nature of the interaction.

---

# Case 4 — Personalised Grocery Recommendations

## Partner Client Brief

A grocery e-commerce company wants to increase average order size. They’re adding a “you might also like” module to the homepage that surfaces suggestions based on what a shopper has bought or browsed before. Nothing else about the account or checkout flow changes.

## Consultant Review

### Likely Category

**Minimal risk**

### Why This Is My First-Pass Call

The AI system is being used to recommend products to customers based on their previous purchases and browsing activity.

It does not make decisions about employment, education, access to essential services, law enforcement or another identified high-risk area.

It also does not appear to involve a prohibited AI practice or a specific transparency-triggering interaction with an AI system.

The system is functioning as a conventional product-recommendation tool to support online shopping.

### Proposed AI Architecture

**Customer visits grocery website → recommendation system analyses previous purchases and browsing activity → system generates personalised product suggestions → “you might also like” module displays recommendations → customer decides whether to purchase**

### Provider

The company that develops and provides the AI recommendation system, or the grocery e-commerce company if it develops the system itself.

### Deployer

The grocery e-commerce company using the recommendation system on its website.

### Third-Party Vendor

An external AI, recommendation or e-commerce technology provider if the grocery company obtains the recommendation system from another company.

### Required Obligations / Controls

There are no specific AI Act obligations arising from a minimal-risk classification in this scenario.

However, the company should still consider:

- GDPR and data-protection requirements
- Consumer-protection requirements
- Whether recommendations are accurate
- Whether recommendations could be misleading or deceptive

### Decision

**APPROVE**

### Why

The proposed recommendation feature appears to be a minimal-risk AI application and does not trigger a specific AI Act risk-tier requirement based on the facts provided.

The company can generally proceed, subject to applicable data-protection, consumer-protection and other relevant legal requirements.

---

# Overall Partner Case Assessment

| Case | Consultant Classification | Decision |
|---|---|---|
| Case 1 — Remote examination monitoring | High-risk + potential prohibited-practice issue | **Deny and redesign** |
| Case 2 — Recruitment screening | High-risk | **Approve with controls** |
| Case 3 — Customer service chatbot | Limited risk / transparency | **Approve with controls** |
| Case 4 — Grocery recommendations | Minimal risk | **Approve** |

---

## Consulting Conclusion

The four cases demonstrate that the AI Act classification depends on the **intended purpose, context, system behaviour and people affected**, rather than simply on whether a system uses AI.

The appropriate consulting response ranges from redesigning a potentially prohibited practice, to controlled deployment of high-risk systems, to transparency measures, and finally to approval of a minimal-risk application.