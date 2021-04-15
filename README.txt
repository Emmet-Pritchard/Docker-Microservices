1. What is a docker container? [2]

Answer: A standard unit of software that packages code and
        its dependencies in order for the application to 
        run quickly and efficiently on multiple computing
        environments at the same time.

2. What is the difference between a container and a virtual machine? [2]

Answer: The main difference between these two is the fact that 
        virtual machines require an OS to run where containers
        do not need to include a guest OS in every instance.

3. What is the purpose of a Dockerfile? [2]

Answer: A dockerfile is a text document that contains all of the
        commands that a user could call on the command line in 
        order to assemble a docker image. 

4. What is the purpose of a requirements.txt file? [2]

Answer: A requirements.txt file is mainly used to describe the
        dependencies of the app, pinned to specific versions. 
        This can be generated and installed with pip.

5. What is the purpose of a docker-compose.yml file? [2]

Answer: A docker-compose.yml is a configuration file for docker-compose
        and it allows you to deploy, combine, and configure multiple
        docker-containers at the same time. 

6. What is the difference between a docker image and docker container? [2]

Answer: A docker-image is a set of files that has no state, whereas
        a docker-container is the instantiation of a docker-image.
        A container is a run-time instance of images. 

7. What command can be used to create an image from a Dockerfile? [2]

Answer: The docker build command builds Docker images from a dockerfile
        and a "context". A build's context is the set of files located
        in the specified PATH or URL.

8. What command will start a docker container? [2]

Answer: The docker run command first creates a writable container layer 
        over the specified image, and then starts it using the specified 
        command. That is, docker run. 

9. What command will stop a docker container? [2]

Answer: The command to stop one or more running containers is 
        docker stop [options] CONTAINER [CONTAINER...]. An example
        would be $ docker stop my_container.

10. What command will remove a docker container? Image? [5]

Answer: The command docker rm [OPTIONS] CONTAINER will remove one 
        or more containers.

11. What command will list all running docker containers? all containers? [5]

Answer: The command docker container ls is the default command which will list
        all running containers. To show all containers regardless of whether 
        or not they are running, add --all or -a as an option.

12. What command will list all docker images?

Answer: The command docker image ls is the default command which will list
        all non-intermediate images. To show all intermediate images simply
        add --all or -a as an option. 

13. What command do you use to deploy docker containers using information in the dockercompose.yml file? [2]

Answer: First make sure that you have a docker-compose.yml file in the project
        directory and make sure that the ports are exposed. Once you have that created, 
        from the project directory, start the application (deploy the container) by running
        the command docker-compose up.

14. How can you specify in the docker-compose.yml file that you want docker containers to use the
hosts network? [5]

Answer: Within the docker-compose.yml file, under build: if you add the network flag and 
        then you can specify the host. So for example it would look like this --
        build:
            network: host
        If you want to specify this outside of the build, you can use the code segment --
        network_mode: host

15. How can you specify in the docker-compose.yml file where the Dockerfile for a particular container
is found? [5]

Answer: Under build: we can include an option that is labeled dockerfile: with the name that 
        we want. For instance we can do something like--
        build:
           dockerfile: Dockerfile_name
        We can then access the Dockerfile_name within the container to get information on it.
