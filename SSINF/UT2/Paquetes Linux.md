#### Repositorios de Paquetes
Normalmente hay una base de datos grande con todos los paquetes, que está replicada por todo el mundo.

___

#### Gestión de Paquetes
###### apt install
###### apt install --reinstall
En linux, cuando instalas un paquete, se añade ese paquete a una base de datos interna del gestor de paquetes (`apt`), con lo que se sabe que paquetes tienes instalados y qué version tienes. Además de descargar e instalar el paquete.

La flag `--reinstall` lo que hace es reconfigurar el paquete a la configuración por defecto.

###### apt remove --purge
Cuando desintalas un programa solo se elimina de la base de datos del paquetes. Por eso hace falta la flag `--purge`, que lo borra del disco duro. 

###### apt update
Cuando actualizas, se fija en el número de version y marca los paquetes para ser actualizados si hay una version superior disponible. Es decir, se actualizan los índices de la base de datos.

###### apt upgrade
Cuando mejoras, actualiza los paquetes que estén marcados. Aquí es donde se descargan las actualizaciones y se instalan.

