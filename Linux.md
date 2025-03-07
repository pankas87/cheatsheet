# Linux

> ## Servicios
> ### Gestionar
> ```bash
>    systemctl --type=service
> ```
> ## Usuarios
> ### Gestionar
> ```bash
>   # Crear usuario
>   adduser ${NOMBRE_USUARIO}
>   # Asignar rol sudo
>   usermod -aG sudo ${NOMBRE_USUARIO}
>   # Listar
>   cat /etc/passwd
>
>   # Listar, solo el nombre
>   # Comando cut: 
>   #   flag -d Separa cada línea del archivo en tokens delimitados por el caracter recibido a través de -d
>   #   flag -f Indica el número de token que extraemos
>   cut -d: -f1 /etc/passwd
> ```