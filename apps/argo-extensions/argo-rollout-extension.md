Install argo rollout (in ui argocd)
https://github.com/argoproj-labs/rollout-extension
Install Argo CD and Argo CD Extensions Controller: https://github.com/argoproj-labs/argocd-extensions
Use the same install.yaml into the kustomize example.

Create argo-rollouts extension in argocd namespace
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj-labs/rollout-extension/v0.2.1/manifests/install.yaml

Install argo-rollout
https://argoproj.github.io/argo-rollouts/installation/

kubectl create namespace argo-rollouts
kubectl apply -n argo-rollouts -f https://github.com/argoproj/argo-rollouts/releases/latest/download/install.yaml


Test rollout
https://argoproj.github.io/argo-rollouts/getting-started/