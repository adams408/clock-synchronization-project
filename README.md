# Clock Synchronization Project
## Setup
[Install Docker](https://docs.docker.com/desktop/install/windows-install/)<br>
#### Clone the Repository:

    git clone git@github.com:adams408/clock-synchronization-project.git
## Run the Containers
Pull any images if necessary, and build the image. if changes are made to the dockerfile call this to rebuild the image.

    docker-compose build

Executes the docker-compose.yml to start all containers. include the -d flag to run in the background.

    docker-compose up -d
## Common Docker Commands
`docker-compose down`[^1]<br>
`docker ps`[^2]<br>
`docker inspect "CONTAINER NAME"`[^3]<br>
`docker exec -it "CONTAINER NAME" bash`[^4]<br>
`ping "IPADDRESS OF CONTAINER"`[^5]

[^1]: Stops running your containers. use if changes are made to the image.
[^2]: Will list currently running docker containers.
[^3]: Shows you the info of a particular container.
[^4]: Create an interactive bash shell inside the docker container.
[^5]: Show the containers can talk to one another.
