# example-config-as-code
Use a Github action to update a feature flag in a specific Split Environment. This is an example of using Split's Admin APIs to implement Configuration as Code (CaC)

Edit the file [flag_managed_by_github.json](flag_managed_by_github.json) and the flag definition will be updated. 

You can use the [YAML github action](.github/workflows/api_call_on_file_change.yml) in your own repository, or modify to suit your needs. 
