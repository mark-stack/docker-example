# Laravel 9 + Docker
### A default Laravel 9 template containerized with Docker.

This is an instruction on how to **build** a new Laravel 9 project in Docker in around 15 mins - not to fork this one.

## Stack:
* Laravel 9
* MySQL
* Sail
* Docker

## Prerequisites (Windows installation):
* Windows 10 required build 21H2
* Docker for Windows
* WSL installed
* A Linux terminal such as Debian
* Visual studio with the “Remote development” extension installed.

## Create a new project:
1. Open Docker and wait for it to connect.
2. Open Debian
3. Debian: curl -s "https://laravel.build/docker-example?with=mysql,redis&devcontainer" | bash
4. Wait a little while to build
5. Debian: will be prompted for Linux password
6. Debian: cd docker-example
7. Debian: create an Alian for Sail commands with “alias sail='[ -f sail ] && bash sail || bash vendor/bin/sail'”
8. sail up
9. You’ll see the containers running in Docker
10. Open http://127.0.0.1:80 (port 80 is in docker-composer.yaml)


## Edit in Visual studio:
“Remote Development” extension is needed
Once you have a remote extension installed, go in Docker and the containers tab. On ‘docker-example’ that’s green, click the Visual Studio icon (“open in vscode”)
You can how edit the project kile normal. Any changes made will show when you refresh the browser.

## Start and stop container
Stop container: Debian: ctrl + c, or stop button in Docker
Restart: Start (play button) in Docker

## Misc Commands (in Debian):
alias sail='[ -f sail ] && bash sail || bash vendor/bin/sail'
Sail php artisan list

## Locate project folder:
Open debian
cd docker-example

## Git (adding to a new repo):
Create a new Github repository
Open a new Debian terminal
git init
git add .
git commit -m "first commit"
Git remote add origin <your repo url with .git at end>
git push --set-upstream origin master
Username: your Github username
Password: Your Github personal access token
The Master branch now has the code


[The deployed files are in the master branch](../tree/master)

