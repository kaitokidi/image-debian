# Debian images on Scaleway

[![Build Status](https://travis-ci.org/scaleway/image-debian.svg?branch=master)](https://travis-ci.org/scaleway/image-debian)

Scripts to build the official Debian images on Scaleway

These images are built using [Image Tools](https://github.com/scaleway/image-tools) and depends on the [armhf port of debian docker images](https://registry.hub.docker.com/u/armbuild/debian/).

<img src="http://upload.wikimedia.org/wikipedia/commons/4/4a/Debian-OpenLogo.svg" width="100px" />

---

**This image is meant to be used on a C1 server.**

We use the Docker's building system and convert it at the end to a disk image that will boot on real servers without Docker. Note that the image is still runnable as a Docker container for debug or for inheritance.

[More info](https://github.com/scaleway/image-tools#docker-based-builder)

## Available tags

Codename | Tags                       | Infos
---------|----------------------------|-------
wheezy   | **7**, **7.9**             | [![](https://badge.imagelayers.io/scaleway/debian:wheezy.svg)](https://imagelayers.io/?images=scaleway/debian:wheezy 'Get your own badge on imagelayers.io')
jessie   | **8**, **8.2**, **latest** | [![](https://badge.imagelayers.io/scaleway/debian:jessie.svg)](https://imagelayers.io/?images=scaleway/debian:jessie 'Get your own badge on imagelayers.io')
sid      | **sid**, **unstable**      | [![](https://badge.imagelayers.io/scaleway/debian:sid.svg)](https://imagelayers.io/?images=scaleway/debian:sid 'Get your own badge on imagelayers.io')

---

## Install

Build and write the image to `/dev/nbd1` (see [documentation](https://www.scaleway.com/docs/create_an_image_with_docker))

    $ make install

Full list of commands available at: [scaleway/image-tools](https://github.com/scaleway/image-tools/#commands)

---

## Links

- [Community: Official Debian Image](https://community.cloud.online.net/t/official-debian-image/344/11?u=manfred)
- [Community: New Linux Distributions on C1](https://community.cloud.online.net/t/official-new-linux-distributions-ubuntu-coreos-centos-fedora-arch-linux/229?u=manfred)
- [Image on Docker registry](https://registry.hub.docker.com/u/armbuild/scw-distrib-debian/)

---

A project by [![Scaleway](https://avatars1.githubusercontent.com/u/5185491?v=3&s=42)](https://www.scaleway.com/)

[[Back To Top]](#debian-images-on-scaleway)
