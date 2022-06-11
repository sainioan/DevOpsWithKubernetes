# Part 1 exercise 1.09: More services

1. Create the pingpong app and add Dockerfile to the directoy
[pingpong](https://github.com/sainioan/Apps/tree/main/Pingpong)

2. Create the deployment and service files for the application.

3. Add a section to the ingress file that makes it possible to use the ingress file between two applications.

```
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: logoutput-ingress
spec:
  rules:
  - http:
      paths:
      - path: /GET
        pathType: Prefix
        backend:
          service:
            name: logoutput-svc
            port:
              number: 2345
      - path: /pingpong
        pathType: Prefix
        backend:
          service:
            name: pingpong-svc
            port:
              number: 2345

```

4. Test the applicaation 'http://localhost:8081/pingpong'

![PingPong](https://github.com/sainioan/DevOpsWithKubernetes/blob/main/part1/pingpong.jpg)

