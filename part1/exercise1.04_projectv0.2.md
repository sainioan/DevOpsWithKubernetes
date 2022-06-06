## Part 1 exercise 4


### Command to delete previous deployment:
 `kubectl delete deployment todo-app`

### Create new deployment.yaml 

### Command to Apply new deployment
`kubectl apply -f manifests/deployment.yaml` 

### Command to Get pods with `kubectl get pods`

```
NAME                         READY   STATUS    RESTARTS   AGE
logoutput-6c7ccd5967-gc2p7   1/1     Running   0          27h
todo-7d75676b7c-7gvzx        1/1     Running   0          13s
```

### Command to Get the logs

 `kubectl logs -f todo-7d75676b7c-7gvzx `

output:
```
> ls@1.0.0 start
> node todo.js

Server started in port 7000
'''
```