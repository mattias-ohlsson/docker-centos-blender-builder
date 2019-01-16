# [mattiasohlsson/centos-blender-builder](https://hub.docker.com/r/mattiasohlsson/centos-blender-builder/)

## Usage

### Automatic build

    docker run --storage-opt size=20G mattiasohlsson/centos-blender-builder

### Automatic build (advanced)

    docker create --name blender-builder --storage-opt size=20G mattiasohlsson/centos-blender-builder

Repeat:

    docker start blender-builder
    docker logs --follow blender-builder

### Manual build

    docker run -it --storage-opt size=20G mattiasohlsson/centos-blender-builder bash

Use devtoolset-7.

    scl enable devtoolset-7 bash

Run /usr/bin/start or go to $HOME/blender-git/.

## Source

[github.com/mattias-ohlsson/docker-centos-blender-builder](https://github.com/mattias-ohlsson/docker-centos-blender-builder)
