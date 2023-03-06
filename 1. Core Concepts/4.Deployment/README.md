### Comandos básicos

#### Criar deployment a partir de um yml
`kubectl create -f deployment.yml` - Cria um deployment

#### Deletar deployment
`kubectl delete deployment my-deployment -n default` - deleta o deployment chamado *nginx-deployment*

### Editar propriedade do deployment em execução
`kubectl edit rs -n default my-deployment`