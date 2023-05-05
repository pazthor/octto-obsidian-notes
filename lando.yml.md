```yml
name: laravel-project 
recipe: laravel  
config:  
  webroot: public  
  php: '8.1'  
  via: nginx  
  database: mysql  
  
# Landofile  
services:  
  database:  
    portforward: 3333 # fija el puerto  
  chromedriver: # For Laravel Dusk  
    type: compose  
    services:  
      image: robcherry/docker-chromedriver:latest  
      command: /usr/local/bin/supervisord -c /etc/supervisord.conf  
      expose:  
        - '4444'  
      environment:  
        CHROMEDRIVER_WHITELISTED_IPS: ""  
        CHROMEDRIVER_URL_BASE: "/wd/hub"  
      security_opt:  
        - seccomp:unconfined

```