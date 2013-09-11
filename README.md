# tutorial-client

This is a small exploration of mine to have a decent repl in a clojurescript and [Pedestal] (https://github.com/pedestal/pedestal) based app running in the browser


I copied the app from the tag 2.1.1 of the Pedestal tutorial.

I just created a new pedestal project (with the new 0.2.2 version of the toosl) and copied the code in it

## Usage

 - in the tutorial-service folder, `lein repl`, `start`
 - In the tutorial-client folder, `lein repl`, `start`, `(cljs-repl)`
 - in another terminl launch Chrome with the `--disable-web-security switch`
 - load the app (http://localhost:3000)
 - load the development aspect
 - in the repl type `(js/alert "hello !")` if the popup shows up, you have a working repl
 -from the start.cljs file copy and paste in the repl these two lines
   - `(ns debugging (:require [tutorial-client.start :as start]))`
   - `(get-in start/to-be-monitored-app [:app :state])`
   - this should show you the state of the currently running app
