Industry Foundation Classes (IFC) - An Introduction
===================================================

What is IFC?
------------

In general, IFC, or "Industry Foundation Classes", is a standardized, digital description of the built environment, including buildings and civil infrastructure. It is an open, international standard ([ISO 16739-1:2018](https://www.iso.org/standard/70303.html)), meant to be vendor-neutral, or agnostic, and usable across a wide range of hardware devices, software platforms, and interfaces for many different use cases. The IFC schema specification is the primary technical deliverable of buildingSMART International to fulfill its goal to promote openBIM®.

More specifically, the IFC schema is a standardized data model that codifies, in a logical way...

...the **identity** and **semantics** (_name, machine-readable unique identifier, object type or function_)...

...the **characteristics** or **attributes** (_such as material, color, and thermal properties_)...

...and **relationships** (including locations, connections, and ownership)...

...of **objects** (like columns or slabs)...

...**abstract concepts** (performance, costing)...

...**processes** (installation, operations)...

...and **people** (owners, designers, contractors, suppliers, etc.).

The schema specification can describe how a facility or installation is used, how it is constructed, and how it is operated. IFC can define physical components of buildings, manufactured products, mechanical/electrical systems, as well as more abstract structural analysis models, energy analysis models, cost breakdowns, work schedules, and much, much more.

How is IFC used?
----------------

Today, IFC is typically used to exchange information from one party to another for a specific business transaction. For example, an architect may provide an owner with a model of a new facility design, an owner may send that building model to a contractor to request a bid, and a contractor may provide the owner an as-built model with details describing installed equipment and manufacturer information. IFC can also be used as a means of archiving project information, whether incrementally during the design, procurement, and construction phases, or as an "as-built" collection of information for long-term preservation and operations purposes.

The desired IFC data can be encoded in various formats, such as XML, JSON, and STEP (see _[Standards > Industry Foundation Classes (IFC) > IFC Formats](https://technical.buildingsmart.org/standards/ifc/ifc-formats/)_ ), and transmitted over web services, imported/exported in files, or managed in centralized or linked databases.

Software vendors of building information modeling tools - including model authoring, design, simulation and analysis, viewing and more - will provide interfaces to end users to export, import, and transmit data in some IFC format. It is up to users to decide what they want to share from their tools via IFC.

Who uses IFC?
-------------

Hundreds of software applications for use by many different stakeholders in the process can send and receive IFC data (see [_Community > Software Implementation_](https://technical.buildingsmart.org/community/software-implementations/) ). Since 1997, IFC has been tried and tested through many iterations, gaining worldwide trust as a means to deliver projects from all over the world.

License
-------

IFC is licensed under the Creative Commons Attribution-NoDerivatives 4.0 International License. To view a copy of this license, visit [http://creativecommons.org/licenses/by-nd/4.0/](http://creativecommons.org/licenses/by-nd/4.0/)
