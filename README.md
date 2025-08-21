# Triplestore selection

A repo used to select a viable triplestore solution

## Resources
 - Comprehensive lectures about triplestore/rdf/SPARQL: 
   - https://www.youtube.com/watch?v=fkUduxokEtE&list=PLoOmvuyo5UAeihlKcWpzVzB51rr014TwD&index=8&ab_channel=OpenHPITutorials
 - List of editors
   - https://rdfandsparql.com/blog/tpost/pbsx7g3ue1-whats-the-best-sparql-editor

## RDF
RDF is the framework that specifies how resources are described.
It's native format is xml, but a more common format is Turtle(ttl). This looks a lot like sparql

check namespaces on:
https://prefix.cc/

## Triple store

Stores data in triple form. S, P, O,

Also referred to as quad stores. In that case the triple is prefixed with a graph name.

**TBox** this is the part where the schema lives. Schema's are also expressed in RDF and can use other schemas like rdf, rdfs, owl, xs, etc 

**ABox** contains the data (or individuals) that conform to the TBox. Data in the ABox usually is of types defined in the TBox, but can actually be anything. The triple store follows the open world principle

## Sparql

Version 1.0 is the first final version of the spec and only supports querying data.
Version 1.1 adds complexer query methods and data manipulation

Sparql can can be accessed via an HTTP api endpoint

sparql clients:
   - https://www.npmjs.com/package/sparqljs
   - https://www.npmjs.com/package/sparql-http-client

## Questions
 - **How are namespaces resolved?**
   - Namespaces somtimes resolve to an actual turtle file