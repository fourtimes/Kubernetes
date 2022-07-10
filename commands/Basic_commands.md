**To deploy the pod yml file**
```
kubectl apply -f (file current path)  => [ex: kubectl apply -f 1.yml] 
```
**View the all the pods**
```
kubectl get po -A
```
**To view the without namespace pod**
```
kubectl get po
```
**To view the with namespace pod**
```
kubectl get po -n (namespace name)
```
**Describe the pod**
```
 kubectl describe po (podname) -n (namespace name)
 ```
 **view the logs of the pod**
 ```
  kubectl logs po (podname) -n (namespace name)
 ```
 **Get all the labels of the pod**
 ```
 kubectl get po -A --show-labels
```
**Get the specified namespace pod**
```
kubectl get po -l (lables-name and keyword)-A
 ```
