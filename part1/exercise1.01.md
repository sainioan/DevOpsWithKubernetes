## Part 1 exercise 1

Click [here](https://github.com/sainioan/randomStringGenerator.git) to go to my the app repository. 
### Command to create a cluster:
`k3d cluster create -a 1` 

### Command to create a deployment 
`kubectl create deployment randomstringgenerator --image=anniinasainio/randomstringgenerator`

### Output from the command `kubectl get pods`

```
NAME                                     READY   STATUS    RESTARTS   AGE
randomstringgenerator-655dd9cbfc-7h5ts   1/1     Running   0          56s
```

###Command to see thelogs

`kubectl logs -f randomstringgenerator-655dd9cbfc-7h5ts `

```
 vymNfn3wFHfGah 4.6.2022 17.23.42
 vymNfn3wFHfGah 4.6.2022 17.23.47
 vymNfn3wFHfGah 4.6.2022 17.23.52
 vymNfn3wFHfGah 4.6.2022 17.23.57
 vymNfn3wFHfGah 4.6.2022 17.24.02
 vymNfn3wFHfGah 4.6.2022 17.24.07
 vymNfn3wFHfGah 4.6.2022 17.24.12
 vymNfn3wFHfGah 4.6.2022 17.24.17
...
