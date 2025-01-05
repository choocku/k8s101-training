# Rollout commands
- You can see the status of the rollout by the below command

`$ kubectl rollout status deployment/myapp-deployment`

# To see the history and revisions

`$ kubectl rollout history deployment/myapp-deployment`

# Create the deployment

`$ kubectl apply -f deployment-definition.yaml`

- Edit **nginx:1.7.1** to **nginx:1.9.1** in **deployment-definition.yaml**

# Upgrade the image in deployment 

`$ kubectl apply -f deployment-definition.yaml`
