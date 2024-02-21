# Environments

## Working with environments

We support multiple environments to work with. these commands will help you to import config,secrets as environment variables, mount and also ipmprting managed resources.

For more details visit [kl add](https://github.com/kloudlite/kl/blob/main/docs/kl/kl\_add.md).

```
kl use env
```

## working with configs, secrets, managed resources

```
# Adding
kl add config
kl add secret
kl add mres

# Add config to download at the time of load
kl add mount --configName=<config_name>
```
