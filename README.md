# [mattiasohlsson/centos-blender-2.8-builder](https://hub.docker.com/r/mattiasohlsson/centos-blender-2.8-builder/)

## Usage

### Automatic build

    docker run --storage-opt size=20G mattiasohlsson/centos-blender-2.8-builder

### Automatic build (advanced)

    docker create --name blender-builder --storage-opt size=20G mattiasohlsson/centos-blender-2.8-builder

Repeat:

    docker start blender-builder
    docker logs --follow blender-builder

### Manual build

    docker run --storage-opt size=20G mattiasohlsson/centos-blender-2.8-builder bash

Use devtoolset-7.

    scl enable devtoolset-7 bash

Run /usr/bin/start or go to $HOME/blender-git/.
