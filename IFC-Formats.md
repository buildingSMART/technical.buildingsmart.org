IFC Formats
===========

IFC may be encoded in various electronic formats, each having benefits and tradeoffs of software support, scalability, and readability. As building data can be quite large (i.e. gigabytes), the choice of format may have practical considerations.

Which do I use?
---------------

For the widest compatibility and smallest size for file-based import and export, STEP Physical File (SPF) is recommended. For web service communication, any of the above formats may be automatically negotiated by clients and servers.

[Edit](https://technical.buildingsmart.org/wp-admin/admin.php?page=tablepress&action=edit&table_id=5)

| Format | Extension | MIME Type | Text | Indexed | Size | Summary |
| --- | --- | --- | --- | --- | --- | --- | 
| **Official** |
| STEP Physical File (SPF)  | .ifc  | application/x-step  | Yes  | No  | 100%  | STEP Physical Format (SPF or IFC-SPF) is the most widely used format for IFC in practice, which is the most compact of the formats listed that can be read as text. IFC-SPF is based on the ISO standard for clear text representation of EXPRESS data models [ISO 10303-21](https://www.iso.org/standard/63141.html)  |
| Extensible Markup Language (XML)  | .ifcXML  | application/xml  | Yes | No | 113% | Extensible Markup Language (XML) provides enhanced readability and benefits from a broad range of software tools. ifcXML is based on the ISO standard for representation of STEP data in XML format [ISO 10303-28](https://www.iso.org/standard/40646.html) |
| ZIP  | .ifcZIP | application/zip | No | No | 17% | IFC data may embedded within a ZIP file. The embedded data may be encoded as either SPF or XML, where the resulting size is typically comparable. |
| Terse RDF Triple Language (Turtle) | .ttl based on [ifcOWL](https://technical.buildingsmart.org/standards/ifc/ifc-formats/ifcowl/) | text/turtle | Yes | No | 1372% | More info on: [ifcOWL](https://technical.buildingsmart.org/standards/ifc/ifc-formats/ifcowl/) | 
| Resource Description Framework (RDF/XML) | .rdf based on [ifcOWL](https://technical.buildingsmart.org/standards/ifc/ifc-formats/ifcowl/) | application/rdf+xml | Yes | No | 816% | More info on: [ifcOWL](https://technical.buildingsmart.org/standards/ifc/ifc-formats/ifcowl/) |
| **Provisional/Candidate** |
| JavaScript Object Notation (JSON) | .json | application/json | Yes | No | 148% | JSON provides enhanced readability and benefits from a broad range of software tools. |
| Hierarchical Data Format (HDF) | .hdf | application/x-hdf | No | Yes | n/a | HDF5 may store IFC data within hierarchical database, which provides high performance access to engineering data. HDF is based on the ISO standard for STEP data representation [ISO 10303-26](https://www.iso.org/standard/50029.html) |
| **Experimental/Unsupported** |
| SQLite | .sqlite | application/x-sqlite3 | No | Yes | n/a | SQLite may store IFC data within a relational database, which provides indexed access to data within large models and benefits from a broad range of software tools. |
