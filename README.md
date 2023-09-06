# Cloudformation CLI

Comandos básicos de cloudformation cli

- aws cloudformation help
  
- aws configure

- aws configure --profile 'Name-User'

Crear un stack
- aws cloudformation create --stack-name prueba-cli --template-file "ruta-del-archivo"

Actualizar stack
- aws cloudformation update --stack-name prueba-cli --template-file "ruta-del-archivo"

Despliega stack (el que más utilizo)
- aws cloudformation deploy --stack-name prueba-cli --template-file "ruta-del-archivo"

Eliminar stack
- aws cloudformation delete-stack --stack-name 'Nombre-stack'

Descripción del stack
- aws cloudformation describe-stack
- aws cloudformation describe-stack-events --stack-name 'Nombre-stack'



## Instalación de jenkins

Validar los archivos instalados
- java --version
- jenkins --version

Revisar la credencial de login
- sudo su
- cat /var/lib/jenkins/secrets/initialAdminPassword

Link de apoyo
- https://www.jenkins.io/doc/book/installing/linux/


## Utilizando la imagen de docker jenkins 

Para ingresar al contenedor de docker
- sudo docker exec -it myjenkins /bin/bash

A fin de mostrar la credencial
- cat /var/jenkins_home/secrets/initialAdminPassword