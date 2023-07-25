# Projeto_estudo_empresa_cassum

php
services:
  php: # Nome do serviço PHP
    image: php:7.4-apache
    container_name: meu-php-old
    ports:
      - "80:80"
      - "443:443"
    volumes:
      - /var/www/Projeto/projeto-tarefa-cassum:/var/www/html
    links:
      - db
