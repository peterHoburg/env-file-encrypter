# env-file-encrypter

* config file
  * contains name of env var, type of fetcher. AWS Secrets, etc...
    * yaml
    * toml
* Metadata file
  * When the secret was grabbed last, for AWS Secrets we can check if a new secret value is needed
  * TTL for a secret
* Code to read the metadata + config file -> grab values and put them into an encrypted file
* Code to read the encrypted file and add it to docker/docker-compose/bash env var.
