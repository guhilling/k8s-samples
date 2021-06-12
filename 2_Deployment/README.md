# Deployment als Ressource-Datei ablegen.
Das Deployment kann erzeugt werden mit:
```
oc create -f pod_apache.yaml
```

Um die Datei anzulegen:
```
oc create deployment apache --image=registry.access.redhat.com/ubi8/httpd-24:latest --dry-run=client -o yaml > Deployment_Apache.yaml
```

