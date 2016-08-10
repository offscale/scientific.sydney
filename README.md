# scientific.sydney-dist
Built with Hexo with the Phantom theme.

## Install deps

Node.JS (LTS or latest)

    npm i

## Run

    npm start

## Generate static files

    npm generate 

## Example nginx config

    server {
      server_name ~^(?<domain>.+)$;
      root /home/static/sites/$domain/public;
    
      access_log /var/log/nginx/$domain-static-access.log;
    
      error_log /var/log/nginx/static-error.log;
    }