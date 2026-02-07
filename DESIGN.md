# DESIGN.md --- GovAssist AI (AMD Slingshot)

## 1. System Architecture (Edge--Cloud Hybrid)

### 1.1 Edge Layer (AMD-Powered)

Responsibilities: - Local Speech Processing (STT/TTS)\
- Pre-processing of uploaded documents\
- Caching frequently used scheme rules\
- Reducing cloud dependency for rural areas

Components: - AMD CPU edge node\
- Lightweight voice service (Bhashini client)\
- Local rule cache\
- Secure local storage (encrypted)

### 1.2 Cloud Layer (AWS)

Responsibilities: - Advanced reasoning and explainability\
- Centralized scheme knowledge base\
- Document validation and storage\
- Application tracking and analytics

Components: - AWS Bedrock (LLM for explanations)\
- FastAPI backend\
- AWS Textract (OCR)\
- PostgreSQL + DynamoDB\
- AWS S3 for documents\
- CloudWatch monitoring

## 2. Data Flow

1.  User speaks → Edge node captures audio\
2.  Bhashini converts speech to text\
3.  Citizen profile is extracted\
4.  Rule-based eligibility engine matches schemes\
5.  AWS Bedrock explains eligibility\
6.  Document checklist is generated\
7.  User fills forms via voice\
8.  Reconfirmation step validates data\
9.  Redirect to official portal

## 3. Eligibility Engine Design

-   Deterministic rule layer (age, income, state, category)\
-   AI layer used only for reasoning and natural language explanation\
-   Every decision is logged with traceable policy references

## 4. Document Processing

-   Uploaded documents are pre-processed at edge\
-   AWS Textract extracts fields\
-   System validates consistency with profile\
-   Missing fields are flagged with guidance

## 5. Security Design

-   End-to-end encryption\
-   Aadhaar OTP optional verification\
-   Role-based access control\
-   Audit logs for all decisions

## 6. UI/UX Design Principles

-   Large buttons and simple layout\
-   Voice-first interaction\
-   Minimal text, maximum audio feedback\
-   Multilingual support\
-   Step-by-step guided flow

## 7. Deployment Plan

Phase 1: Prototype at 1--2 CSC centers\
Phase 2: District-level pilot\
Phase 3: State-wide rollout\
Phase 4: National scaling

## 8. AMD Optimization Strategy

-   Use AMD CPU for local speech processing\
-   Use AMD GPU for LLM inference testing\
-   Benchmark latency and energy efficiency\
-   Optimize edge--cloud workload split
