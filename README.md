# devops

1. AWS/GKE
2. k8s managed cluster
3. Several namespaces (like product1, product2)
4. Each team has access only to own namespace
5. Add NACL
6. Some services have tolerations and taints
7. Each product based on microservice arch (http, https, udp) and only some services could connect to service from another product (another namespace)
8. Each product-solution has own ingress controllers (nginx, kong, istio)
9. Only one reason to be in one cluster - "just we want"
10. One of the product havn't access to the internet (based on events in AWS)
11. "Terraform controller"
12. CI/CD for whole company (Jenkins based)
13. Kubernetes layer should be separated from CloudInfrastructure layer (eg Terrafrom create ALB/NLB, not k8s). Like team Infra and k8s-team
14. Endpoints (sqs, s3, rds etc)
15. Monitoring (Prom)
16. Multi-Cloud Deployment (AWS + GCP)


Business case: Company1 acquire Company2, some teams start new functionality. No time to migrate to one Cloud, in one namespace etc (cross account connection)
DevOps team should help each team in each "company" to decrease (at least not increase) TTM.
DevOps team should unify monitoring tools, maybe even logging.
