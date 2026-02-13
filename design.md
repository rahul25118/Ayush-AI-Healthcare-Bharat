# System Design: Ayush-AI Architecture

## 1. Tech Stack (AWS Ecosystem)
- **AI/ML Engine:** Amazon Bedrock (Claude 3.5 Sonnet) for medical reasoning.
- **Extraction:** Amazon Textract & Amazon Comprehend Medical.
- **Compute:** AWS Lambda (Serverless) for cost-efficiency.
- **Storage:** Amazon HealthLake (FHIR compliant) & Amazon S3.
- **Database:** Amazon DynamoDB (Patient logs).
- **Security:** AWS IAM & AWS KMS for data privacy.

## 2. Data Flow
1. **Input:** User uploads a photo of a prescription or speaks symptoms into the mobile app.
2. **Processing:** AWS Lambda triggers Amazon Bedrock to analyze the text/voice data.
3. **Reasoning:** The AI identifies medications and flags potential health risks.
4. **Output:** A simplified summary is sent back to the user in their local language.
5. 
