# hashicorp-vault

## install 
brew update
brew outdated
brew tap hashicorp/tap
brew install hashicorp/tap/vault

## vault command 
vault -v
vault server -help 
vault server -dev
export VAULT_ADDR='http://127.0.0.1:8200'				
export VAULT_TOKEN="hvs.6j4cuewowBGit65rheNoceI7”
vault status