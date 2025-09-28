# Kubernetes Helm 101

This repos demonstrates a number of minimal Kubernetes and Helm setups.

## Minimal Kubernetes Pod

[`minimal-k8s/pod.yaml`|(minimal-k8s/pod.yaml) deploys a minimal pod that prints "Hello, world!" every 30 seconds. The pod will continue running until stopped.

Deploy the pod with `kubectl apply -f minimal-k8s/pod.yaml`.

To stop the pod, use `kubectl delete pod minimal`.

## Minimal Helm chart

[`minimal-helm`](minimal-helm) wraps the minimal Kubernetes pod into a minimal Helm chart.

Deploy the chart with `helm install minimal-helm ./minimal-helm`.

To remove everything again, run `helm delete minimal-helm`.
