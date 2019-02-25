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
 
 
 **4.** 
 # APROVISIONAMIENTO BASE DE DATOS
 

 **5**
 # INTEGRACIÓN
 
 
 **6.**
 # REPOSITORIO GIT HUB=> https://github.com/santyfajardo/sd2019a-exam1.git
 
 
 **7.**
 # PROBLEMAS ENCONTRADOS Y SOLUCIONES IMPLEMENTADAS
 
 
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


 
