## Kanban Application

This is a simple implementation of a Kanban Board, a tool that helps visualize and manage work.

Made of 3 separate Docker containers that holds and each docker file in kanban-app and kanban-ui folder

- PostgreSQL database
- Java backend (Spring Boot)
- Angular frontend


## Run the command below apply the kubernetes manifest file 
```bash
$ kubectl apply -f kanban-ui.yaml 

```
```bash
$ kubectl apply -f kanban-app.yaml 

```
```bash
$ kubectl apply -f postgres.yaml 

```
##

The entry point for a user is a website which is available under the address: **http://localhost:80/**

## Note: In a production environment we have implement 

* Secret mangement using tool liks hashicorp vault,aws secret manager or any secret management tool to secure database credentials

* Implementation of ingress for route base routing for application accessibility  in the  kubernetes cluster that a ingress controller


