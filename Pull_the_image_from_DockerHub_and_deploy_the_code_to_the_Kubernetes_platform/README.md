We have to deploy the 2 yaml file using the below commands:

```
kubectl apply -f pod.yml

kubectl apply -f service.yml
```

find the minikube ip on our local use the below command.
```
minikube ip
```
Then, go to the browser use it the below details

```
minikubeIp:nodePort

ex:
http://192.168.49.2:31515/
```

**Output**
![image](https://user-images.githubusercontent.com/91359308/230558658-2c3c1f62-c141-4f75-84f5-1fea444fdbff.png)


