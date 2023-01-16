# kubernetes-training
## TP2
pour lancer le deploy; il suffit de faire un 
 kubectl apply -f nginx-webapp.yml
 ouvrir le port decout avec un  kubectl port-forward simple-webapp-color 8080:8080 --address 0.0.0.0
 puis alle dans le navigateur: addIP:8080

## TP3
lance le service sur le NameSpace production: kubectl apply -f service-nodeport-web.yml -n production; 
pour voire laddIP du service dans le clurster: kubectl -n production get services;
pour voire laddIP externe: kubectl -n production describe svc service-nodeport-web
pour voir lappli: alle dans le navigateur etentré addIP(machine physique ou vagrant):30008
 puis restualise pour voir la manifestation du loadbalancer sur nos deux sites.
