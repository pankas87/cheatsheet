# Gestión de Usuarios y Permisos
> ## Crear usuario
>
> ## Otorgar y revocar permisos
> ```sql
>    -- Otorgar
>    GRANT SELECT, INSERT, DELETE, UPDATE ON Users TO 'Amit'@'localhost';
>    GRANT ALL PRIVILEGES ON `db`.* TO `user`@`localhost`;
>    -- Revocar
>    REVOKE ALL PRIVILEGES ON *.* FROM '<user_name>'@'localhost';
> ```

# Logs
> ## General Query Log
> ### Habilitar (MySQL 6.1+)
> ```bash
> SET global log_output = 'FILE';
> SET global general_log_file='/Applications/MAMP/logs/mysql_general.log';
> SET global general_log = 1; 
> ```

# Conexión
> ## Conexión con Certificado SSL
>
> ```bash
> mysql -u <user> -h <host> -P <port> --ssl=1 --ssl-ca=<path-to-cert> --ssl-verify-server-cert
> ```
>
>