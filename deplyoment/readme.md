* change the service's pod selector with 'kubectl set selector'

* debug kubectl commands with --v 6 option
  kubeclt get pods --v 9

* patch:
  kubectl patch deployment <dep-name> -p '{"spec": {"minReadySeconds": 10}}'

* rollback:
  kubectl -n testbed rollout undo deploy/kubia-dep
  kubectl -n testbed rollout history deploy/kubia-dep
  kubectl -n testbed rollout pause deployment/kubia-dep
  kubectl -n testbed rollout resume deployment/kubia-dep
   kubectl -n testbed rollout status deploy/kubia-dep
