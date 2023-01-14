# kubernetes-training
pour lancer le deploy; il suffit de faire un 
 kubectl apply -f nginx-webapp.yml
 ouvrir le port decout avec un  kubectl port-forward simple-webapp-color 8080:8080 --address 0.0.0.0
 puis alle dans le navigateur: addIP:8080
