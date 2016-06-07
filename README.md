![Docker](https://github.frapsoft.com/top/docker.png)

# Docker Tutorial [![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=102)](https://github.com/ellerbrock/open-source-badge/) [![Gitter Chat](https://badges.gitter.im/frapsoft/frapsoft.svg)](https://gitter.im/frapsoft/frapsoft/)

## Installation

Download the [Docker Toolbox](https://www.docker.com/products/docker-toolbox).

Its **best practice** to run each service in his own Docker container. To orchestrate them we need [Docker Compose](https://docs.docker.com/compose/).

`docker-machine` for administration and configuration von Docker Machines

## Documentation

- [Awesome Docker](http://veggiemonk.github.io/awesome-docker/)
- [from Vagrant to Docker](http://blog.osteel.me/posts/2015/12/18/from-vagrant-to-docker-how-to-use-docker-for-local-web-development.html)
- [Docker Images Comparison](https://www.brianchristner.io/docker-image-base-os-size-comparison/)
- [Docker related Blog](https://labs.ctl.io/)

## Docker Images

Visit [Docker Hub](https://hub.docker.com/) for Docker Containers.

### Plain Linux

- `docker pull alpine` - [official Alpine](https://hub.docker.com/_/alpine/) | [Documentation](http://gliderlabs.viewdocs.io/docker-alpine/) | [apk](http://wiki.alpinelinux.org/wiki/Alpine_Linux_package_management#Update_the_Package_list) | [packages](https://pkgs.alpinelinux.org/packages)
- `docker pull busybox` - [official BusyBox](https://hub.docker.com/_/busybox/)
- `docker pull centos` - [CentOS](https://hub.docker.com/_/centos/)
- `docker pull debian` - [official Debian](https://hub.docker.com/_/debian/)
- `docker pull ubuntu` - [official Ubuntu](https://hub.docker.com/_/ubuntu/)

### LAMP / LEMP Stack

- `docker pull eboraas/apache` - [official Apache](https://hub.docker.com/r/eboraas/apache/)
- `docker pull nginx` - [official nginx](https://hub.docker.com/_/nginx/)
- `docker pull php` - [official PHP](https://hub.docker.com/_/php/)
- `docker pull mariadb` - [official MariaDB](https://hub.docker.com/_/mariadb/)
- `docker pull mysql` [official MySQL](https://hub.docker.com/_/mysql/)

#### PHP Applications

- `docker pull wordpress` - [official Wordpress](https://hub.docker.com/_/wordpress/)
- `docker pull piwik` - [official Piwik](https://hub.docker.com/_/piwik/)
- `docker pull phpmyadmin/phpmyadmin` - [phpmyadmin](https://hub.docker.com/r/phpmyadmin/phpmyadmin/)

### Node.js

- `docker pull node` - [official Node.js](https://hub.docker.com/_/node/)

#### Phusion Passenger

- `brew install passenger` - optimized Node.js Image

#### Flat File CMS

- `docker pull gugu/raneto` - [Raneto](https://hub.docker.com/r/gugu/raneto/)

#### Blog

- `docker pull ghost` - [official ghost](https://https://hub.docker.com/_/ghost/.docker.com/r/gugu/raneto/)

### NoSQL

- `docker pull mongo` - [official MongoDB](https://hub.docker.com/_/mongo/)
- `docker pull redis` - [official Redis](https://hub.docker.com/_/redis/)

### Penetration Testing

#### Attacking

- `docker pull kalilinux/kali-linux-docker` [official Kali Linux](https://hub.docker.com/r/kalilinux/kali-linux-docker/)
- `docker pull owasp/zap2docker-stable` - [official OWASP ZAP](https://github.com/zaproxy/zaproxy)

#### Vulnerable

- `docker pull opendns/security-ninjas` - [Security Ninjas](https://hub.docker.com/r/opendns/security-ninjas/)

### Continuous Integration Testing

- `docker pull jenkins` - [official Jenkins](https://hub.docker.com/_/jenkins/)

## Commands

I recommend reading the [Docker Cheat Sheet](https://github.com/wsargent/docker-cheat-sheet).

- `docker images` - list installed images
- `docker ps` - shows running containers
- `docker-machine active` - list active machines
- `docker-machine ip default` - get the IP from the default container

## Examples

### Start Apache with http(s) and map htdocs folder

`docker run -p 80:80 -p 443:443 -v /Volumes/Daten/Daten/Programmierung/coding/docker/data/htdocs:/var/www/html/ -d eboraas/apache`

### Start Kali Linux with interactive bash Shell

```
docker pull kalilinux/kali-linux-docker
docker run -t -i kalilinux/kali-linux-docker /bin/bash
```

### Contact / Social Media

*Get the latest News about Web Development, Open Source, Tooling, Server & Security*

[![Twitter](https://github.frapsoft.com/social/twitter.png)](https://twitter.com/frapsoft/)
[![Facebook](https://github.frapsoft.com/social/facebook.png)](https://www.facebook.com/frapsoft/)
[![Google+](https://github.frapsoft.com/social/google-plus.png)](https://plus.google.com/116540931335841862774)
[![Gitter](https://github.frapsoft.com/social/gitter.png)](https://gitter.im/frapsoft/frapsoft/)
[![Github](https://github.frapsoft.com/social/github.png)](https://github.com/ellerbrock/)

### Development by 

Developer / Author: [Maik Ellerbrock](https://github.com/ellerbrock/)  
Company: [Frapsoft](https://github.com/frapsoft/)


### License 

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />

This work by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/ellerbrock/" property="cc:attributionName" rel="cc:attributionURL">Maik Ellerbrock</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.