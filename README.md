| No. | Command                                                                                        | Purpose                                                           |
| --- | ---------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| 1   | `sudo apt update`                                                                              | Updates the package list.                                         |
| 2   | `sudo apt upgrade -y`                                                                          | Upgrades all installed packages.                                  |
| 3   | `q`                                                                                            | Exit from the upgrade screen (if required).                       |
| 4   | `sudo apt install docker.io -y`                                                                | Installs Docker.                                                  |
| 5   | `sudo systemctl enable docker`                                                                 | Starts Docker automatically after every reboot.                   |
| 6   | `sudo systemctl status docker`                                                                 | Checks whether Docker service is running.                         |
| 7   | `docker --version`                                                                             | Displays installed Docker version.                                |
| 8   | `sudo usermod -aG docker $USER`                                                                | Adds your user to Docker group so `sudo` isn't needed every time. |
| 9   | `newgrp docker`                                                                                | Applies the new group immediately.                                |
| 10  | `docker pull nginx`                                                                            | Downloads the Nginx image from Docker Hub.                        |
| 11  | `docker images`                                                                                | Shows downloaded images.                                          |
| 12  | `cd webpages`                                                                                  | Moves into the webpages folder.                                   |
| 13  | `echo "Hi from CDAC" > index.html`                                                             | Creates a webpage.                                                |
| 14  | `cat index.html`                                                                               | Displays webpage contents.                                        |
| 15  | `cd ..`                                                                                        | Returns to parent directory.                                      |
| 16  | `docker run -d --name another-nginx -p 8080:80 -v $(pwd)/webpages:/usr/share/nginx/html nginx` | Runs an Nginx container and mounts your local folder into it.     |
| 17  | `docker ps`                                                                                    | Lists running containers.                                         |
| 18  | `nano index.html`                                                                              | Edits the webpage.                                                |
| 19  | `docker stop another-nginx`                                                                    | Stops the container.                                              |
| 20  | `cd ..`                                                                                        | Go back one directory.                                            |

