## Storage Class
A StorageClass provides a way for administrators to describe the "classes" of storage they offer. Different classes might map to quality-of-service levels, or to backup policies, or to arbitrary policies determined by the cluster administrators. Kubernetes itself is unopinionated about what classes represent. This concept is sometimes called "profiles" in other storage systems.

1. Create the storage class *storage-class.yaml* (will use the storage block from AWS in this example)
2. Create the Persistent Volume Claim associated with the storage class *pvc.yaml*
3. Create the Pod associated with Persistent Volume Claim *storage-class.yaml*