# Setting up Environment

The `kl` tool simplifies the process of setting up your local development environment by allowing you to apply configurations, secrets, and managed resources with a single command structure. This enables you to run subcommands with environment variables (env\_vars) preloaded, streamlining the development and testing process.

### Subcommand with Preloaded Env\_Vars

To run a subcommand with environment variables loaded, you can use the following syntax:

```sh
kl -- <subcommand>
```

This command executes the specified `<subcommand>` with all relevant environment variables loaded, ensuring that your local environment mirrors the configurations of your project setup in `kl`. This is particularly useful for running local tests or development servers that rely on specific configurations and secrets.

### Sub Shell with Env\_Vars Loaded

For an even more integrated experience, `kl` provides the `kl shell` command, which opens a new subshell with all your project's environment variables preloaded. This allows you to work within a shell session that automatically includes all the necessary env\_vars for your project, simplifying the process of running applications, scripts, or commands that depend on those environment variables.

```sh
kl shell
```

Upon executing this command, you'll be placed into a new command line environment where all your `kl` project's configurations, secrets, and managed resource references are available as environment variables. This is ideal for developers who need a consistent and ready-to-use environment that closely matches the project's deployed or production settings.

### Advantages

* **Consistency**: Ensures that your local development environment matches the configurations and settings defined for your project, reducing discrepancies between development, testing, and production.
* **Security**: Allows you to work with sensitive information, such as secrets, without directly exposing them in your local environment or source code.
* **Efficiency**: Streamlines the process of setting up and switching between different project environments, making it easier to manage multiple projects or configurations.

By leveraging `kl` and its commands, you can significantly improve the workflow of setting up and managing your local development environment, ensuring that it aligns with your project's requirements and configurations with minimal effort.
