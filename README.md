# ECS Fargate Deployment via GitHub Actions

This repo demonstrates a CI/CD pipeline that:
- Builds a Docker image
- Pushes it to Amazon ECR
- Deploys it via CloudFormation to ECS Fargate

### Deployed App:
- The container runs a basic NGINX server
- Accessible via Application Load Balancer after stack creation

### How to Deploy:
1. Push to `main` branch or manually trigger workflow
2. GitHub Actions will handle the rest

**CloudFormation Template**: `fargate.yml`  
**GitHub Workflow**: `.github/workflows/deploy.yml`
