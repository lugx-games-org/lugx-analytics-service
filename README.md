# lugx-analytics-service
Analytics microservice for capturing and processing website user interaction data. Integrates with ClickHouse to store web analytics (page views, clicks, session time, etc.). Exposes APIs for collecting analytics data from the frontend. Containerized and deployed on Kubernetes.
### build image locally and push 

- docker build -t samathikisalka/analytics-service:latest .
- docker push samathikisalka/analytics-service:latest

#### Deploy Analytics Service

- kubectl apply -f k8s/analytics-deployment.yaml
- kubectl apply -f k8s/analytics-service.yaml

  #### clickHouse
  
- kubectl apply -f k8s/clickhouse-deployment.yaml
- kubectl apply -f k8s/clickhouse-service.yaml
- kubectl port-forward svc/clickhouse 8123:8123

  http://localhost:8123/



