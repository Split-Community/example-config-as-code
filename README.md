# example-config-as-code
Use a Github action to update a feature flag in a specific Split Environment. This is an example of using Split's Admin APIs to implement Configuration as Code (CaC)

Edit the file [flag_managed_by_github.json](flag_managed_by_github.json) and the flag definition will be updated. 

You can use the [YAML github action](.github/workflows/api_call_on_file_change.yml) in your own repository, or modify to suit your needs. 

The YAML file uses the [Full update of flag definition in environment API](https://docs.split.io/reference/full-update-feature-flag-definition-in-environment)  to replace the existing feature flag definition with the one from the JSON file. 

The filename is used to define the name of the feature flag, and secrets are used for the Admin API Key, environment id and workspace ID. 

The flag definition can be refreshed using the [Get Feature Flag Definition in Environment](https://docs.split.io/reference/get-feature-flag-definition-in-environment) API to pull flags definitions down. 

## Flag definition
![image](https://github.com/Split-Community/example-config-as-code/assets/1207274/dbd86ec2-030d-4aa7-8046-840357ab4661)


## Targeting Rules updated
![image](https://github.com/Split-Community/example-config-as-code/assets/1207274/f1afd825-8db5-4542-858e-1c3782eabc75)
