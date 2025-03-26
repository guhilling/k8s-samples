# Mehrere Ressourcen als Ressource-Datei ablegen.
Das Deployment, Service und Route können erzeugt werden mit:
```
oc create -f Ingress_Apache.yaml
```

Um die Route anzulegen:
```
oc expose service apache --dry-run=client -o yaml >> Ingress_Apache.yaml >> Ingress_Apache.yaml
```

