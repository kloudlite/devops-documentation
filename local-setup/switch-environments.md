# Switch Environments

When working on projects with multiple development environments (e.g., feature/newfeature, staging, production), it's essential to switch between these environments seamlessly. The `kl` tool facilitates this with the `kl use env` command, allowing you to specify which environment's configurations, secrets, and managed resources should be active in your local development setup.

## `kl use env` Command

To switch to a different environment within your project, execute:

```sh
kl use env <environment_name>
```

Replace `<environment_name>` with the name of the environment you wish to switch to. This command updates your local context to use the configurations, secrets, and managed resources associated with the specified environment.

## Reloading Env\_vars

After switching environments using `kl use env`, you'll need to reload the environment variables to reflect the changes in your local development environment. To do this, you can execute the relevant `kl` commands that load these variables, such as:

* `kl -- <subcommand>`: Runs a specific subcommand with the newly loaded environment variables.
* `kl shell`: Opens a new subshell where all commands executed will have access to the updated environment variables.

### **Example Workflow**

1.  **Switch Environment**: Change to the staging environment with:

    ```sh
    kl use env staging
    ```
2.  **Reload Env\_Vars**: Open a new shell or run commands with updated environment variables:

    ```sh
    kl shell
    ```

    or

    ```sh
    kl -- <your_command_here>
    ```

This process ensures that your local development environment accurately reflects the configurations and settings of the selected environment, enabling you to test and develop under conditions that mimic your project's different deployment stages.

## Best Practices

* **Consistency**: Regularly use `kl use env` to ensure you're working in the correct environment, especially when switching tasks or projects.
* **Verification**: After switching environments, use `kl status` to verify that you're working with the intended settings.
* **Automation**: Integrate `kl` commands into your development scripts or toolchains to streamline the setup and switching process.

By following these steps and incorporating the `kl use env` command into your workflow, you can efficiently manage and switch between different project environments, keeping your local development aligned with your project's broader operational contexts.

\
