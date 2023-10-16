## Node Selector

1. First add a label to a node.
```shell
kubectl label nodes <node-name> <label-key>=<label-value>
```

2. Create the pod with "spec.nodeSelector.<label-key>:<label-value>