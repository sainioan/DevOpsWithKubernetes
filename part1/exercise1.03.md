## Part 1 exercise 3: 'Log output'

Click [here](https://github.com/sainioan/Apps/blob/main/Log%20output/manifests/deployment.yaml) to find the deployment.yaml file  

### Command to create a deployment using the yaml file
` kubectl apply -f manifests/deployment.yaml`
### Output from the command `kubectl get pods`
'kubectl get pods'
```
NAME                         READY   STATUS    RESTARTS   AGE
logoutput-6c7ccd5967-gc2p7   1/1     Running   0          10s
todo-app-57f85d79f8-6qf8d    1/1     Running   0          4h1m
```



###Command to see thelogs

`ubectl logs -f logoutput-6c7ccd5967-gc2p7 `

```
97fueaxY59MUVq 5.6.2022 13.39.19
97fueaxY59MUVq 5.6.2022 13.39.24
97fueaxY59MUVq 5.6.2022 13.39.29
97fueaxY59MUVq 5.6.2022 13.39.34
97fueaxY59MUVq 5.6.2022 13.39.39
...
