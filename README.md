CEDAR Archetype Instance Writer
===============================

Minimal Java project that uses [jsonschema2pojo](https://github.com/joelittlejohn/jsonschema2pojo) to generate Java classes 
that can write instances of CEDAR templates.

The ```./src/main/resources/json-schema``` directory contains an example JSON Schema-based CEDAR template.

The ```./src/main/resources/json``` directory contains an example JSON-based template instance corresponding to that template.

The main class ```org.metadatacenter.archetype.TemplateInstanceWriter``` contains an example of writing a template instance 
using a jsonschema2pojo-generated Java class.

#### Building and Running

To build this library you must have the following items installed:

+ [Java 11](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
+ A tool for checking out a [Git](http://git-scm.com/) repository.
+ Apache's [Maven](http://maven.apache.org/index.html).

First build the [CEDAR parent project](https://github.com/metadatacenter/cedar-parent).

Get a copy of the latest code:

    git clone https://github.com/metadatacenter/cedar-archetype-instance-writer.git

Change into the cedar-archetype-instance-writer directory:

    cd cedar-archetype-instance-writer 

Then build it with Maven:

    mvn clean install

To run:

    mvn exec:java

