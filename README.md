# Rh Platform Candidate Assessment
Please Select from one of the following options:
1. Create a simple Hello World application (any language you prefer) and deploy it using a localized version of Kubernetes (minikube, k3s, etc).
- Ensure the application is containerized
- Configure the application to be deployed in QA and Production
- Include some form of CI/CD
  
2. Create a terraform module for an Amazon API Gateway which forwards requests to an SNS/SQS fanout distribution
- The Gateway should have some form of security built in (IP whitelist, mTLS, Lambda Auth)
- The SNS/SQS topic should also be created with terraform. Consider that multiple queues may be needed which represent services that might need to ingest the incoming requests through the gateway

3. Create a Helm values file which could be used to install and configure the kube-prometheus stack using the chart at https://github.com/prometheus-community/helm-charts/tree/main/charts/kube-prometheus-stack
- The configuration should be made for monitoring a production kubernetes cluster
- Some form of alerting should be configured in the solution.
- Consider integrations with external tools (Slack, Email, a paging system) for "Eventing"


The total time spent should be roughly 1 to 3 hours. Note that the assesment is open-ended and does not have a single "solution", so keep in mind any tradeoffs, assumptions, or limitations you encounter. Completeness is not the goal of this assement, but more an evaluation of how a problem is approached. Note that option 1 must be demoable. Option 2 does not need to be demoable (i.e. no AWS account needed and applying the terraform is not necessary). Option 3 does not need to be demoable, but if you are able to demo the installation of the chart in a localized k8s distribution (minikube, k3s, etc.) feel free to do so. 

Once you've completed the assesment, please upload the solution to github so that the team can review it.
