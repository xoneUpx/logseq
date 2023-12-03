- cloud account via #github
	- configure [[argocd]] to fetch secrets from vault using dedicated plugin [link](https://argocd-vault-plugin.readthedocs.io/en/stable/) and maybe [link2](https://scribe.citizen4.eu/argocd-secret-management-with-argocd-vault-plugin-539f104aff05)
- consider using vault k8s operator
- policy for admin access:
  ``path "*" {
  capabilities = ["create", "read", "update", "delete", "list", "sudo"]
  }``