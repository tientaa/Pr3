Demo: a51cc8aa88e344e1f8ec6db014697d88-1431848550.us-east-1.elb.amazonaws.com:5153/api/reports/daily_usage
Demo: a51cc8aa88e344e1f8ec6db014697d88-1431848550.us-east-1.elb.amazonaws.com:5153/api/reports/user_visits



Microservices AWS Kubernetes Project
This project sets up a microservices architecture on AWS EKS (Elastic Kubernetes Service), including a PostgreSQL database and a Python analytics service. It provides configurations and deployment files for both cloud and local environments.

Project Structure
analytics/: Python analytics service

app.py: Main application logic
config.py: Configuration settings
requirements.txt: Python dependencies <br>
db/: SQL scripts for PostgreSQL <br>

1_create_tables.sql: Create tables <br>
2_seed_users.sql: Seed user data <br>
3_seed_tokens.sql: Seed token data <br>
deployment/: Kubernetes YAML files <br>

configmap.yaml: Environment variables configuration <br>
coworking.yaml: Python analytics service deployment <br>
postgresql-deployment.yaml: PostgreSQL deployment <br>
postgresql-service.yaml: PostgreSQL service definition <br>
pv.yaml: Persistent volume configuration <br>
pvc.yaml: Persistent volume claim <br>
deployment-local/: Local deployment configurations <br>

screen/: Screenshots of the deployment process <br>

buildspec.yaml: AWS CodeBuild configuration <br>

Dockerfile: Docker image build instructions for the Python service <br>

LICENSE.txt: License information <br>

README.md: Project documentation <br>

Getting Started <br>
Prerequisites <br>
AWS CLI <br>
kubectl <br>
Docker <br>
PostgreSQL <br>
Deployment <br>
Run the following command to deploy the services to your Kubernetes cluster: <br>

kubectl apply -f deployment/ <br>
Local Development <br>
Use configurations in deployment-local/ for local testing before deploying to AWS. <br>

License <br>
This project is licensed under the MIT License. <br>
