# Media Server

The issue is that my NAS isn't able to run the Arr container services. So I am running them on my PC and mounting my PC to the NAS.

## Setup

Requirements:

- docker
- docker-compose

Most of the setup is based on the following guide:

<https://academy.pointtosource.com/containers/sonarr-radarr-prowlarr/>

1. Setup directories

Create the directories in the volumes of the docker-compose file.
In my case created a mount point for that to my NAS.

<https://sites.google.com/site/installationubuntu/qnap/qnap-nfs-shares-on-ubuntu?authuser=0>

This mount point is used in the docker-compose file.

2. Copy the '.env.example' file to '.env' and fill in the variables. Use the previous mount as the ROOT_DIR
3. Run `docker-compose up -d` to spin up the containers
4. Go to each of the services and configure them remember to make backups
