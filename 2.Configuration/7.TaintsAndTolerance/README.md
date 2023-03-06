### O que é
A afinidade do nó é uma propriedade dos pods que os atrai para um conjunto de nós (seja como uma preferência ou um requisito rígido). Taints são o oposto - eles permitem que um nó repela um conjunto de pods.

As tolerâncias são aplicadas aos pods. As tolerâncias permitem que o agendador agende pods com taints correspondentes. As tolerâncias permitem o escalonamento, mas não garantem o escalonamento: o escalonador também avalia outros parâmetros como parte de sua função.

Taints e tolerâncias trabalham juntos para garantir que os pods não sejam programados em nós inadequados. Um ou mais taints são aplicados a um nó; isso marca que o nó não deve aceitar nenhum pod que não tolere as manchas.


### Comandos Básicos

#### Criando uma uma taint para determinado node (nó)
`kubectl taint nodes minikube app=blue:NoSchedule` - Cria uma taint para o node *minikube* com as chaves *app=blue* com o efeito *NoSchedule*

#### Removendo uma uma taint para determinado node (nó)
`kubectl taint nodes minikube app=blue:NoSchedule` - O comando é o mesmo, mas com um sinal de menos "-" ao final

##### Valores para taint-effect
* *NoSchedule*
* *NoExecute*
* *NoSchedule*
