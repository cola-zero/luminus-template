# Luminus-Template

A Leiningen template for projects using [Luminus](https://github.com/yogthos/luminus-template). 

The template initializes a base Luminus application.

## Installation

If you're using Leiningen 2 the template should work out of the box

If you're using Leiningen 1, you'll need to install the following plugins:

    lein plugin install lein-newnew 0.3.5
    lein plugin install luminus/lein-template 0.2.7


## Usage

Run the following command to create a new Luminus project:

    lein new luminus <your project name>

To build as standalone run:

```bash
lein uberjar
```
and you'll be able to run the resulting standalone jar as you would with any other executable Java jar:
```bash
java -jar target/myapp-0.1.0-SNAPSHOT-standalone.jar

2012-12-15 19:17:23.471:INFO:oejs.Server:jetty-7.x.y-SNAPSHOT
2012-12-15 19:17:23.512:INFO:oejs.AbstractConnector:Started SelectChannelConnector@0.0.0.0:8080
Server started on port [ 8080 ].
You can view the site at http://localhost:8080
```

To build a WAR run:
```bash
lein ring uberwar
```
Then you can deploy the resulting WAR to Tomcat or any other Java application server.

## License

Copyright © 2012 Yogthos

Distributed under the Eclipse Public License, the same as Clojure.
