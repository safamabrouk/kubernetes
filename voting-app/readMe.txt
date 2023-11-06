## get services
kubectl get svc

 kubectl create -f voting-app-pod.yml
 kubectl create -f voting-app-service.yml
## get service and pod 
 kubectl get pods,svc

## access to the application inside the port 

when we fo get services we have an ip
we can use that ip and the port to 
access in the navgateur the application of
voting-app 

the service nodeport (we have and ip cluster of the pod with the port 
we make sure to access to the application)

#### get the url to access to pod with service 

minkube service voting-service --url 

htpp://192.168.99.101:30004

### create the rediis pod 

kubectl create -f rediis-pod.yml
kubectl create -f rediis-service.yml

### create postgres ds

kubectl create -f postgres-pod.yml
kubectl create -f postgres-service.yml

## create worker 

kubectl create -f worker-pod.yml


### gt pods

kubectl get pods

### create result 

kubectl create -f result-pod.yml
kubectl create -f result-service.yml

### get the url of result application service 
minkube service result-service --url 


##create deployment (one deployment per type of pod .deploymenet = replicas of pods )
kubectl create -f result-app-deploy.yaml
kubectl create -f result-service.yaml 
minikube service result-service --url ## get the url of service we need it to communicate with pod result 
###repeat this with all kind of pod and if the pod is exposed 
create his service /

### deployment => replicas of pod insted of create one pod 
   we create 3 pods with the template of pod mentionned in the file 
   service => if the pod is exposed internally or externally 

