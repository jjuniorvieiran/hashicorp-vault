# hashicorp-vault

## install 
- `brew update`
- `brew outdated`
- `brew tap hashicorp/tap`
- `brew install hashicorp/tap/vault`

## vault commands 
### start server
- `vault -v`
- `vault server -help`
- `vault server -dev`
- `export VAULT_ADDR='http://127.0.0.1:8200'`
- `export VAULT_TOKEN="hvs.6j4cuewowBGit65rheNoceI7”`
- `vault status`

### write/read/delete secrets
- `vault kv put -help`
- `vault kv put -mount=secret hello foo=world`
- `vault kv get secret/hello`
- `vault kv delete secret/hello`

### secret engines
- `vault secrets enable -path=kv kv`
- `vault secrets enable kv`
- `vault secrets list`
- `vault kv put kv/hello target=world`
- `vault kv get kv/hello`
- `vault kv put kv/my-secret value="s3c(eT"`
- `vault kv get kv/my-secret`
- `vault kv list kv/`
- `vault kv delete kv/my-secret`
- `vault secrets disable kv/`