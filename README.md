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
* To see the last container
    ```
    docker ps -l
    ```

