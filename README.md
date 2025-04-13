# Kubernetes Node.js App Deployment - Steps

## Step 1: Create a simple Node.js application.

## Step 2: Write a Dockerfile to containerize the app.

## Step 3: Build and push Docker image (Version 1) to Docker Hub.

## Step 4: Create Kubernetes deployment and service YAML file for Version 1.

## Step 5: Apply the YAML using `kubectl apply -f app-v1.yaml`.

## Step 6: Verify deployment using:
- `kubectl get pods`
- `kubectl get services`

## Step 7: Access the application using:
- `kubectl port-forward service/nodeapp-service 3000:3000`
- Visit `http://localhost:3000`

## Step 8: Modify the app (e.g., change message to “Hello from Version 2”).

## Step 9: Build and push Docker image (Version 2) to Docker Hub.

## Step 10: Create a new Kubernetes deployment YAML file for Version 2.

## Step 11: Apply the second version using `kubectl apply -f app-v2.yaml`.

## Step 12: Verify using `kubectl get pods` and access with:
- `kubectl port-forward pod/<nodeapp-v2-pod-name> 3000:3000`

## Step 13: Observe output to confirm version change.

## Step 14: Clean up resources using:
- `kubectl delete -f app-v1.yaml`
- `kubectl delete -f app-v2.yaml`
