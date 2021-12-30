Role Name
=========

This role creates containers using podman.

Requirements
------------

Required Collections
- containers.podman

Role Variables
--------------

## Container data/config locations. {{ Containername }}/config
ContainerData: /Guardian/Containers

Containers:
  - Gitea
  - Jackett
  - Transmission
  - Sonarr

#Linuxserver.io container vars
UserID: 101009 # abc user
GroupID: 101009 # serverio group
TimeZone: Pacific/Auckland

#Lancache vars
lancacheIP: "192.168.10.2"

#Pihole vars
PiholeIP: "192.168.10.6"

#Jellyfin vars
Youtubevids: "/mnt/Gamma/YoutubeVids"
Podcasts: "/mnt/Gamma/Podcasts"
Music: "/mnt/Gamma/Music"

#Sonarr vars
Anime: "/Guardian/Glusterfs/Anime"
Tvshows: "/nfs/Tvshows"

#Transmission vars
Transmission_User:
Transmission_Password:

#Gitea vars
Gitea_Password:


A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - snockow6.containers

License
-------

BSD
