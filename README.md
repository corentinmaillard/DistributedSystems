# Distributed Systems Project
### Made by:
- Corentin Maillard
- Mourad Mettioui

## Description
This Git repository is used for the development of the **camera** component of our distributed systems project. The application uses Docker Desktop and runs on Kubernetes.

## Getting Started
### How to Create an Image
There are two images to create: 
1. **`getting-started`**: This will be our main pod for the camera feature in the future.
2. **`test-second-pod`**: A test pod used to experiment with DNS-based communication (details explained further below).

To build the images, run the following commands:

```
docker build -t getting-started .
docker build -t test-second-pod .
```

### Start Minikube and Load the Images

First, you need to start Minikube with the following command:

```
minikube start
```

You can also launch the Minikube dashboard with:

```
minikube dashboard
```

After that, to load the images on minikube you will need the command :

```
minikube image load getting-started
minikube image load test-second-pod
```
