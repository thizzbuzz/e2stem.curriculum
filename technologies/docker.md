* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 

## Docker

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

Docker makes it easier to collaboratively develop by creating an isolated environement for each project.

Linux operating systems are divided into two parts: the **kernel**, which is the core of the OS, and **user space**, which is everything outside the kernel (typically user-installed software). A container is an isolated user space instance that shares the kernel of the host system, unlike a virtual machine which includes its own kernel. 

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

🔷🔷🔷 **Docker**

#### Installation

Update and upgrade your system

`sudo apt-get update && sudo apt-get upgrade`

Download the install script:

`curl -fsSL https://get.docker.com -o get-docker.sh`

Execute the script using the command:

`sudo sh get-docker.sh`

Add the default Pi user to the docker group:

`sudo usermod -aG docker Pi`

And restart your computer...

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

🔷🔷🔷 **Docker-compose**

Install Python dependencies for Docker-compose:

`sudo apt-get install libffi-dev libssl-dev`
`sudo apt install python3-dev`
`sudo apt-get install -y python3 python3-pip`

Now install Docker-compose:

`sudo pip3 install docker-compose`

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

🔷🔷🔷 **Usage**

By default Docker-compose will look for a file called `docker-compose.yml` in the directory where you run this command:

`sudo docker-compose up`

Or if the compose file is called something else:

`sudo docker-compose -f <my-compose-file> up`

Certain changes like adding a new dependency will require you to rebuild your containers, in that case add the `--build` option flag:

`sudo docker-compose -f <my-compose-file> up --build`

That's it! When you want to bring the project down run:

`sudo docker-compose down`


