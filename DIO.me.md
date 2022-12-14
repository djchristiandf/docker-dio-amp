# DIO.me
## A maior empresa para devs

[![N|Solid](https://hermes.digitalinnovation.one/tracks/48e9f018-f7c9-4f0f-b524-cd9223579626.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Descrição
Neste projeto o expert utilizou o Docker Compose para executar uma aplicação HTML em um Container Apache. Você poderá ir além e fazer alterações mais robustas ao seu projeto, estilizando sua página e utilizando seus conhecimentos em (HTML, CSS e JS). Você também pode buscar outras formas para executar seu arquivo HTML em outras Linguagens de Programação.

PASSO A PASSO:

Criar um arquivo YML com as definições de um servidor Apache (httpd); 
Especificar no arquivo YML o local onde os arquivos da aplicação estarão. A aplicação pode ser um simples Hello World. Será que você consegue executar uma aplicação web completa? 
Subir o arquivo YML e a aplicação para um repositório no GitHub. 
Agora é a sua vez de ser o protagonista! Implemente o desafio sugerido pelo expert e suba seu projeto para um repositório próprio, com isso, você aumentará ainda mais seu portfólio de projetos no GitHub!

Pré-requisitos:

Conhecimento Básico em Docker(Docker Compose);
Conhecimento Básico em Apache;
Conhecimento Básico em HTML;
Computador com SO de sua preferência(Windows, Linux, Mac OS);

# projeto utilizado como base
PHP 8 development environment with PHP-FPM, Nginx and MySQL, using Docker and Docker Compose
You need to have Docker and Docker Compose installed on your server to proceed using this PHP environment.

The following three separate service containers will be used:

An app service running PHP 8 FPM.
A db service running MySQL.
An nginx service that uses the app service to parse PHP code before serving the application to the final user.
Running the environment
Set the MySQL environment variables creating a .env file based on the .env.example file.

Build the app image with the following command:

docker-compose build app
When the build is finished, you can run the environment in background mode with:
docker-compose up -d
To show information about the state of your active services, run:
docker-compose ps
You can use the docker-compose exec command to execute commands in the service containers, such as an ls -l to show detailed information about files in the application directory:

docker-compose exec app ls -l
Now go to your browser and access your server’s domain name or IP address on port 8000: http://server_domain_or_IP:8000. In case you are running this demo on your local machine, use http://localhost:8000 to access the application from your browser.

You can use the logs command to check the logs generated by your services:

docker-compose logs nginx
If you want to pause your Docker Compose environment while keeping the state of all its services, run:
docker-compose pause
You can then resume your services with:
docker-compose unpause
To shut down your Docker Compose environment and remove all of its containers, networks, and volumes, run:
docker-compose down