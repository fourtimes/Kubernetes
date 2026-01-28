## Pod bacis commands:

**To deploy the pod yml file**
```sh
kubectl apply -f deployment.yml 
```
**View the all the pods**
```sh
kubectl get po -A
```
**To view the without namespace pod**
```sh
kubectl get po
```
**To view the with namespace pod**
```sh
kubectl get po -n (namespace-name)
```
**view the pod entire details**
```sh
kubectl get po  -n (namespace-name) -o wide
```
**Describe the pod**
```sh
 kubectl describe po (podname) -n (namespace-name)
 ```
 **view the logs of the pod**
 ```sh
  kubectl logs po (podname) -n (namespace-name)
 ```
 **Get all the labels of the pod**
 ```sh
 kubectl get po -A --show-labels
```
**Get the specified lables of the pod**
```sh
kubectl get po -l (lables-name and keyword)-A
 ```
**To view all the details of the namespace**
```sh
kubectl get all -n fourtimes
```
**To view the pod, service, endpoint details with specified namespace**
```sh
kubectl get po,svc,ep -n (namespace) -o wide
```
**Port forwarding**
```sh
kubectl port-forward svc/svc-name -n (namespace) hostPort:containerPort --address

ex:
---
k port-forward svc/fourtimes-po -n fourtimes 8080:80
```
**Rollout the status of deployment**
```sh
kubectl rollout status deployment/(deployment-name)
```