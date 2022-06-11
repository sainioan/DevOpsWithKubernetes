# Part 1 exercise 7: ingress

1. Edit the application to write the timestamp and random string to the server.

2. Command to deploy the new version of the app  `kubectl apply -f manifests/deployment.yaml` using tag v.3

3. Command to create and apply the service  `kubectl apply -f manifests/service.yaml`

4. Create ingress yaml with the correct parameters. Command to apply the ingress file `kubectl apply -f manifests/ingress.yaml`

5. Command to check the server output  `curl localhost:8081/GET`
Output:
```
(base) anniinasainio@Anniinas-MacBook-Air Log output % curl http://localhost:8081/GET
 Rb7R5NBVBwblWn 11.6.2022 13.12.15%   
```
