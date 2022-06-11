# Part 1 exercise 8: project v05

1. Delete the previous cluster `k3d cluster delete` and open local port 8081 using the command
`k3d cluster create --port 8082:30080@agent:0 -p 8081:80@loadbalancer --agents 2`

2. Command to deploy the Todo app  `kubectl apply -f manifests/deployment.yaml` 

3. Command to create and apply the service  `kubectl apply -f manifests/service.yaml`

4. Create ingress yaml with the correct parameters. Command to apply the ingress file `kubectl apply -f manifests/ingress.yaml`

5. Command to check the server output  `curl localhost:8081/GET`
Output:
```
(base) anniinasainio@Anniinas-MacBook-Air Todo % curl http://localhost:8081/GET                                                 
<html> <head>A simple web page:</head><body><h1> Hello World!</p></h1></body></html>%                                                                                                                                       
```
