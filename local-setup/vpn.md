# VPN Connection

For secure access to applications and managed resources within your environment directly from your local machine, `kl` offers functionality to manage VPN connections. This feature ensures that you can interact with your environment's resources as if they were part of your local network.

### Connecting to the VPN

To establish a VPN connection to your current environment, use the following command:

```sh
sudo kl vpn start
```

Running this command will initiate a VPN connection, granting you access to the applications and managed resources associated with the active environment in `kl`. This is crucial for testing, development, and access purposes, especially when dealing with resources not publicly accessible over the internet.

### Disconnecting from the VPN

When you no longer need direct access to your environment's internal resources, you can disconnect the VPN using:

```sh
sudo kl vpn stop
```

This command terminates the VPN connection, effectively isolating your local machine from the environment's internal network.
