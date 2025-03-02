Volumens are persistent data stores for containers.

we attach a local storage to the containers virtual file system.
Data remain persistant as its not affected by the container.

* docker run -it -v <absolute_path_of_local_machine>:<conatiners_file> image

For docker compose 

    volume:
    - host_dir:cont_dir


- Named Volumes:
docker run -v VOL_NAME:CONT_DIR

- Ananymous Volume
docker run -v MOUNT_PATH

- Bind Mount
docker run -v HOST_DIR:COUNT_DIR

docker volume prune

remove all unwanted unused data. 