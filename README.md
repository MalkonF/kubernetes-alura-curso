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

### Deletar os pods
```
kubectl delete pod nginx-pod
```

### Deletar todos os pods dentro do arquivo
```
kubectl delete -f .\primeiro-pod.yaml
```

### Abrir o terminal de determinado container
```
kubectl exec -it portal-noticias -- bash
```