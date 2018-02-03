# Necessary Docker Commands
* How docker works:

    ![](./images/how-docker-works.png)

* Docker workflow:

    ![](./images/docker-work-flow.png)

* To get a remote image and run it's bash:
    ```
    docker run -ti debian bash
    ```
    `docker run`: The docker command
    
    ```ti```: terminal interactive
    
    `debian`: name of the docker image

* To get all the docker images list:
    ```
    docker images
    ```
* To see all containers:
    ```
    docker ps -a
    ```
* To see the last stopped container
    ```
    docker ps -l
    ```
* To create an image from the existing container
    * `Long step`:
        * Get the container ID from the command
            ```
            docker ps -l
            ```
        * Build an image from there
            ```
            docker commit <container-id>
            ```
            This will return an image ID

        * Set a name for the image
            ```
            docker tag <image-id> your-image-name
            ```
    * `Short Step`:
        * Get the container ID
            ```
            docker ps -l
            ```
        * Build an image from the and name it at the same time
            ```
            docker commit <container-id> your-image-name
            ```
* Processes:


``Notes``:

* Every time we create a container from the image the container will be different from the other containers.
* To run the terminal interactively (if we want to use tabs for suggestions we can use `-ti`)

