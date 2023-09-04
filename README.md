# aks-kustomization-demo
This repo demonstrates the use of demo to deploy AKS.

## View Kuztomization Configs
```
kubectl kustomize .
kubectl kustomize overlays/dev/
kubectl kustomize overlays/prod/
```

## Creating Namespaces if you dont have them already
```
kubectl create namespace dev; kubectl create namespace prod;
```

## Applying Kustomize Configs - (Using kubectl kustomize integration)
```
kubectl apply -k .
kubectl apply -k overlays/dev/
kubectl apply -k overlays/prod/
```