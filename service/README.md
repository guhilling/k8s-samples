# Mehrere Ressourcen als Ressource-Datei ablegen.
Das Deployment und der zugehörige Service können erzeugt werden mit:
```
oc create -f Resources_Apache.yaml
```

Um die Service-Beschreibung anzulegen:
```
oc expose deployment apache --port 8080 --dry-run=client -o yaml  >> Resources_Apache.yaml
```

