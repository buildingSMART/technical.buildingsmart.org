ifcOWL
======

What is ifcOWL?
---------------

ifcOWL provides a Web Ontology Language (OWL) representation of the Industry Foundation Classes (IFC) schema. ifcOWL was an acadamic experiment that concluded that IFC is difficult to represent in other formats than EXPRESS. The IfcOWL is full of exceptions and particularities that make it hard to use in practise.

Semantic web enthousiast are advised to use the [bSDD](http://bsdd.buildingsmart.org/) that serves TTL for every URI and a GraphQL interface.


![](https://technical.buildingsmart.org/wp-content/uploads/2019/03/expressxsdowl-300x192-300x192.png)
-----------------------------------------------------------------------------------------------------------------------------

What is it good for?
--------------------

Using the ifcOWL ontology, one can represent building data using state of the art web technologies (semantic web and linked data technologies). IFC data thus becomes available in directed labelled graphs (RDF). This graph model and the underlying web technology stack allows building data to be easily linked to material data, GIS data, product manufacturer data, sensor data, classification schemas, social data, and so forth. The result is a web of linked building data that brings major opportunities for data management and exchange in the construction industry and beyond.

EXPRESS, IFC, LIST
------------------

The entire IFC EXPRESS schema (IFC entities and types and properties and so forth) is made available in one large ifcOWL ontology. In addition, the ifcOWL ontology uses some OWL classes and properties that are defined elsewhere. Namely, data types that are specific to EXPRESS (not to IFC) and to the representation of lists are defined in the following locations:

EXPRESS ontology: http://w3id.org/express#  
LIST ontology: http://w3id.org/list#

The ifcOWL ontology only imports the EXPRESS ontology. The EXPRESS ontology in turn imports the LIST ontology.

![](https://technical.buildingsmart.org/wp-content/uploads/2019/03/express_basics_1-127x300.png)

Conversion procedure
--------------------

The ifcOWL ontologies are generated directly from the IFC EXPRESS schemas. The recommended conversion procedure is entirely open and documented in an LDWG recommandation. The procedure follows the principles displayed in the below schema.

![](https://technical.buildingsmart.org/wp-content/uploads/2019/03/expresstoowl-300x245-300x245.png)

The above procedure is implemented in a number of tools:

[UGent – Aalto IFC-to-RDF converter](https://github.com/pipauwel/IFCtoRDF)  
[Walter Terkaj EXPRESS-to-OWL converter](http://www.terkaj.com/tools/ExpressToOwl/ExpressToOwl.zip)

These tools all result in the respective schema ontologies made available in the [IFC Schema Database](https://technical.buildingsmart.org/standards/ifc/ifc-schema-specifications/). For any further questions, please engage via the [buildingSMART International Forums](https://forums.buildingsmart.org/).

More information about ifcOWL can also be found at:
Pieter Pauwels and Walter Terkaj, EXPRESS to OWL for construction industry: towards a recommendable and usable ifcOWL ontology. Automation in Construction 63: 100-133 (2016). [http://dx.doi.org/10.1016/j.autcon.2015.12.003](http://dx.doi.org/10.1016/j.autcon.2015.12.003).
