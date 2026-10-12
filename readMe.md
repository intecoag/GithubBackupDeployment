# Setup
1. Git-Repo in /mnt/contain-store/stacks clonen auf Ziel-Server
2. .env.template zu .env kopieren und anpassen
3. Key bereitstellen unter key.pem
4. Aufstarten mit update.sh
5. Im Crontab update.sh einmal täglich ausführen lassen: aktualisiert das Image und das Repo
00 3 * * * cd /mnt/contain-store/stacks/GithubBackupDeployment && ./update.sh 1>/dev/null 2>/dev/null # Autoupdate GithubBackupDeployment