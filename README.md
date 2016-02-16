# gervice

A golang service example.
The objective of this project is to offer a fast and simple way to create Restful APIs in GoLang using little code and some useful go libraries.

## Installing

1. Clone this repository somewhere.
1. In repository folder start the development server with:

  ```
  $ go get
  $ go get github.com/githubnemo/CompileDaemon
  $ CompileDaemon -command="./gervice"
  ```
1. You can access the sample URLs in your browser (or using some Restful Client):

  ```
  GET http://localhost:3333/param/anything  # prints the 'anything parameter'
  POST http://localhost:3333/pong           # validates an user name
  GET http://localhost:3333/me              # client that sends request to POST /pong
  GET http://localhost:3333/me2             # same than /me but in an Golang Object way
  GET http://localhost:3333/me3             # evolution of /me and /me2... the easiest and clearest way
  GET http://localhost:3333/ping            # changing a simple map and object for printing as JSON
  GET http://localhost:3333/migrate         # automatically create the User table in database
  GET http://localhost:3333/adduser         # adds an user to User table
  GET http://localhost:3333/where           # loads all User table entries in database.
  ```

## Features

1. Automatically re-compiles project when modifying any file of it.
1. Integrates with SQLite3 by default, so you can star developing and after that install your final database.
1. Using GORM to integrate to databases, well supported library and providing Migration for Database versioning.
1. Using Gin as web server and router.

## TODO

Here is the next features in our roadmap:

1. CORS
1. HTTPS (only)
1. Scaffold generator (like on Rails)
1. Auth using OAuth and JWT
