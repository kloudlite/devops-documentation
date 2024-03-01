# Installation

Here is the installation guide for `kl`, your go-to solution for accessing environments you've created in kloudlite.

This tool not only facilitates the setup of local environments but also assists in accessing hosted environments and intercepting applications within those environments.

### Prerequisites

Before proceeding with the installation, please ensure you have the following:

* Internet connection
* Terminal access (Linux/MacOS) or Command Prompt/PowerShell (Windows)

### Installation on Linux/MacOS

You can install Kloudlite CLI (`kl`) on Linux and MacOS using either `curl` or `wget`. Follow the instructions below based on your preference.

#### Using CURL

Open your terminal and execute the following command:

```sh
curl 'https://kl.kloudlite.io/kloudlite@v1.0.4-nightly?select=kl' | bash
```

#### Using Wget

If you prefer `wget`, use this command instead:

```sh
wget -qO- 'https://kl.kloudlite.io/kloudlite@v1.0.4-nightly?select=kl' | bash
```

#### Install Specific Version

To install a specific version of \[Your Tool Name], use the following command, replacing `v1.0.0` with the desired version number:

```sh
curl 'https://kl.kloudlite.io/kloudlite@v1.0.4-nightly?select=kl' | bash
```

### Installation on Windows

For Windows users, the installation process involves using PowerShell. Follow the steps below:

#### Install using PowerShell

Open PowerShell as Administrator and run the following command:

```powershell
iwr 'https://kl.kloudlite.io/kloudlite@v1.0.4-nightly?select=kl' | iex
```

### Post-Installation Steps

After successfully installing `kl`, you can start setting up and accessing your local and hosted environments. For detailed instructions on how to use `kl`, please refer to next sections.

### Troubleshooting

If you encounter any issues during the installation process, please consult our FAQ or Troubleshooting section. For further assistance, feel free to reach out to our support team.
