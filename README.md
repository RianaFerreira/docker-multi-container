React client
Api server express.js  
Database https://hub.docker.com/_/postgres/  
Background job management https://hub.docker.com/_/redis/  
Nginx request management https://hub.docker.com/_/nginx/  
Use default.conf in a custom image for Nginx to manage the routing of requests:
* api requests should be routed to the express server
* react app requests should be routed to the react server
