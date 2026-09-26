# CloudAWSandGCP
Invoices arrive by email or web upload into S3. EventBridge routes the event, Step Functions orchestrates Textract + Bedrock Nova extraction to DynamoDB, and low-confidence cases pause the workflow for human approval via a WaitForTaskToken callback. Built with Java 21 Lambda and a React dashboard.
