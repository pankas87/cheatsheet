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
>
> ## Grupos
> ### Gestionar
> ```bash
>    # Crear grupo
>    groupadd <nombre-de-grupo>
>    # Borrar grupo
>    groupdel <nombre-de-grupo>
> ```
>
> # SSH
> ```bash
>    # Generar clave SSH
>    ssh-keygen -t ed25519 -C "your_email@example.com"
> ```
>
## FFMPEG - Conversión de Videos
>
> ```bash
>   # Convertir MKV a MP4
>   ffmpeg -i input.mkv -codec copy output.mp4
>
>   # "Quemar" subtítulos en video
>   ffmpeg -i mymovie.mp4 -vf subtitles=subtitles.srt mysubtitledmovie.mp4
> ```