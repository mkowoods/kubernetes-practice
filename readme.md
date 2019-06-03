### Kubernetes Zoo

Projects:
 - Elastic Search
   - Single Instance StatefulSet(DaemonSet used to handle node config: [related issue](https://github.com/pires/kubernetes-elasticsearch-cluster/issues/85))
     - Deploy: `kubectl apply -f basic-elasticsearch.yaml` 
   - Simple Cluster of 3 Instances/2 Masters sized to fit on a ns-standard-1 instance from gcp
     - Deploy: `chmod +x deploy.sh && ./deploy.sh` 
     - Note this can take 10-15 Minute before the service is available, probably due to CPU limits
 - Sample wordpress App with MySql - Makes use of persistent volumes/StatefulSets
 - Basic Guestbook App
    - Redis Master/Slave Configuration
    - Ingress Service

 
useful images:
 - for performing nslookup/ping
   - `kubectl run bb-diagnostics --image=radial/busyboxplus:curl -it --rm`

### Command Cheatsheet
  - `kubectl top nodes`
  - `kubectl top pods`
  - `kubectl logs -f [POD]`
  - `kubectl get all`
  - `gcloud container clusters resize [CLUSTER_NAME] --node-pool [POOL_NAME] --num-nodes [NUM_NODES]`