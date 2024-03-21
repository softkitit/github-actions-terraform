<!-- markdownlint-disable -->
General terraform workflows to reuse in your projects, to initialize state, validate, plan, apply, and destroy infrastructure

## Workflows

| Name                                                                                | Description |
|-------------------------------------------------------------------------------------|-------------|
| [CI - Terraform Initialize State](#ci---terraform-initialize-state)                 | Lint, format and validate terraform code |




## CI - Terraform Initialize State

Initialize terraform state on remote backend and create PR with backend file configuration

### Usage

```yaml
```



### Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|----------|
| environment | Environment name deploy to | string | N/A | true |
| image | Docker Image to deploy | string | N/A | true |
| organization | Repository owner organization (ex. acme for repo acme/example) | string | N/A | true |
| repository | Repository name (ex. example for repo acme/example) | string | N/A | true |
| synchronously | Wait until ArgoCD successfully apply the changes | boolean | false | false |
| tag | Docker Image tag to deploy | string | N/A | true |



### Secrets

| Name | Description | Required |
|------|-------------|----------|
| github-private-actions-pat | Github PAT allow to pull private repos | true |






<!-- markdownlint-restore -->