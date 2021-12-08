# [Self hosted remote access gateway: Guacamole](https://www.youtube.com/watch?v=LWdxhZyHT_8&t=277s)
## Use to remote into proxmox server

- Say you've spun up lots of VMs

![](img/2021-12-08-15-29-23.png)

- typically you have these installed to help with remoting
  - VNC client
  - SSH client (putty)
  - Remote Desktop client

- Which is cool, until you move to another machine, which you have to set all of the above all over again

- Guacamole: a clientless remote desktop gateway.  Clientless meaning it uses standard protocols, RDP, VNC, SSH.  Which are already supported by Operating systems

![](img/2021-12-08-15-31-57.png)

- works in any browser with no plugins

## Setup using Docker, then Rancher
- Rancher: spins up Kubernetes, which then gives docker

1. go to github page to get docker image

![](img/2021-12-08-15-35-39.png)

2. take a look at Commands

![](img/2021-12-08-15-35-58.png)

3. Look at environment variable in parameters

![](img/2021-12-08-15-36-50.png)

4. Look at extensions

![](img/2021-12-08-15-37-31.png)

5. this enables authentication

### Lookup
- VNC client