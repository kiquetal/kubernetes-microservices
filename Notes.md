#### Install minikube

-  eval $(minikube docker-env)

#### Pods are not visisble outside the cluster

- kubectl exec webapp ls
- kubectl -it exec webapp sh 
- 
#### Services

- Is a long runing object, will have an IP address stable fixPort
 
service-> selector app:webapp

pod -> labels app:webapp

kubectl describe svc fleetman-webapp

##### NodePort and clusterIP

- NodePort: Expose the port to the outside world.
  nodePort: greather than 30000

- ClusterIP: only be accesible inside cluster, private services

#### Using minikube

- minikube start
- minikube docker-env
export DOCKER_TLS_VERIFY="1"
export DOCKER_HOST="tcp://192.168.49.2:2376"
export DOCKER_CERT_PATH="/home/kiquetal/.minikube/certs"
export MINIKUBE_ACTIVE_DOCKERD="minikube"


#### API Gateway

- Simple source of truth
- Maps income requests to microservices

#### 
