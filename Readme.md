kubectl get pod
kubectl apply -f mongo-config.yml
kubectl apply -f mongo-secret.yml
kubectl apply -f mongo.yml
kubectl apply -f webapp.yml

kubectl get all
kubectl get configmap
kubectl get secret
kubectl describe service webapp-service
kubectl describe pod mongo-deployment-855b879886-zgc69
kubectl logs webapp-deployment-9fccd564d-9b5pl

# To access weapp on browser
kubectl get svc => chosse nodeport
minikube ip => http://192.168.49.2
kubectl get node -o wide


#acessable => http://192.168.49.2:30100/