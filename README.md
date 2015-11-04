# cljsnode

Clojurescript based reference SPA on Heroku using node express, bootstrap,
reactjs/reagent and Kioo templates, demonstrating "isomorphic" clojurescript
shared between frontend and backend and Figwheel hotloading code changes
to both.

Check it out at https://cljsnode.herokuapp.com

Fork on github as a starting point for your own projects.
A goal is to turn this into a Leiningen template.

## Run Locally

To start a server on your own computer:

    lein do clean, deps, compile
    lein run

Point your browser to the displayed local port.
Click on the displayed text to refresh.

## Deploy to Heroku

To start a server on Heroku:

    heroku apps:create
    git push heroku master
    heroku open

This will open the site in your browser.

## Development Workflow

Start figwheel for interactive development with
automatic builds and code loading:

    lein figwheel app server

Wait until Figwheel is ready to connect, then
start a server in another terminal:

    lein run

Open the displayed URL in a browser.
Figwheel will push code changes to the app and server.

## License

Copyright © 2015 Terje Norderhaug

Based on an app concept by Marian Schubert.

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
