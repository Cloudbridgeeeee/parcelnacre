# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 and Lambda | Encrypted report imports, checked row by row |
| Bedrock | Rider notes classified into exception types |
| SageMaker AI | Recurring cause detection, retrained monthly |
| DynamoDB | Shipments, exceptions and the decision log |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.
