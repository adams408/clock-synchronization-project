# clock-synchronization-project

install docker

install the latest docker desktop

open powershell as administrator, execute this command: wsl --install // restart computer. now the docker daemon should be running.

open a command terminal to execute docker commands.

check for latest docker-compose version on your machine use: docker-compose --version

test: docker run -it ubuntu // will automatically pull down the ubuntu image from dockerhub and then run the linux machine and enter you into a bash shell. exit with "exit".

---

github clone: git clone git@github.com:adams408/clock-synchronization-project.git

run docker containers with docker-compose

docker-compose build // pull any images if necessary, build image.

docker-compose up -d // run containers in the background.

---

common docker commands

docker-compose build // if changes are made to the dockerfile call this to rebuild the image.

docker-compose up -d // executes the docker-compose.yml to start all containers. include the -d flag to run in the background.

docker-compose down // stops running your containers. use if changes made to the image.

docker ps // will list currently running docker containers.

docker exec -it "CONTAINER NAME" bash // create an interactive bash shell inside the docker container.

test: ping "IPAddress OF ANOTHER CONTAINER" // to show the containers can talk to one another.

docker inspect "CONTAINER NAME" // shows you the IP addresses assigned to a particular container.
