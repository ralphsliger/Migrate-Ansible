
##Building a simple LAMP stack and deploying Application using Ansible Playbooks.

These playbooks require Ansible 1.2.

These playbooks are meant to be a reference and starter's guide to building Ansible Playbooks. These playbooks were tested on CentOS 6.x so we recommend that you use CentOS or RHEL to test these modules.

This LAMP stack can be on a single node or multiple nodes. The inventory file 'hosts' defines the nodes in which the stacks should be configured.

    [webservers]
    localhost

    [dbservers]
    bensible
Here the webserver would be configured on the local host and the dbserver on a server called "bensible". The stack can be deployed using the following command:

    ansible-playbook -i hosts site.yml
Once done, you can check the results by browsing to http://localhost/index.php. You should see a simple test page and a list of databases retrieved from the database server.
 

##Iniciando con Ansible

Requisitos:
Para realizar las prácticas debes tener instalado en el equipo o servidor de pruebas:
-Docker
-Python
Instalación de Ansible desde afuera de la carpeta de tu proyecto solo este comando

    pip install ansible
Construcción de la imagen personalizada


En caso de reiniciar el experiemento ejecute:

    ./clean_all.sh
Ingresa a la carpeta 'ansible000' y sigue los pasos indicados.    

