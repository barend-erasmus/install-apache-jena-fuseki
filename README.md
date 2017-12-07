# Install Apache Jena Fuseki

Fuseki is a SPARQL server. It provides REST-style SPARQL HTTP Update, SPARQL Query, and SPARQL Update using the SPARQL protocol over HTTP.


We need to start by updating the local server's apt package indexes.

`sudo apt-get update`

Next, we need to install Java.

`sudo apt-get install -y default-jdk`

Download the Apache Jena Fuseki tar and extract by running:

`sudo wget http://apache.saix.net/jena/binaries/apache-jena-fuseki-3.5.0.tar.gz`

and

`sudo tar xvzf apache-jena-fuseki-3.5.0.tar.gz`

Next, give the root user ownership of the `/opt` directory.

`sudo chown -R root /opt`

Create a directory for Apache Jena Fuseki and copy the extrated files to this directory.

`sudo mkdir /opt/apache-jena-fuseki-3.5.0`

`sudo cp -R apache-jena-fuseki-3.5.0 /opt`

Start Apache Jena Fuseki

`/opt/apache-jena-fuseki-3.5.0/fuseki start`

Browse `http://{ip-address}:3030`