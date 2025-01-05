# Rollout commands
- You can see the status of the rollout by the below command

`$ kubectl rollout status deployment/myapp-deployment`

# To see the history and revisions

`$ kubectl rollout history deployment/myapp-deployment`

# Create the deployment

`$ kubectl apply -f deployment-definition.yaml`

- Edit **nginx:1.7.1** to **nginx:1.9.1** in **deployment-definition.yaml**

# Update the image in deployment 

`$ kubectl apply -f deployment-definition.yaml`

# To check status of upgrading or rollout
```
$ kubectl rollout status deployment/myapp-deployment
$ kubectl rollout history deployment/myapp-deployment
```

# To undo a change

`$ kubectl rollout undo deployment/myapp-deployment`

# To delete the deployment

`$ kubectl delete -f deployment-definition.yaml`
