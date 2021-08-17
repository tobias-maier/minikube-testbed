kubectl logs <pod> -c <container>
kubectl port-forward <pod-name> <machine-port>:<container-port>

labels:
======
show all labels: kubectl get po --show-labels
show some labels: kubectl get po -L env,app,version
modify:
 kubectl label po <name> key=value --overwrite

annotation:
==========
kubeclt annotate pod <podname> key=value (--overwrite)
