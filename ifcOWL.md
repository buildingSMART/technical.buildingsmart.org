What is IfcOWL?
---------------

Web Ontology Language (OWL) is a W3C standard for representing ontologies (formal, machine-readable models of concepts and relationships). It extends RDF (Resource Description Framework) with richer vocabulary and formal logic so software can infer new facts and check consistency. Both OWL and RDF are dedicated to information represented as subject–predicate–object “triples”, which together form a directed, labelled graph.

| **Schema language** | **Schema extension** | **Data language** | **Data extension** |
|---------------------|----------------------|-------------------|--------------------|
| XSD                 | .xsd                 | XML               | .xml               |
| JSON Schema         | .json                | JSON              | .json              |
| EXPRESS             | .exp                 | STEP              | .stp, .p21 (.ifc)  |
| OWL                 | .owl, .ttl           | RDF               | .ttl               |

The IFC Industry Foundation Classes (IFC) schema is primarily standardised as an EXPRESS schema for STEP (P21) representation of data, not necessarily a directed, labelled graph.

The _IfcOWL_ provides the OWL representation of the IFC schema. The _IfcOWL_ was an academic experiment that concluded that EXPRESS-based IFC is difficult to represent in formats other than EXPRESS. The _IfcOWL_ is full of exceptions and particularities that make it hard to use in practice.


What is IfcOWL good for?
--------------------

Using the IfcOWL ontology, one can represent building data using state-of-the-art web technologies (semantic web and linked data technologies). IFC data thus becomes available in directed labelled graphs (RDF). This graph model and the underlying web technology stack allow building data to be easily linked to material data, GIS data, product manufacturer data, sensor data, classification schemas, social data, and so forth. The result is a web of linked building data that brings major opportunities for data management and exchange in the construction industry and beyond.

EXPRESS, IFC, LIST
------------------

The IFC EXPRESS schema (IFC entities, types, properties, and so forth) is made available in one large _IfcOWL_ ontology. In addition, the IfcOWL ontology uses some OWL classes and properties that are defined elsewhere. Namely, data types that are specific to EXPRESS (not to IFC) and to the representation of lists are defined in the following locations:

EXPRESS ontology: http://w3id.org/express#  
LIST ontology: http://w3id.org/list#

The IfcOWL ontology only imports the EXPRESS ontology. The EXPRESS ontology, in turn, imports the LIST ontology.

![](https://technical.buildingsmart.org/wp-content/uploads/2019/03/express_basics_1-127x300.png)

IFC (EXPRESS) to IfcOWL conversion procedure
--------------------

The IfcOWL ontologies are generated directly from the IFC EXPRESS schemas. The recommended conversion procedure is entirely open and documented in an LDWG recommendation. The procedure follows the principles displayed in the schema below.

![](https://technical.buildingsmart.org/wp-content/uploads/2019/03/expresstoowl-300x245-300x245.png)

The above procedure is implemented in a number of tools:

[UGent – Aalto IFC-to-RDF converter](https://github.com/pipauwel/IFCtoRDF)  
[Walter Terkaj EXPRESS-to-OWL converter](http://www.terkaj.com/tools/ExpressToOwl/ExpressToOwl.zip)

These tools all result in the respective schema ontologies made available in the [IFC Schema Database](https://technical.buildingsmart.org/standards/ifc/ifc-schema-specifications/). For any further questions, please engage via the [buildingSMART International Forums](https://forums.buildingsmart.org/).

More information about IfcOWL can also be found at:
Pieter Pauwels and Walter Terkaj, EXPRESS to OWL for the construction industry: towards a recommendable and usable IFCOWL ontology. Automation in Construction 63: 100-133 (2016). [http://dx.doi.org/10.1016/j.autcon.2015.12.003](http://dx.doi.org/10.1016/j.autcon.2015.12.003).

The IfcOWL representation of the IFC schema is officially published by buildingSMART for IFC versions from 2.3 to 4.0. 

bSDD supports the RDF/TTL 
----------------------

For those looking for RDF/TTL representation of IFC schema content, we recommend checking the [buildingSMART Data Dictionary (bSDD)](http://bsdd.buildingsmart.org/). The bSDD now serves content also in a TTL format, every definition has a URI, and data can be parsed both with the [REST API](https://app.swaggerhub.com/apis-docs/buildingSMART/Dictionaries/v1) and the [GraphQL interface](https://github.com/buildingSMART/bSDD/blob/master/Documentation/bSDD%20and%20GraphQL.md).

Make sure to use the correct MIME type "text/turtle", for example:
```
curl -X 'GET' \
  'https://api.bsdd.buildingsmart.org/api/Class/v1?Uri=https%3A%2F%2Fidentifier.buildingsmart.org%2Furi%2Fbuildingsmart%2Fifc%2F4.3%2Fclass%2FIfcWall' \
  -H 'accept: text/turtle'
```


----------------------------------------------------------------------------------------
Authored by: Leon van Berlo on 29th Jul 2022

Last modified: Artur Tomczak, 9th Dec 2025

(full version history on [GitHub](https://github.com/buildingSMART/technical.buildingsmart.org/blob/main/ifcOWL.md))
