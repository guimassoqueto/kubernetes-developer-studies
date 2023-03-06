### Comandos Básicos

#### Criando uma uma label para o node
`kubectl label nodes minikube size=Large` - Cria uma taint para o node *minikube* com as chaves *app=blue* com o efeito *NoSchedule*

### Relacionar o pod ao Node
Verifique que o .yml do pod a ser criado possui spec.nodeSelector.size: Large, para poder criá-lo neste node