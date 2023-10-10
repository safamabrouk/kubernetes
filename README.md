# kubernetes
## commands for replicatSet 
    kubectl create -f replicatset-definition.yml
    kubectl get replicatset
    kubectl delete replicatset myapp-replicaset
    kubectl replace -f replicatset-definition.yml
    kubectl scale --replicas=6 -f replicatset-defnition.yml
    kubectl creat -h 
    kubectl create deployment -h 
    kubectl create deployment front-end --image=nginx --replias=3

