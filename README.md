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

AWS EB delegates running of containers to ECS.
Task definitions instruct ECS how to run each of the containers.
https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definitions.html
https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definition_parameters.html

Dockerrun.aws.json configuration is based on this documentation
https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definition_parameters.html#container_definitions
