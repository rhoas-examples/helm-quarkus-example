# rhoas-helm-template

rhoas-helm-example

## Running chart 

Select services you want to run
```
rhoas profile manage
```

Generate secrets and configuration maps and apply them to your namespace
```
rhoas profile generate --file-format kube --folder=secrets
kubectl apply -f .rhoas
```



```
helm install . --generate-name 
```

