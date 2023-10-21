## Selectors

See the labels inside the pod.yaml

```shell
kubectl get pod --selector os=ubuntu
```

To select multiples selector at once

```shell
kubectl get all --selector os=ubuntu,env=prod
```