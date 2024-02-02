# Custom CephBlockPool

Ein Beispiel für einen eigenen ```CephBlockPool``` mit ```Erasure Coding```.

Siehe auch:
- https://rook.io/docs/rook/latest/CRDs/Object-Storage/ceph-object-store-crd/
- https://docs.ceph.com/en/latest/rados/operations/erasure-code/

In OpenShift Data Foundation wird dies im "Internal Mode" _nicht_ unterstützt!

In der Storageclass _muss_ der Metadatapool (```pool```) 3-way-replication unterstützen.

Anlegen:

```
kubectl apply -k .
```
