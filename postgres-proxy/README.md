# Postgres proxy

Say you have a Postgres running that can only be accessed from within a cluster, let's connect to it!

```bash
kubectl port-forward $(kubectl get pods -nportal --no-headers | grep "^postgres-proxy" | awk '{print $1}') 5433:5432 -nportal
```

Then open PgAdmin and connect to localhost.
