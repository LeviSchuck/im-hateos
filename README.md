im-hateos
=========

A small static collection of json's to simulate a web chat front end.

The interaction is to follow CQRS principles,
that is, there are provided queries to view
and follow, and there are commands given that
can be executed.

The format of the JSON will follow something
similar to what [Siren][] proposes.

Start serving by running

    python -m SimpleHTTPServer

Then give your application the
http://localhost:8000/root.json


An additional parameter `_delay` is provided
in these documents.
You are expected delay your application by the
value in miliseconds before processing it and
events next in the sequence.

[Siren]: https://github.com/kevinswiber/siren
