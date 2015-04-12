# cljs experiments

Example project using [the boot build tool][boot] with the [boot-cljs],
[boot-cljs-repl], and [boot-reload] tasks.

## Prepare

[Install boot][installboot].  Then, in a terminal:

```bash
boot -u
```

This will update boot to the latest stable release version. Since boot is
pre-release software at the moment, you should do this frequently.

## Build

boot cljs -O advanced

Then load the index.html

## Develop

```bash
boot serve -d target/ watch speak cljs-repl cljs -sO none reload
```

There will be an nREPL server up, use a boot's or your ide's client and do

```clojure
(start-repl)
```

## TODO

  * Add dev and prod tasks
  * Extract Template
  * Add HTTP server to prod
  * Build an uberjar

## License

Copyright © 2014 Ricardo Gomez

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.

[boot]:             https://github.com/boot-clj/boot
[installboot]:      https://github.com/boot-clj/boot#install
