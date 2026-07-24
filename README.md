# Services_HomeLab
All of my services running on my home lab and the related documents to it.

## MEDIA SERVICES:
### Full ARR stack 
Running on docker using compose. All of the configurations and the file itself is included in this repo.

The stack is configured usnig the /data as the root folder and the structre as follows (neccessary for the jellyfin service to read and use the contents).

/data/
├── docker-compose.yml
├── media
│   ├── Games (Optional added as a tag in torrent whic directly reflects here)
│   ├── movies
│   │   └── Any movie downloaded by the torrent is added as folder here, and the contents are inside the folder.
│   ├── music
│   │   ├── Artist
│   │   │   └── Album(songs inside)
│   └── tv
│       └── Series folder with seasons as subfolder
│           ├── Season 1
├── monitor.log
└── torrents (Here every folder is linked to the media folder for content management which eleminated duplicate downloads, only references are present here.) 
    ├── movies
    ├── music
    ├── prowlarr
    └── tv
