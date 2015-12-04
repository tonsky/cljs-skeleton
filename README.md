# Skeleton CLJS app

Has:

- http-kit server
- compojure router
- clojurescript app
- rum
- websocket endpoint
- transit serialization
- figwheel development server

Copy and modify for your needs.

## Dev setup

```sh
lein figwheel &
open http://localhost:8080/
```

This will watch, recompile and auto-reload CLJS app and CSS files.

## Prod setup

```sh
lein package
java -jar target/skeleton.jar &
open http://localhost:8080/
```

Here `lein package` is just an alias for `lein do cljsbuild once advanced, uberjar`.
