# Node React Microservices app

implemented using docker and kubernetes

# Development process: -[Skaffold cli](https://skaffold.dev/)

- `skaffold`
  this will kickstart the entire application automatically

# Manual kickstart (docker and kubernetes must be installed & configured)(not recommended)

navigate to infra/k8s director and run following commands

- `kubectl apply -f posts-depl.yaml`
- `kubectl apply -f comments-depl.yaml`
- `kubectl apply -f query-depl.yaml`
- `kubectl apply -f event-bus-depl.yaml`
- `kubectl apply -f moderation-depl.yaml`
- `kubectl apply -f client-depl.yaml`
- `kubectl apply -f ingress-srv.yaml`

# Note: important configuration

# host file in your system

C:\Windows\System32\drivers\etc (depending on your OS)

update the 'hosts' file and add this

- `127.0.0.1 posts.com`

# Development Server

after running every command/configs mentioned above,
navigate to [Post_Microservice_App](http://posts.com)
