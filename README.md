src/foo.app.src was made with "rebar create-app"

Building
========
rebar get-deps
rebar compile
rebar ling-build-image # sends app to a hosted service that builds it into a LING Xen kernel image

Running
=======
The kernel can be booted by Xen locally:
$ xl create -c domain\_config
This will boot to an erlang shell, whence can be run:
\> foo:hello().
