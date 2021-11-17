# rhoas-helm-template

Example how to use RHOAS services with Helm.
This example deploys Kafka Example application to your cluster.

## Requirements

1. rhoas cli installed (https://github.com/redhat-developer/app-services-cli)
2. Red Hat account to login
3. Kafka Service deployed 

## Running chart 

1. Select Kafka service you want to use with this example
```
rhoas profile manage
```

2. Generate secrets and configuration maps
```
rhoas profile generate --file-format kube --folder=secrets
```

3. Apply them to your namespace
```
kubectl apply -f .rhoas
```

4. Run helm example

```
helm install . --generate-name 
```

