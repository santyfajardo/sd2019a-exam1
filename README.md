**1.**
# Examen 1

**Integrantes:** Santiago Fajardo, Sebastian Garcia y Marisol Giraldo

**Códigos:** A00328044, A00329796 y A00246380

**Emails:** santiago_fajardo96@hotmail.com, joan.garcia1@correo.icesi.edu.co y marisol.giraldo@correo.icesi.edu.co

**Curso:** Sistemas Distribuidos

**Tema:**  Automatización de Infraestructura

**Profesor:** Daniel Barragán

# OBJETIVOS:
- Realizar de forma autónoma el aprovisonamiento automático de Infraestructura.
- Diagnosticar y ejecutar de forma autónoma las acciones necesarias para lograr infraestucturas estables.

# TECNOLOGÍAS UTILIZADAS
- **Vagrant:** Vagrant es una herramienta gratuita de línea de comandos, disponible para Windows, MacOS X y GNU/Linux, que permite      generar entornos de desarrollo reproducibles y compartibles de forma muy sencilla. Para ello, Vagrant crea y configura máquinas  virtuales a partir de simples ficheros de configuración.
- **Ansible:** Es una plataforma de software libre para configurar y administrar computadoras.Combina instalación multi-nodo,   ejecuciones de tareas ad hoc y administración de configuraciones.
- **PostgreSQL:** Es un sistema de gestión de bases de datos relacional orientado a objetos y de código abierto.
- **Centos7:** Es un sistema operativo de código abierto, basado en la distribución Red Hat Enterprise Linux, operándose de manera      similar, y cuyo objetivo es ofrecer al usuario un software de "clase empresarial" gratuito. Se define como robusto, estable y fácil de   instalar y utilizar.

# DESCRIPCIÓN:
  Se desplegará una plataforma con cuatro máquinas virtuales con las siguientes funciones: CentOS7 Load Balancer, CentOS7 Webserver1,     CentosOS7 Webserver2 y CentOS7 Database. El repositorio tendrá un Vagranfile y el aprovisionamiento se realizará empleando la           herramienta Ansible de forma remota sobre las maquinas virtuales.
  El usuario desde la consola o navegador web realizará peticiones al balanceador CentOS7 Load Balancer, el cual deberá redireccionar     las peticiones entrantes hacia uno de los servidores web:CentOS7 Webserver 1 y CentOS7 Webserver 2, incluyendo un mensaje que indique   el servidor que responde la petición. Los servidores web, deberán realizar peticiones para obtener información almacenada en la base     de datos CentOS7 Database.
  
 **2.**
 # APROVISIONAMIENTO DEL BALANCEADOR DE CARGA
 
 
 **3.**
 # APROVISIONAMIENTO SERVIDORES WEB
 
 ![102](https://user-images.githubusercontent.com/35766585/53375358-06151c80-3929-11e9-8b99-23a261aaa54a.png)
 ![103](https://user-images.githubusercontent.com/35766585/53375384-1a591980-3929-11e9-8939-2ff338739ee1.png)

 
 **4.** 
 # APROVISIONAMIENTO BASE DE DATOS
 
 Para la base de datos se utilizo Postgresql un sistema de gestion de bases de datos relacional orientado a objetos. Para mayor informacion ingresar al archivo db-playbook.No obstante el archivo que nos importa realmente es el archimo main que podemos encontrar dentro de la carpeta task, que se encuentra dentro de las carpetas roles y createdb. En este archivo estan estipuladas las tareas que debe cumplir para crear la base de datos. Ademas existen unas tareas que se encargan de probar si la base de datos fue creada exitosamente y ademas si el usuario tiene acceso. 

 **5**
 # INTEGRACIÓN
 Para el tema de integracion utilizamos una branch especial llamada igualmente integration. De esta manera cada uno podia trabajar en ramas diferentes sin ser afectado por los demas compañeros. De este modo cada quien tiene la posibilidad de realizar su trabajo por separado para luego ser juntado en una sola rama llamada integration. Ademas activamos la opcion de que cada pullrequest necesita la aprovacion de uno de los integrantes de esta manera existe una barrera mas de proteccion. Pues sirve que en caso de que el archivo se encuentre dañado el compañero que revise pueda revisarlo antes de que se mezcle. 
 
 **6.**
 # REPOSITORIO GIT HUB=> https://github.com/santyfajardo/sd2019a-exam1.git
 
 
 **7.**
 # PROBLEMAS ENCONTRADOS Y SOLUCIONES IMPLEMENTADAS
  Al momento de realizar el aprovisionamiento de la base de datos tuvimos dificultades con el lenguaje, dado que las plantillas encontradas hacian referencia al sistema operativo ubuntu. Por lo que debiamos buscar su semejante para centos, dado que diferentes comandos no se ejecutaban.
 
 **8.**
 # REFERENCIAS BIBLIOGRÁFICAS
 
 - REPOSITORIO GITHUB URL: https://github.com/ICESI URL: https://github.com/ICESI-Training
 
 - Vagrant, la herramienta para crear entornos de desarrollo reproducibles 
   https://www.conasa.es/blog/vagrant-la-herramienta-para-crear-entornos-de-desarrollo-reproducibles/
 
 - Ansible
   https://www.ansible.com/
 
 - PostgreSQL
   https://www.postgresql.org/
   
 - How To Install and Use PostgreSQL on CentOS 7 
   https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-centos-7
   
-  How to Install and Configure Ansible on CentOS 7
   https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-ansible-on-centos-7


 
