# Run Nginx pod

### My env

- macOS
- Docker desktop k8s

### Run pod

- filename : run-my-nginx.yaml

``` bash
kubectl apply -f <filename>
```

``` bash
kubectl get pods -o wide
```

- docker desktop k8s 의 경우, 포트 포워딩을 통해서 포트 지정해주어야 함

```bash
kubectl port-forward <pods name> 8888:80
```

- 접속 테스트

``` bash
curl localhost:8888
```
