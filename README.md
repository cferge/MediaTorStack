# MediaTorStack
My Media Stack used with Docker Compose
- Deployed via Portainer during Testing > Will test via CLI for deployment.
- Developed to help with my Learning of Docker-Compose as well as help with Restores of my Media Stack if I ever need it.


Apps Employed
- Sonarr (TV Shows)
- Radarr (Movies)
- Prowlarr (Search Daemon Mgmt)
- LazyLibrarian (EBook Mgmt)
- Plex (Media Server)
- Deluge (Downloader)
- Lidarr (Music)
- and More Possibly... 
- Using https://github.com/piscue/docker-backup-scripts to backup the Docker Environment


# Installing Chad's Docker "MediaTorStack" Deployment

- Fix/Update your Variables/Storage Path's in the .ENV File.

### An Explanation of how I'm setup
- Machine is an HP z230 SFF Workstation running Proxmox 7.x
- Virtual Machines are powered by QEMU/KVM (Proxmox)
- Storage is hosted on OpenMediaVault Virtual Machine
- 1x Single Virtual Machine hosts the Docker Container's for the MediaTorStack.
- Storage is connected to OpenMediaVault by backend connection to MediaTorStack VM via NFS.
- There are 2x main NFS Shares. /Media and /Torrents