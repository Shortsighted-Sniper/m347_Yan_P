
# KN01: Docker Grundlagen

## A) Installation

![](./images/A/Docker.png)

![](./images/A/website.png)

## B) Docker Command Line Interface

### Aufgabe 1

`docker -v`

![](./images/B/docker_version.png)

### Aufgabe 2

`docker search ubuntu` & `docker search nginx`

![](./images/B/search_ubuntu.png)

![](./images/B/search_nginx.png)

### Aufgabe 3

> run soll angeben, dass wir ein container starten möchten

> -d besagt, dass das container im hintergrund laufen sollte

> -p 80:80 besagt, setzte den host port 80 (das erste 80) auf port 80 im container (zweite zahl nach semicolon)

> docker/getting-started ist das image, dass wir laufen möchten

### Aufgabe 4

`docker pull nginx`

![](./images/B/docker_pull.png)

`docker create -p 8081:80 nginx:latest`

![](./images/B/docker_create.png)

`docker start <CONTAINER ID>`

![](./images/B/docker_start.png)

#### webpage

![](./images/B/homepage.png)

### Aufgabe 5

`docker run -d ubuntu`

![](./images/B/run_ubuntu.png)

### Aufgabe 6

![](./images/B/docker_exec.png)

### Aufgabe 7

`docker ps` & `docker ps -a`

![](./images/B/docker_ps.png)

### Aufgabe 8

`docker stop <CONTAINER NAME>`

![](./images/B/docker_stop.png)

### Aufgabe 9

`docker rm <CONTAINER ID>`

![](./images/B/docker_rm.png)

## C) Registry und Repository

![](./images/C/repo.png)

## D) Privates Repository

`docker tag nginx:latest arstneio/m347:nginx`

mit Tags können wir extra details an einem image geben. Es kann auch als differenzierung von Images helfen mit gleichem package name. es wird meistens für versionen von images bezeichtnet. Zum Beispiel ubuntu:latest oder ubuntu:18.04

`docker push Benutzername/reponame:nginx`

![](./images/D/docker_push.png)

Ich Pushe mein erstelltes image auf meinem Repo. Ich musste zuerst aber mich im docekr hub einloggen.

![](./images/D/mariadb.png)

![](./images/D/hub.png)
