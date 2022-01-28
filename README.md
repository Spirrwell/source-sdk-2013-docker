# TL;DR
- git clone https://github.com/Spirrwell/source-sdk-2013-docker.git
- cd source-sdk-2013-docker/mp/src
- docker pull registry.gitlab.steamos.cloud/steamrt/scout/sdk/i386
- docker run --rm -it -v "$(pwd)/../":"$(pwd)/../" --user $(id -u):$(id -g) -w "$(pwd)" --name scout_i386 registry.gitlab.steamos.cloud/steamrt/scout/sdk/i386 /bin/bash
- ./creategameprojects
- make -f games.mak
