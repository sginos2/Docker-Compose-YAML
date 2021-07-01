# Docker-Compose-YAML

Docker build command:
docker build -t simpleuiapp:1.0 .

Docker run command:
docker run -d --rm --name diego -p 4000:4000 simpleuiapp:1.0

To deploy my stack/docker-compose.yaml file:
docker stack deploy -c docker-compose.yaml simpleuiapp-stack

To scale out my stack to 7 instances:
docker service scale simpleuiapp-stack_firstservice=5

To remove my stack and containers:
docker stack rm simpleuiapp-stack

To display in the browser:
localhost:4000
Or, after deploying the stacks:
localhost:3000
or
localhost:3001
