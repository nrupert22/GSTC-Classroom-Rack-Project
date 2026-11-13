# "One command update scripts"


# (PVE Host) Opens other script in tmux
(For use in conjunction with other "PVE Host" script)  \
Opens other script in new tmux session.
```text
#!/bin/bash
tmux new-session -s pve-update './full-update-node.sh; bash'
  ```

# (PVE Host) Opens from other script, runs actual updates
(For use in conjunction with other "PVE Host" script)  \
Runs apt updates with timestamped logging, prompts the user about a potential reboot, and closes the tmux session after keypress.
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
Very simple apt only updater. :)
```text
#!/bin/bash
apt-get update
apt-get dist-upgrade -y
echo "Update complete, restart if needed!"
  ```

# Docker updater, updates ct/vm & docker containers
Updates apt and docker containers.
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
Updates via apt normally but changes directory to update docker containers.
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
