# lugx-analytics-service
Analytics microservice for capturing and processing website user interaction data. Integrates with ClickHouse to store web analytics (page views, clicks, session time, etc.). Exposes APIs for collecting analytics data from the frontend. Containerized and deployed on Kubernetes.

kubectl apply -f k83/analytics-deployment.yaml
kubectl apply -f k83/analytics-service.yaml
kubectl apply -f k83/clickhouse-deployment.yaml
kubectl apply -f k83/clickhouse-service.yaml
