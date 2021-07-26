# kubernetes-alura-curso

## Comandos

### Criando um pod
```
kubectl run nginx-pod --image=nginx:latest
```

### Acompanha em tempo real o que está acontecendo no cluster
```
kubectl get pods --watch
```

### Formata a saída do comando de maneira wide(ampla)
```
kubectl get pods -o wide
```

### Formata a saída do comando de maneira wide(ampla)
```
kubectl get nodes -o wide
```

### Exibe todos os svc
```
kubectl get svc
```

### Exibe todos os config maps
```
kubectl get configmap
```

### Exibe informações sobre o replicaset
```
kubectl get replicaset
```

### Exibe informações sobre os config maps
```
kubectl describe configmap db-configmap
```

### Exibe informações sobre os pods

```
kubectl describe pod nginx-pod
```

### Abre o arquivo de configuração do pod
```
kubectl edit pod nginx-pod
```

### Gerar pods de maneira declarativa
```
kubectl apply -f .\primeiro-pod.yaml
```

### Gera config maps de maneira declarativa
```
kubectl apply -f .\db-configmap.yaml
```

### Deletar os pods
```
kubectl delete pod nginx-pod
```

### Deletar todos os pods dentro do arquivo
```
kubectl delete -f .\primeiro-pod.yaml
```

### Deletar todos os svc's
```
kubectl delete svc --all
```

### Abrir o terminal de determinado container
```
kubectl exec -it portal-noticias -- bash
```