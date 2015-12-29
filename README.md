# Kube Chart Repository


This repository contains [Helm](https://github.com/helm/helm) Charts for [Kube-solo](https://github.com/TheNewNormal/kube-solo-osx) and [Kube-Cluster](https://github.com/TheNewNormal/kube-cluster-osx) Apps.

####First install [Kube-Solo](https://github.com/TheNewNormal/kube-solo-osx) App
#####Then, add this Chart repo to Helm:
```console
$ helm up
$ helm repo add kube-charts https://github.com/TheNewNormal/kube-charts
$ helm up
```

###Install charts:

Install [Deis v2 Lite](https://github.com/deis/deis) chart:
```
$ helm fetch kube-charts/deis-lite
$ helm install deis-lite
$ kubectl --namespace=deis get pods  # to check pods
```

Install Wordpress chart:
```
$ helm fetch kube-charts/wordpress
$ helm install wordpress
$ kubectl get pods  # to check pods
```

