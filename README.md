# docker-commands

# SQL Server installation: 
1) ``docker pull mcr.microsoft.com/mssql/server``
2) ``docker run -d --name sql_server_name -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=YourPassword123' -p 1433:1433 microsoft/mssql-server-linux``

# Restoring the database from backup in MSSQL Server
1) Create a docker inside docker ``sudo docker exec -it dockerContainerName mkdir /var/opt/mssql/backup``
1) Copy the backup file to docker ``sudo docker cp yourfile.bak dockerContainerName:/var/opt/mssql/backup``
