# Vpn

## Working with vpn

To access services of cluster and tunnel your local app to the server you need to connect to vpn. For that you can use the following commands.

```
sudo kl vpn start
sudo kl vpn stop
sudo kl vpn status
sudo kl vpn restart

# expose port of selected device
kl vpn expose port -p <port>:<your_local_port>

# delete exposed port of selected device
kl vpn expose port -d -p <port>:<your_local_port>
```
