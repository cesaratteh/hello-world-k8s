# Hello World App

## Run Locally

```bash
mvn clean package
```

```bash
java -jar target/hello-world-1.0-SNAPSHOT.jar
```

## Run in Docker

```bash
docker build -t hello-world:latest .
```

```bash
docker run -p 8080:8080 hello-world:latest
```

## Run in Kubernetes
```bash
kubectl apply -f k8s-deployment.yaml
```

```bash
kubectl get pods
```

```bash
kubectl port-forward svc/hello-svc 8080:80
```

Access: http://localhost:8080/api/hello
