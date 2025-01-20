# Logs
> ## General Query Log
> ### Habilitar (MySQL 6.1+)
> ```bash
> SET global log_output = 'FILE';
> SET global general_log_file='/Applications/MAMP/logs/mysql_general.log';
> SET global general_log = 1; 
> ```