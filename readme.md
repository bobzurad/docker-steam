##Build
docker build -t bobzurad/steam .

##Run
open a bash in the image (changes will not be saved unless you commit!!!!)
docker run -t -i bobzurad/steam /bin/bash

##Steamcmd
TODO: use official ubuntu image
TODO: build a Dockerfile that contains all the instructions to install steamcmd and cs:source server
Follow instructions here to install steamcmd
https://developer.valvesoftware.com/wiki/SteamCMD

run steamcmd with:
sudo ./steamcmd.sh

start cssource server with:
./cssource/srcds_run -steam_dir steamcmd/ -steamcmd_script steamcmd/steamcmd.sh -console -game cstrike +map de_dust2 -maxplayers 20 -port 27015
