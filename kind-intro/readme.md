## Basic Kind "Hello World" cluster

1. To start the cluster:
   ```
   kind create cluster --config kind-demo/kind-demo-cluster.yaml  
   ```
2. To check additional cluster information:
    ```
    kubectl cluster-info --context kind-kind
    ```

3. It is possible to access a pod container via:
   ```
   k exec -it <pod_name> -- bin/bash
    ```

4. Kubectl apply deployment:
   ```
   k apply -f <file_name>
    ```
