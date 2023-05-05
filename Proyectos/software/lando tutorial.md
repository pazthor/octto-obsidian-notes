
Actualmente lando es una capa( "envoltura" *wrapper*) entre docker compose y tu desarrollo, principalmente enfocado a reducir el onboarding de instalación que puede tener tu  


Actualmente  tengo un archivo  [[lando.yml]] como ejemplo donde pondre lo que he ocupado hasta el momento para una configuración de laravel.



## appserver
es el servicio donde se ubica tu app
si haces `lando info` aparece `appserver` seguido de  las configuraciones 


error de mysql 8, de tarda un chingo
https://github.com/lando/lando/issues/1462
issue-solución
https://github.com/lando/lando/issues/2948#issuecomment-1003484299


matar todos los contenedores  en lando
https://docs.lando.dev/help/purging-containers.html

[[Ejecutar Laravel en landon]]

### Fuentes a revisar:

https://agileadam.com/2021/05/setting-a-specific-external-port-for-mysql-in-lando/

https://docs.lando.dev/guides/external-access.html#locking-down-ports

https://docs.lando.dev/core/v3/services.html#supported-services

https://docs.lando.dev/core/v3/proxy.html

https://docs.lando.dev/core/v3/tooling.html