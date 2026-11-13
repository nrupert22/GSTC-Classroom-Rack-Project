# "One command update scripts"


# (PVE Host) Opens other script in tmux
```text
#!/bin/bash
tmux new-session -s pve-update './full-update-node.sh; bash'
  ```

# (PVE Host) Opens from other script, runs actual updates
```text
#!/bin/bash
#This updates the PVE node logging to a file.
date >> last-update-log.txt
apt-get update
apt-get dist-upgrade -y | tee -a last-update-log.txt
echo "Update complete, restart if needed!"
echo ""
read -n 1 -s -r -p "Press any key to continue"
tmux kill-session
  ```

# Basic updater
```text
#!/bin/bash
apt-get update
apt-get dist-upgrade -y
echo "Update complete, restart if needed!"
  ```

# Docker updater, updates ct/vm & docker containers
```text
#!/bin/bash
apt-get update
apt-get upgrade -y
docker compose down
docker compose pull
docker compose up -d
echo "Update complete, restart if needed!"
  ```

# Nextcloud updater, same as other but changes directory
```text
#!/bin/bash
apt-get update
apt-get upgrade -y
cd /opt/nextcloud
docker compose down
docker compose pull
docker compose up -d
cd ~
echo "Update complete, restart if needed!"
  ```
