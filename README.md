## Customized Confluent Open Source Helm Chart

You can find the original Confluent project [here](https://github.com/confluentinc/cp-helm-charts)

This has been customize dto our needs.



## Installing Charts

```
cd cp-helm-charts
helm install . 
```

## Documentation

This install the charts to your existing K8s cluster.

Out of the boc the above commad should install/provision a


- 3 node Kafka , Zokeeper
- Kafka and Kafka Connect deployed as Stateful sets
- Dynamic PVC prvisioning for Zokeeper Kafka and Kafka Connect


##Tips

To delete a cluster 
```
helm delete <chartname>

## You can list charts installed using 
helm list


##  to delete PVC's in one shot 
kubectl  delete  pvc --selector=release=<chartname>

``` 



