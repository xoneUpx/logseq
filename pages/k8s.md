- delete finalizers:
  kubectl patch RESOURCE NAME -p '{"metadata":{"finalizers":[]}}' --type=merge