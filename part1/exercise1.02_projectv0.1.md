## Part 1 exercise 2: Project v0.1: 'Todo'

Click [here](https://github.com/sainioan/Apps.git) to go to my the app repository containing the todo app.  

### Command to create a deployment 
`kubectl create deployment todo-app --image=anniinasainio/todo-app`

### Output from the command `kubectl get pods`

```
NAME                        READY   STATUS    RESTARTS   AGE
todo-app-57f85d79f8-6qf8d   1/1     Running   0          2m4s
```

###Command to see thelogs

`kubectl logs -f todo-app-57f85d79f8-6qf8d` 
```
> ls@1.0.0 start
> node todo.js

Server started in port 7000 `
```
