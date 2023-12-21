- delete finalizers:
  kubectl patch RESOURCE NAME -p '{"metadata":{"finalizers":[]}}' --type=merge
  
  or:
  kubectl patch configmap/mymap \
      --type json \
      --patch='[ { "op": "remove", "path": "/metadata/finalizers" } ]'