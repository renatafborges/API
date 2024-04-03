<h1 align="center">
   <a href="#"> **UNDER CONSTRUCTION** </a>
   <a href="#"> APIS: CRUDS & AUTHENTICATION </a>
</h1>

<h3 align="center">
    This Projects follows what I learned about APIs in GoExpert classes with FullCycle
</h3>

<h4 align="center"> 
	 Status: Finished
</h4>

<p align="center"> 
 <a href="#how-it-works">How it works</a> • 
 <a href="#author">Author</a> • 

</p>

## How it works

- Diretories organization: following standands in https://github.com/golang-standards/project-layout

- api
  - swagger.yaml -> Swagger specs

- cmd
  - server/
    - docs -> API Documentation with swaggo (https://github.com/swaggo/swag)

- cmd
  - server
    - main.go -> The main applications for this project. Responsible for loading .env configurations, opening SQlite database connection, running migration for Product & User entities. Using Go Chi Router, I created the routes for Products and Users.

- configs
  - configs.go -> Default configs for project.

- internal
  - dto -> Dtos: CreateProductInput, CreateUserInput, GetJWTInput, GetJWTOutput.
  - entity -> Product & User entities and Unit tests.
  - infra
    -  database
    -  webserver 
  
---

This project is divided into one part:
1. Backend

### Pre-requisites

Before you begin, you will need to have the following tools installed on your machine:
[Git] (https://git-scm.com), 
[Golang] (https://go.dev/doc/install)
In addition, it is good to have an editor to work with the code like [VSCode] (https://code.visualstudio.com/)

#### Running Project

```bash

# Clone this repository
$ git clone https://github.com/renatafborges/Client-Server-API.git

# Access the project folder cmd/terminal
$ cd Client-Server-API

# go to the server folder
$ cd server

# in server folder run main.go
$ go run main.go

# The server will start at port: 8080 with the following message
Server is running on :8080

# open another terminal tab and access client folder
(to verify the current folder)
$ ls
(to move up a folder level)
$ cd ..
(access client folder)
$ cd client 

# in client folder run main.go
$ go run main.go

# The following message will appear at terminal in case of success
200
File created with success!

# in client folder the file will be created
cotacao.txt

# you may delete this file in case of another test
# you can use the extension SQLite Viewer and SQLite to access bid.sqlite database in server/bid.sqlite
```
## Author
Made with love by Renata Borges 👋🏽 [Get in Touch!](Https://www.linkedin.com/in/renataborgestech)
---
