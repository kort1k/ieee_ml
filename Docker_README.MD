(Note that you need to do this well before coming to the workshop when you have data connection)

Section 1: Pulling the Docker Image
----------------------------------------------------------------------------------------------
If you are familiar with Docker, this is what you need
--------------------------------------------------------------------------
docker pull kgunnamieee/mlw


If you do not have Docker, please go through this
--------------------------------------------------------------------------------

Install with Docker on Windows:
*******************************

Download and install docker-ce from https://www.docker.com/
Direct link: https://store.docker.com/editions/community/docker-ce-desktop-windows






Install with Docker on Linux:
*****************************
Use command
	$ sudo apt-get install docker-ce
to get the latest version of docker-ce

More information at https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-ce-1

Add the docker group if it doesn't already exist:
sudo groupadd docker

To run docker command without sudo, you need to add your user (who has root privileges) to docker group. For this run following command:

 sudo usermod -aG docker $USER 


--------------------------------------------------------
For windows, you can run docker commands from Powershell or direct executable (Docker for Windows). In linux, you can open a terminal.

The following commands are the same from this point for Linux or Windows.
-----------------------------------------------------------------------------------------------------------

Steps to run the code

 Building the code

Once you pull the code from, build it using the command below:
docker build -t "mlw" -f Dockerfile .

or you can pull the docker image directly
docker pull kgunnamieee/mlw


Section II. Executing the code
----------------------------------------------------------------------------------------------------------------
To execute the code enter the following command

			docker run -p 8888:8888 -p 6006:6006 -p 6064:6064 mlw 


Now, open the following link

			http://localhost:8888/

Inside the jupyter server, open each notebook and use the commands in jupyter to execute the code



Section III. Debug mode
----------------------------------------------------------------------------------------------------------------

To enter the debug mode uncomment the debug part in each file and follow the instructions given there. 

To open the debugger go to the following link,

			http://localhost:6006/

---
command line:
open a separate terminal from host and type "docker ps "
You will get the following output

CONTAINER ID        IMAGE                               COMMAND     CREATED             STATUS              PORTS NAME               
xxxxxxxxxxxxxx        mlw                                 "/mlw/start.sh"
('container_id')
Then do
docker exec -it "container_id"  bash
to attach new bash shell to the same container






