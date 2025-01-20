# Docker

> ## Contenedores
> ### Listar
> ```bash
>    docker ps -a
> ```
>
> ### Iniciar, detener, reiniciar
> ```bash
> docker start ${container-id}
> docker stop ${container-id}
> docker restart ${container-id}
> ```
>
> ## Networking - Redes
> ### Obtener dirección IP
> ```bash
> docker inspect ${container-id} | grep IPAddress
> ```
> ### Conexión Bash
> ```bash
> docker exec -it ${container-id} /bin/bash
> ```