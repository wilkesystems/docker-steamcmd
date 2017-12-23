# Supported tags and respective `Dockerfile` links

-	[`artful` (*ubuntu/artful/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/ubuntu/artful/Dockerfile)
-	[`buster` (*debian/buster/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/debian/buster/Dockerfile)
-	[`buster-slim` (*debian/buster-slim/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/debian/buster-slim/Dockerfile)
-	[`centos6` (*centos/6/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/centos/6/Dockerfile)
-	[`centos7`, `centos` (*centos/7/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/centos/7/Dockerfile)
-	[`fedora24` (*fedora/24/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/fedora/24/Dockerfile)
-	[`fedora25` (*fedora/25/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/fedora/25/Dockerfile)
-	[`fedora26`, `fedora` (*fedora/26/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/fedora/26/Dockerfile)
-	[`jessie` (*debian/jessie/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/debian/jessie/Dockerfile)
-	[`jessie-slim` (*debian/jessie/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/debian/jessie-slim/Dockerfile)
-	[`opensuse42.1` (*opensuse/42.1/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/opensuse/42.1/Dockerfile)
-	[`opensuse42.2` (*opensuse/42.2/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/opensuse/42.2/Dockerfile)
-	[`opensuse42.3` `opensuse` (*opensuse/42.3/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/opensuse/42.3/Dockerfile)
-	[`stretch`, `debian` (*debian/stretch/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/debian/stretch/Dockerfile)
-	[`stretch-slim`, `mainline`, `latest` (*debian/stretch-slim/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/debian/stretch-slim/Dockerfile)
-	[`trusty` (*ubuntu/trusty/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/ubuntu/trusty/Dockerfile)
-	[`wheezy` (*debian/wheezy/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/debian/wheezy/Dockerfile)
-	[`wheezy-slim` (*debian/wheezy-slim/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/debian/wheezy-slim/Dockerfile)
-	[`xenial`, `ubuntu` (*ubuntu/xenial/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/ubuntu/xenial/Dockerfile)
-	[`zesty` (*ubuntu/zesty/Dockerfile*)](https://github.com/wilkesystems/docker-steamcmd/blob/master/ubuntu/zesty/Dockerfile)

----------------

# SteamCMD
![SteamCMD](https://github.com/wilkesystems/docker-steamcmd/raw/master/docs/logo.png)

The Steam Console Client or SteamCMD is a command-line version of the Steam client. Its primary use is to install and update various dedicated servers available on Steam using a command-line interface. It works with games that use the SteamPipe content system. All games have been migrated from the deprecated HLDSUpdateTool to SteamCMD.

----------------

# Get Image
[Docker hub](https://hub.docker.com/r/wilkesystems/steamcmd)

```bash
docker pull wilkesystems/steamcmd
```

----------------

# How to use this image

```bash
$ docker run -it wilkesystems/steamcmd
```

----------------

# Required Ports for Steam
Which ports do I need to open for Steam?

| To log into Steam and download content |
|----------------------------------------|
| HTTP (TCP port 80) and HTTPS (443)     |
| UDP 27015 through 27030                |
| TCP 27015 through 27030                |

| Steam Client                                                  |
|---------------------------------------------------------------|
| UDP 27000 to 27015 inclusive (Game client traffic)            |
| UDP 27015 to 27030 inclusive (Typically Matchmaking and HLTV) |
| UDP 27031 and 27036 (incoming, for In-Home Streaming)         |
| TCP 27036 and 27037 (incoming, for In-Home Streaming)         |
| UDP 4380                                                      |

| Dedicated or Listen Servers |
|-----------------------------|
|TCP 27015 (SRCDS Rcon port)  |

| Streamworks P2P Networking and Steam Voice Chat |
|-------------------------------------------------|
| UDP 3478 (Outbound)                             |
| UDP 4379 (Outbound)                             |
| UDP 4380 (Outbound)                             |

----------------

# Auto Builds

New images are automatically built by each new library push.

[![Docker build](https://dockeri.co/image/wilkesystems/steamcmd)](https://hub.docker.com/r/wilkesystems/steamcmd/)

----------------

# Package: steamcmd
Steam (http://www.steampowered.com) is a software content delivery system developed by Valve software (http://www.valvesoftware.com). There is some free software available, but for the most part the content delivered is non-free.

The Steam Console Client or SteamCMD is a command-line version of the Steam client. Its primary use is to install and update various dedicated servers available on Steam using a command-line interface.

This package comes with a fairly substantial non-free license agreement that must be accepted before installing the software.