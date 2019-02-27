# dockerized-wordpress
> *Starts a Wordpress 5.1 project in a docker environment ready to use*.
  
![Wallpaper](https://user-images.githubusercontent.com/5404361/53292329-9f182c00-379f-11e9-9b19-f601ba5c5768.png)

## Features
Starts a completely clean installation of the WordPress (5.1) in a dockerized environment with MariaDB (10.4.2-bionic), PHP (7.2.1), Nginx (1.15.8) and PHP My Admin (4.7).

This project is ready to work with environment variables. The database access data of the Wordpress application is reported in the **.env** file at the project root, along with the environment variables of the containers.
  
## Steps to get started
1 - Make sure you have Docker and Docker Compose installed on your operating system. If you do not access the official documentation at https://docs.docker.com/install/ and install.

2 - Clone this repository with the command **`git clone git@github.com:vitorgiovane/dockerizedwordpress.git`** or **`git clone https://github.com/vitorgiovane/dockerizedwordpress.git`** in a terminal.

3 - Open the project root folder in a terminal and run the **`composer install`** command.

4 - Rename the **.env.example** file in the project root to **.env** and fill in the environment variables as you prefer. You can use the **.env.ready** file as the basis for populating these variables. This file has generic environment data but is able to start the environment quickly.

5 - Now is the time to start the containers. Open the project root in a terminal and run the **`sudo docker-compose up -d --build`** command.

> Note: The **--build** attribute builds the images and **-d** executes the containers in the background.
