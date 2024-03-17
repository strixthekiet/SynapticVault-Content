---
tags:
  - CompSci/cloud-computing
aliases:
  - "#CompSci/cloud-computing"
  - cloud
  - cloud computing
---
# Cloud Computing
### Description:
- [Holori - Cross Cloud Management Platform](https://app.holori.com/dashboard/)
### Vertical scaling vs horizontal scaling:
- Scale up vs scale out
- Bigger machine vs more machines
### Public vs private cloud

| Factors                     | Public Cloud                                                 | Private cloud                                   |
| --------------------------- | ------------------------------------------------------------ | ----------------------------------------------- |
| Resources                   | Resources are shared among multiple customers                | Resources are shared with a single organization |
| Tenancy                     | Data of multiple organizations is stored in the public cloud |                                                 |
| Pay Model                   | Pay what you used                                            | Have a variety of pricing models                |
| Operated by                 | Third-party service provider                                 | Specific  organization                          |
| Scalability and Flexibility | It has more scalability and flexibility                      |                                                 |
| Expensive                   | less expensive                                               | More expensive                                  |
| Availability                | The general public (over the internet)                       |                                                 |
### Cloud computing categories:
- Comparision:

|                  | Traditional | IaaS | CaaS | PaaS | FaaS | SaaS |
| ---------------- | ----------- | -------- | -------- | -------- | -------- | -------- |
| Data & config    | ✅          | ✅       | ✅       | ✅       | ✅       | ✅       |
| Application code | ✅          | ✅       | ✅       | ✅       | ✅       | 🛑       |
| Scaling          | ✅          | ✅       | ✅       | ✅       | 🛑       |    🛑      |
| Runtime          | ✅          | ✅       | ✅       | 🛑       |   🛑       |    🛑      |
| OS               | ✅          | ✅       |   🛑       |    🛑      |   🛑       |     🛑     |
| Virtualization   | ✅          |    🛑      |   🛑       |      🛑    |     🛑     |    🛑      |
| Hardware         | ✅          |   🛑       |     🛑     |       🛑   |   🛑       |    🛑      |

|                                        | [[Amazon Web Service]]                                     | [[Microsoft Azure]]                                                                   | [[Google Cloud Platform\|GCP]]                     |
| -------------------------------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------------- | -------------------------------------------------- |
| **Compute**                            | Amazon EC2, Amazon ECS, AWS Lambda                         | Azure Virtual Machines, Azure Container Instances, Azure Functions                    | Compute Engine, Kubernetes Engine, Cloud Functions |
| **Storage**                            | Amazon S3, Amazon EBS, Amazon EFS                          | Azure Blob Storage, Azure Disks, Azure Files                                          | Cloud Storage, Cloud Bigtable, Cloud Filestore     |
| **Databases**                          | Amazon RDS, Amazon DynamoDB, Amazon Aurora                 | Azure SQL Database, Azure Cosmos DB, Azure PostgreSQL                                 | Cloud SQL, Cloud Spanner, Cloud Firestore          |
| **Networking**                         | Amazon VPC, Amazon Route 53, AWS Transit Gateway           | Azure Virtual Network, Azure DNS, Azure ExpressRoute                                  | Cloud Networking, Cloud DNS, Cloud VPN             |
| **Machine Learning & AI**              | Amazon SageMaker, Amazon Rekognition, Amazon Comprehend    | Azure Machine Learning, Azure Cognitive Services, Azure Databricks                    | AI Platform, Vertex AI, Cloud AutoML               |
| **Serverless Computing**               | AWS Lambda, Amazon API Gateway, AWS Step Functions         | Azure Functions, Azure Logic Apps, Azure Durable Functions                            | Cloud Functions, Cloud Run, Cloud Workflows        |
| **Containers**                         | Amazon ECS, Elastic Container Service for Kubernetes (EKS) | Azure Container Instances (ACI), Azure Kubernetes Service (AKS)                       | Kubernetes Engine (GKE), Cloud Run                 |
| **Identity & Access Management (IAM)** | AWS IAM, Amazon Cognito                                    | Azure Entra ID, Policies, RBAC (allows for more specific conditions like VM location) | Cloud IAM, Google Cloud Identity                   |
