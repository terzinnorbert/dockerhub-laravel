# Docker and compose for Laravel development

## Usage

```
cd your-laravel-application
curl -LO https://raw.githubusercontent.com/terzinnorbert/dockerhub-laravel/master/docker-compose.yml
docker-compose up
```

The docker-compose contains the following services:  

* web - home of your laravel  
* database - mysql 5.7  
* smtp - mailcatcher for email testing  
* proxy  

## Proxy steps

The proxy uses the host machine's 80 port and resolves the VIRTUAL_HOST parameter.

Add the following line to /etc/hosts file:
```
127.0.0.1 laravel.docker
```