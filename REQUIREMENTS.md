# REQUIREMENTS.md --- GovAssist AI (AMD Slingshot)

## 1. Project Overview

GovAssist AI is a voice-first, explainable AI platform that helps Indian
citizens discover eligible government welfare schemes, understand
eligibility, prepare documents, and receive guided support for
applications. The system is optimized for an **edge--cloud hybrid
deployment on AMD hardware** for rural and low-bandwidth environments.

## 2. Target Users

-   Rural citizens with low digital literacy\
-   Common Service Centres (CSCs)\
-   NGOs and grassroots organizations\
-   District welfare officers (read-only dashboards)

## 3. Functional Requirements

### 3.1 User Interaction

-   FR1: The system shall support **voice input in multiple Indian
    languages** via Bhashini.
-   FR2: The system shall capture a citizen profile through a
    conversational Q&A.
-   FR3: The system shall provide **personalized eligible schemes**
    instead of generic lists.
-   FR4: The system shall explain eligibility with a clear **"Why
    Eligible?"** rationale.
-   FR5: The system shall generate a **personalized document
    checklist**.
-   FR6: The system shall support **voice-based form filling**.
-   FR7: The system shall perform a **reconfirmation step** before
    submission.
-   FR8: The system shall redirect users to the correct official
    government portal.

### 3.2 Eligibility Engine

-   FR9: The system shall use a **rule-based eligibility engine** as the
    primary decision layer.
-   FR10: The system shall use an LLM (AWS Bedrock) only for explanation
    and guidance.
-   FR11: All eligibility decisions must be explainable and auditable.

### 3.3 Document Handling

-   FR12: The system shall allow users to upload scanned documents.
-   FR13: The system shall use OCR (AWS Textract) to extract and
    validate key fields.
-   FR14: The system shall flag missing or inconsistent documents.

### 3.4 Tracking & Support

-   FR15: The system shall provide a dashboard to track application
    status.
-   FR16: The system shall support grievance submission (optional
    extension).

## 4. Non-Functional Requirements

### 4.1 Performance

-   NFR1: Voice response latency at edge should be \< 2 seconds.
-   NFR2: Eligibility matching should complete within 1 second.
-   NFR3: System must support at least 10 concurrent users per CSC node.

### 4.2 Scalability

-   NFR4: Cloud backend must scale to millions of users.
-   NFR5: System must support adding new schemes without major redesign.

### 4.3 Security & Privacy

-   NFR6: All data must be encrypted in transit and at rest.
-   NFR7: Minimal personal data collection principle must be followed.
-   NFR8: Role-based access control for admins and NGOs.

### 4.4 Reliability

-   NFR9: System availability target: 99.5% uptime.
-   NFR10: Edge nodes must operate in intermittent internet conditions.

## 5. Hardware Requirements (Prototype)

-   1 AMD CPU-based edge node at pilot CSC\
-   1 AMD GPU workstation for development\
-   Limited AMD cloud GPU instances for benchmarking

## 6. Success Metrics

-   30% reduction in document-related rejections\
-   40% increase in completed applications\
-   Average voice interaction time \< 5 minutes\
-   At least 3 Indian languages supported in pilot
