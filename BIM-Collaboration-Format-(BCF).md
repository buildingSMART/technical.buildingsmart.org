BIM Collaboration Format (BCF) - An Introduction
================================================

What is BCF?
------------

In general, the BIM Collaboration Format (BCF) allows different BIM applications to communicate model-based issues with each other by leveraging IFC models that have been previously shared among project collaborators. This can be done by utilizing a file exchange between software platforms or using a RESTful service that connects software platforms directly or to a dedicated 3rd-party BCF server acting as the hub for such communications.

More specifically, BCF works by transferring XML formatted data, which is contextualized information about an issue or problem directly referencing a view, captured via PNG and IFC coordinates, and elements of a BIM, as referenced via their IFC GUIDs, from one application to another.

The development of BCF started in 2009 and was originally conceived by two members of the buildingSMART International Implementation Support Group (ISG), Solibri and Tekla, along with the Institute for Applied Building Infomatics (iabi) at the Munich (Germany) University of Applied Sciences. Their desire to leverage open communication technology for IFC-based workflows led to prototyping, and eventually fully developing, BCF with other ISG members.

BCF is now a buildingSMART International openBIM standard, like IFC and the Data Dictionary (bSDD), open for all to use. Developers can find more information about supporting BCF in their products through the open GitHub repositories [here](https://github.com/buildingSMART/BCF-XML) and [here](https://github.com/buildingSMART/BCF-API).

There are two different ways to utilize BCF – via a [file-based exchange](https://github.com/buildingSMART/BCF-XML) or via a [web service](https://github.com/buildingSMART/BCF-API). The file-based exchange workflow is relatively straightforward and is a process most people are used to using. A BCF file (.bcfzip) is transferred from user to user, edited and returned. Unlike prescribed IFC file workflows, BCF files _can_ be “roundtripped”, as long as everyone maintains the integrity of the shared BCF file and multiple copies of it are not circulated. As an alternative to the file-based workflow, there is the web service-based (RESTful) API mode for BCF. This involves the implementation of a BCF server, with the option of also being the BIM server, that stores all the BCF data and enables project participants to sync the creation, editing, and management of BCF topics in one centralized location.

How is BCF used?
----------------

BCF was created for facilitating open communications and improving IFC-based openBIM processes by utilizing open standards (file formats & data communication protocols) to more readily identify and exchange model-based issues between BIM software tools, bypassing proprietary formats and workflows.

There are a number of use cases that can benefit from BCF-enabled workflows, where information can be derived from the BIM and connected back to the BIM for object-specific information. These cases include may include:

*   Design phase
    *   Documenting quality assurance / quality checking (QA/QC) items of BIMs
    *   Identifying design coordination (aka clash detection) issues between domain BIMs
    *   Annotating design options, object substitutions, and material selections
*   Procurement phase
    *   Bidding coordination items and clarifications
    *   Cost and supplier information for objects, assemblies, and/or systems
*   Construction phase
    *   Quality assurance / quality checking (QA/QC) records of installations vs. BIMs
    *   Tracking availability of items/materials and coordinating substitutions
    *   Collection of last-minute information for handover to owner/operator as part of the COBie deliverables
*   Operations phase
    *   Notations to handover models as changes are made to the facility and its many elements during occupation
    *   Owners notes about needed upgrades

Who supports BCF?
-----------------

A number of applications that support the import and export of IFC files, as well as standalone BCF services, support BCF in its file-based and/or REST-based form. Refer to the [Software Implementation Database](https://technical.buildingsmart.org/resources/software-implementations/) for applications that support the BCF XML and/or REST API implementations.

License
-------

BCF is licensed under the Creative Commons Attribution-NoDerivatives 4.0 International License. To view a copy of this license, visit [http://creativecommons.org/licenses/by-nd/4.0/](http://creativecommons.org/licenses/by-nd/4.0/)
