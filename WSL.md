# Windows Subsystem for Linux (WSL)

> ## Administración de Distribusiones
> ```bash
>    # Listar
>    wsl -l
>    # Instalar
>    wsl --install <distroName> 
>    # Desinstalar
>    wsl --unregister <distroName> 
> ```

> ## Interfaces de red
> ### Obtener dirección IP de instancia, desde host Windows
> ```bash
>    wsl -- ip -o -4 -json addr list eth0
> ```

> ## Docker
> ### Entregar permisos sobre el socket de Docker al grupo de usuarios docker
> ```bash
>    sudo addgroup --system docker
>    sudo adduser $USER docker
>    newgrp docker
>    # And something needs to be done so $USER always runs in group `docker` on the `Ubuntu` WSL
>    sudo chown root:docker /var/run/docker.sock
>    sudo chmod g+w /var/run/docker.sock
> ```