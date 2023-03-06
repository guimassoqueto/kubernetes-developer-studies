### Comandos Básicos

#### Criando uma service account
`kubectl create serviceaccount sa-example -n default` - Cria uma service account chamada *sa-example* no namespace default  

#### Criando um toke e associando a uma service account
`kubectl create token sa-example -n default` - Cria um token para a service account sa-example no namespace default