im-hateos
=========

A small static collection of json's to simulate a web chat front end.

The interaction is to follow CQRS principles,
that is, there are provided queries to view
and follow, and there are commands given that
can be executed.

The format of the JSON will follow something
similar to what [Siren][] proposes.
The `rel` option will not be provided at this
time.

Events will not follow the same verbose standards
as Siren asks for.

Names will be `snake_case`, although I wish
I could do `lisp-case` since it feels more
natural.

Start serving by running

    python -m SimpleHTTPServer

Then give your application the
http://localhost:8000/root.json


An additional parameter `_delay` is provided
in these event documents / objects.
You are expected delay your application by the
value in miliseconds before processing it and
events next in the sequence.


Due to the limitations of the python server,
`PUT` and `POST` operations do not exist.
Thus in the json files, `GET` is specified.
The responses are obviously static, but it can
be put as GET `?param=value` parameters.

[Siren]: https://github.com/kevinswiber/siren
