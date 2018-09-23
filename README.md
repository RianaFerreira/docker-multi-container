## Dependencies
Node.js and NPM `brew install node`
React client `npm install -g create-react-app`
Api server express.js  TODO: find this source

Database https://hub.docker.com/_/postgres/  
Background job management https://hub.docker.com/_/redis/  

Nginx request management https://hub.docker.com/_/nginx/  
Use default.conf in a custom image for Nginx to manage the routing of requests:
* api requests should be routed to the express server
* react app requests should be routed to the react server
