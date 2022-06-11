
1. Delete previous cluster `k3d cluster delete`

2. Command to open local 8081 to 80 in k3d-k3s-default-serverlb and local 8082 to 30080 in k3d-k3s-default-agent-0 `k3d cluster create --port 8082:30080@agent:0 -p 8081:80@loadbalancer --agents 2'

3. Commmand to apply new deployment file `kubectl apply -f manifests/deployment.yaml`

4. Create the service.yaml
 [service.yaml file](https://github.com/sainioan/Apps/blob/main/Todo/manifests/deployment.yaml)

5. Command to create and apply the service `kubectl apply -f manifests/service.yaml`

6.  Command to get the contents of the simple webpage `curl localhost:8082/GET`

The response:
```
 <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<title>Error</title>
</head>
<body>
<pre>Cannot GET /</pre>
</body>
</html>
 ```

