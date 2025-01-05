# Create the ConfigMap
`kubectl apply -f config-map.yaml`

# Get the ConfigMap info
```
kubectl get cm
kubectl describe configmap config-map
```
Let's output the same information in YAML format

`kubectl get configmap config-map -o YAML`

# Deploy the pod
`kubectl apply -f pod-definition.yaml`

# Deploy the service
`kubectl apply -f service-definition.yaml`

# Display the blue background on the browser

# Cleanup

```
kubectl delete -f service-definition.yaml
kubectl delete -f pod-definition.yaml
kubectl delete -f config-map.yaml
```
