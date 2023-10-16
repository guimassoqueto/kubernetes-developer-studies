change the default namespace from *default* to another namespace already running

```shell
kubectl config set-context $(kubectl config current-context) --namespace<name-of-namespace>
```