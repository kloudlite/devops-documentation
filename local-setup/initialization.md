# Initialization

## Preliminary Step: Selecting Your Account

Before you start initializing your project with `kl` and setting up the `kl.yml` configuration file, it's essential to ensure that you're operating within the correct Kloudlite account context.

#### Choosing the Correct Account

Open your terminal or command prompt and execute the following command to select the desired account:

```sh
kl use account
```

You will be prompted to choose an account from the list of accounts associated with your Kloudlite user. Select the appropriate account to set it as your current working context. This step ensures that all operations and configurations you perform are associated with the correct account.

## Initializing Your Project with `kl`

After setting the correct account context, you can proceed to initialize your project within the `kl` environment. Navigate to your project directory and create a `kl.yml` configuration file by executing:

```sh
kl init
```

This command prompts you to choose a project from your selected Kloudlite account. Once you make your selection, a `kl.yml` file will be automatically generated in your project directory

## Setting Up Your Environment

To fully configure your environment, you can use the following `kl` commands to add configurations, secrets, and managed resources (mres) to your project:

#### Adding Configurations

To add a configuration to your project, use:

```sh
kl add config
```

This command allows you to define and add configuration settings that are essential for your project's operation.

#### Adding Secrets

Manage sensitive information securely by adding secrets:

```sh
kl add secret
```

Secrets are securely stored and can be used within your project without exposing sensitive details in your codebase or `kl.yml` file.

#### Adding Managed Resources

To add managed resources (mres) that your project depends on:

```sh
kl add mres
```

Managed resources are external services or resources that your project utilizes, which can be configured directly from the command line.



## Reference

### Sample `kl.yml` File

Here's an example of what your `kl.yml` file might look like:

```yaml
version: v1
defaultenv: sample

project: demo-341290/samplep

mres:
  - name: auth-db
    env:
      - key: AUTH_DB_URI
        refkey: URI

configs:
  - name: environment
    env:
      - key: NODE
        refkey: NODE
        
secrets:
  - name: rds-connection
    env:
      - key: DB_URL
        refkey: RDS_URL
env:
  - key: SAMPLE_ENV
    value: sample_value
    
```

### Reference of kl.yml file

<table><thead><tr><th width="194">Field</th><th>Description</th></tr></thead><tbody><tr><td><strong>version</strong></td><td>Specifies the version of the YAML schema used.</td></tr><tr><td><strong>defaultenv</strong></td><td>The default environment for the project. Initially empty and set by the user.</td></tr><tr><td><strong>project</strong></td><td>A reference to the project within Kloudlite.</td></tr></tbody></table>

#### **Managed Resources (`mres`)**

<table><thead><tr><th width="187">Field</th><th>Description</th></tr></thead><tbody><tr><td><strong>mres[].name</strong></td><td>The name of the managed resource.</td></tr><tr><td><strong>mres[].env</strong></td><td>Specifies environment variables related to the managed resource.</td></tr><tr><td><strong>mres[].env.key</strong></td><td>The environment variable key.</td></tr><tr><td><strong>mres[].env.refkey</strong></td><td>The reference key within the managed resource, whose value is assigned to the environment variable.</td></tr></tbody></table>

#### **Configurations (`configs`)**

<table><thead><tr><th width="214">Field</th><th>Description</th></tr></thead><tbody><tr><td><strong>configs[].name</strong></td><td>The name of the configuration.</td></tr><tr><td><strong>configs[].env</strong></td><td>Configuration related environment variables.</td></tr><tr><td><strong>configs[].env.key</strong></td><td>The key for the environment variable.</td></tr><tr><td><strong>configs[].env.refkey</strong></td><td>The reference key within the configuration, used to populate the environment variable.</td></tr></tbody></table>

#### **Secrets (`secrets`)**

<table><thead><tr><th width="221">Field</th><th>Description</th></tr></thead><tbody><tr><td><strong>secrets[].name</strong></td><td>The name of the secret.</td></tr><tr><td><strong>secrets[].env</strong></td><td>Secret related environment variables.</td></tr><tr><td><strong>secrets[].env.key</strong></td><td>The key for the environment variable.</td></tr><tr><td><strong>secrets[].env.refkey</strong></td><td>The reference key within the secret, used to populate the environment variable.</td></tr></tbody></table>

#### **Environment Variables (`env`)**

<table><thead><tr><th width="173">Field</th><th>Description</th></tr></thead><tbody><tr><td><strong>env[].key</strong></td><td>The key for the environment variable.</td></tr><tr><td><strong>env[].value</strong></td><td>The value assigned to the environment variable.</td></tr></tbody></table>

\
