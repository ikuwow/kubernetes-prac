kubernetes-prac
===

workthrough 101
http://kubernetes.io/docs/user-guide/walkthrough/

## cluster create

```
# small cluster
$ gcloud container clusters create workthrough \
    --disk-size=64 \
    --machine-type=g1-small \
    --num-nodes=2
# configure kubectl
$ gcloud container clusters get-credentials workthrough
```

## pod create

```
$ kubectl create -f pod-nginx.yml
```

