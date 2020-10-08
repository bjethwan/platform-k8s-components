argocd app create bootstrap-cluster \
--repo https://github.com/bjethwan/platform-k8s-components \
--path argocd-bootstrapper \
--dest-server https://kubernetes.default.svc  \
--dest-namespace argocd  \
--sync-policy automated \
--self-heal \
--sync-option Prune=true



