Mininmal clojurescript clj figwheel project to demonstrate "clojure" test runner not working in conjure 4.17, but does work in 4.16.

Start repl

`clj -M:cider`

For some reason `ConjurePiggieback (figwheel.main.api/repl-env "dev")` does not work and returns

```
; piggieback: (figwheel.main.api/repl-env "dev")
; (err) Syntax error (ClassNotFoundException) compiling at (REPL:1:29).
; (err) figwheel.main.api
```
So i instead start the browser and piggieback with:

`ConjureEval(do (require 'figwheel.main.api) (figwheel.main.api/start "dev"))`
