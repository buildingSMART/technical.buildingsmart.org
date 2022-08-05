IFC Implementation Guides
=========================

This page lists recourses to help with the implementation of IFC. Please be aware some resources may be outdated.

Published Guidelines
--------------------

[**IFC2x Edition 3 Model Implementation Guide, Version 2.0**](https://standards.buildingsmart.org/documents/Implementation/IFC2x_Model_Implementation_Guide_V2-0b.pdf), _T. Liebich, 2009/05_ - This implementation guide is intended to provide a guidance for the first practical steps of implementing sections of the IFC2x3 schema, and as a reference to implementation agreements for commonly implemented parts of IFC.

[**Implementation Guideline for IFC Header Section, Version 1.0.2**](https://standards.buildingsmart.org/documents/Implementation/ImplementationGuide_IFCHeaderData_Version_1.0.2.pdf), _K. Häfele, A. Geiger, T. Liebich, 2008/05_ - The implementation reference to the official formatting of the header section of an IFC STEP (.ifc) file.

[**ifcXML (IFC2x3) Implementation Guide, Version 2.0**](https://standards.buildingsmart.org/documents/Implementation/ifcXML%20Implementation%20Guide%20v2-0.pdf), _N. Nisbet, T. Liebich, 2007/06_ - This document targets the XML community by providing guidelines on using and implementing the IFC standard using XML technologies. It is an extension to the existing IFC literature with focus on the specifics of the ifcXML specification compared to the standard EXPRESS based IFC model (as documented in the IFC object model specification and the IFC implementation guide).

[**ifcXML4 Specification Methodology, Version 1.1**](https://standards.buildingsmart.org/documents/Implementation/ifcXML4%20specification%20methodology%20V1-1.pdf), _T. Liebich, M. Weise, 2013/07_ - With the new development of the IFC4 standard, the XML equivalent to the EXPRESS based specification, called ifcXML, has undergone a complete redevelopment. The goal has been to simplify the corresponding XML schema, the ifcXML XSD, and to obtain smaller and more compact XML data files. The development has been executed under the codeword "simple ifcXML".

**[The EXPRESS Definition Language for IFC Development](https://standards.buildingsmart.org/documents/Implementation/The_EXPRESS_Definition_Language_for_IFC_Development.pdf)** - EXPRESS is a conceptual schema language which provides for the specification of classes belonging to a defined domain, the information or attributes pertaining to those classes (colour, size, shape etc.) and the constraints on those classes (unique, exclusive etc.). It is also used to define the relations which exist between classes and the numerical constraints applying to such relations.

Example files
-------------

[**The buildingSMART Github repo**](https://github.com/buildingSMART/Sample-Test-Files) \- Provides several example files.

**[The b-Cert platform](https://www.b-cert.org/)** - provides example files as part of the certification procedure.

**[Open IFC Model Repository](http://openifcmodel.cs.auckland.ac.nz/)** - provides an overview of publicly available IFC files.

Online Resources
----------------

**[IFC GUID](https://technical.buildingsmart.org/resources/ifcimplementationguidance/ifc-guid/)** \- Explanation to the IFC GUID specification for encoding and decoding of the IFC GUID

**[String Encoding & Decoding](https://technical.buildingsmart.org/resources/ifcimplementationguidance/string-encoding/) (for Multiple Language and Character Support)** - The IFC exchange format "STEP physical file" only allows characters represented by decimal value 32 to 126 from the code table in ISO 8859-1. Any other character, like some Western characters, like the German "Umlaut", Greek or Cyrillic letters, or Asian characters, has to be encoded before being exchanged as part of a string value.

[**Implementation Agreements**](https://standards.buildingsmart.org/documents/Implementation/IFC_Implementation_Agreements/) - Agreements by members of the Implementation and Model Support Groups to execute IFC support in specific ways given the inherent ambiguities of the broad IFC schema. The majority of these IAs are based on IFC2x3 implementation. All IFC2x3 IAs were reviewed and either full integrated into IFC4 documentation or declared irrelevant and not translated forward to IFC4 MVD implementations.
