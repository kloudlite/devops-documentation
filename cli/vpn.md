# Vpn

## Working with vpn

To access services of cluster and tunnel your local app to the server you need to connect to vpn. For that you can use the following commands.

```
sudo kl vpn start
sudo kl vpn stop
sudo kl vpn status
sudo kl vpn restart

# to tunnel traffic to your local you need to expose ports also
kl wg expose -p <server_port>:<local_port>
kl wg expose -p <server_port>:<local_port> -d    # provide -d flag to delete
```
