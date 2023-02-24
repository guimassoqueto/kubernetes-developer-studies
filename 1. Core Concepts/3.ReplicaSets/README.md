### Comandos básicos

#### Criar replicaset a partir de um yml
`kubectl create -f replicaset.yml` - Cria um replicaSet

#### Deletar replicaset
`kubectl delete replicaset nginx-replicaset -n default` - deleta o replicaset chamado *nginx-replicaset*

### Editar propriedade do replicaset em execução
`kubectl edit rs -n default nginx-replicaset`