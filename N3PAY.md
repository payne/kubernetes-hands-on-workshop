# Notes taken at KCDC.info 2025 and beyond

[Rob Richardson](https://github.com/robrich) is the workshop instructor.  Course makes no assumptions.   It's ok to move quickly through the docker parts or take your time there.  This repo is all of the courseware for today.

Three groups of info:
1. Docker
2. K8s
3. K8s in the cloud -- likely not getting there today, but it is in the courseware


Context -- docker is how we build containers, k8s is how we run them.

## Rob Richardson intresting involvements

1. [AZGive Camp](https://www.azgivecamp.org/) -- coding for charity
1. redgate -- community ambasador
1. Cy ambassador

## containers are
1. ephemeral (short-lived)
1. isomorphic (unchaging)
1. deterministic (same every time)

This makes them a good way for development & operation departments to communicate.

## Some follow along

1. `docker run -p <host_port>:<container_port> <image_name>`
1. docker container list --all 
1. docker container stop 6af
1. docker container

## Big commands
1. FROM - main command
2. COPY - main command
3. RUN - main command
4. ENV
5. CMD - main command

## hub.docker.com is a place to find images
1. Therre's a "Docker Official Image" that is node.  


## Docker is an ecosystem around container virtualization.  

# Tips
1. Changing the `Dockerfile` requires rebuilding the docker container before you run the new docker container.
1. Containers tools extension for VS Code is good.
1. `docker container rm -f abc` will stop and remove




