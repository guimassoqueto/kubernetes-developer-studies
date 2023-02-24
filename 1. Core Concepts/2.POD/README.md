### Comandos básicos
#### Criando um pod
`kubectl run nginx-pod --image nginx` - Vai criar um pod chamado *nginx-pod* com a imagem do nginx, neste exemplo

#### Criando um pod a partir de um yaml
`kubectl create -f pod.yml` - Cria um pod com as definições especificadas no arquivo yml

#### Verificando pods em execução
`kubectl get pods --namespace default` - Mostra todos os pods em execução no namespace *default*  
`kubectl get pods -n default` - Mesmo comando, porém abreviado

#### Obter descrição do pod em execução
`kubectl describe -n default pod nginx-pod` - Apresenta uma descrição detalhada do pod em execução, no caso *nginx-pod*

#### Deletar um pod em execução
`kubectl delete pod -n default nginx-pod` - Deleta o pod *nginx-pod* do namespace default 

### Editar propriedade do pod em execução
`kubectl edit pod -n default nginx-pod`