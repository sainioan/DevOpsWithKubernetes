
1. Add a simple webpage node app to todo.js in todo app.

2. Commmand to apply new deployment file `kubectl apply -f manifests/deployment.yaml` with a tag 2.0.0

3. Command to get the pods with `kubectl get pods`

```
NAME                                READY   STATUS    RESTARTS       AGE
hashresponse-dep-6fd594cb99-82kfx   1/1     Running   0              98m
logoutput-6c7ccd5967-gc2p7          1/1     Running   1 (115m ago)   3d4h
todo-7676c9766d-w7pcv               1/1     Running   0              9m26s
```

4. Command to forward ports: `kubectl port-forward todo-7676c9766d-w7pcv 5000:5000`
```
Forwarding from 127.0.0.1:5000 -> 5000
Forwarding from [::1]:5000 -> 5000

```
5.  Command to get the contents of the simple webpage `curl localhost:5000/GET`
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
