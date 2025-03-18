# Docker

> ## Contenedores
> ### Listar, Borrar
> ```bash
> docker ps -a
> docker rm ${CONTAINER_ID}
> # Borrar todos
> docker rm $(docker ps -a -q)
> ```
>
> ### Iniciar, Detener, Reiniciar
> ```bash
> docker start ${CONTAINER_ID}
> docker stop ${CONTAINER_ID}
> docker restart ${CONTAINER_ID}> 
> # Detener todos los containers
> docker stop $(docker ps -a -q)
> ```
>
> ## Imágenes
> # Listar, Borrar
> ```bash
> docker volume ls
> docker image rm ${IMAGE_ID}
> docker image prune --all # Elimina imágenes que no están asociadas a ningún container
> ```
>
> ## Volúmenes
> ### Listar, Borrar
> ```bash
> docker volume ls
> docker volume rm ${VOLUME_ID}
> docker volume prune --all # Elimina volúmenes que no están siendo usados
> ```
>
> ## Networking - Redes
> ### Obtener dirección IP
> ```bash
> docker inspect ${CONTAINER_ID} | grep IPAddress
> ```
> ### Conexión Bash
> ```bash
> docker exec -it ${CONTAINER_ID} /bin/bash
> ```