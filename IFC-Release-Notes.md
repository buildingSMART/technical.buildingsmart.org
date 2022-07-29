IFC Release Notes
=================

The following notes indicate the significant milestones and developments (revisions, additions, redactions) of the IFC schema release. The notes are order from most recent at the top to the oldest at the bottom, for quicker reference.

### IFC4.3 RC1 (4.3.rc.1)

The main purpose of IFC4.3 is to extend the IFC schema to cover the description of infrastructure constructions within the domains of Railways, Roads, Ports and Waterways including the elements that are common across those domains. The IFC4.3 schema has been developed to:

*   enhance the current definition of alignment and linear positioning to include railway cant within its geometric representation and span placements to provide “from-to” positioning;
*   enhance the current geometry definitions for advanced sweeps to add a sweep operation taking cant into account, and for advanced surfaces to represent road surfaces;
*   rationalize and enhance the definition of spatial structure to uniformly define a breakdown structure for all domains in question; and
*   rationalize and enhance the current specialization structure of products and product types to reflect the taxonomy of the new domains Railways, Roads, Ports and Waterways and common domains such as geotechnics and earthworks.

The extensions made to the IFC4.2 schema include in detail:

*   62 new occurrence entities (including corresponding type entities where indicated) have been created:
    *   24 proposed by the Shared Infrastructure domain, to support:
        *   the signalling occurrence and type entities (_IfcSign__\[Type\]_, _IfcSignal__\[Type\]_);
        *   the earthworks concepts (_IfcEarthworksCut_, _IfcEarthworksElement_, _IfcEarthworksFill_, _IfcReinforcedSoil_);
        *   the above-ground works occurrence and type entities (_IfcPavement__\[Type\]_, _IfcCourse__\[Type\]_, _IfcImpactProtectionDevice__\[Type\]_, _IfcPlant_);
        *   the geotechnical concepts (_IfcGeotechnicalAssembly_, _IfcGeotechnicalElement_, _IfcGeotechnicalStratum_, _IfcGeomodel_, _IfcGeoslice_, _IfcBorehole_, _IfcSolidStratum_, _IfcVoidStratum_, _IfcWaterStratum_).
    *   22 from the Railways domain to support:
        *   the spatial structure (_IfcRailway_);
        *   the geometric representation of alignment considering the railway cant (_IfcAlignment2DCant_, _IfcAlignment2DCantSegLine_, _IfcAlignment2DCantSegment_, _IfcAlignment2DCantSegTransition_, _IfcAlignment2DVerSegTransition_, _IfcAxisLateralInclination_, _IfcLinearAxisWithInclination_);
        *   the linear placement considering railway cant (_IfcLinearPlacementWithInclination_);
        *   the creation of swept area solid (_IfcDirectrixCurveSweptAreaSolid_, _IfcDirectrixDistanceSweptAreaSolid_, _IfcInclinedReferenceSweptAreaSolid_);
        *   the built element (track concepts) occurrence and type entities (_IfcRail\[Type\]_, _IfcTrackElement\[Type\]_);
        *   the distribution element occurrence and type entities (_IfcDistributionBoard\[Type\]_, _IfcElectricFlowTreatmentDevice\[Type\]_, _IfcMobileTelecommunicationsAppliance\[Type\]_).
    *   7 from the Roads domain to support:
        *   the spatial structure (_IfcRoad_);
        *   the creation of sectioned surfaces (_IfcSectionedSurface_);
        *   the creation of profile definitions using widths and slopes (_IfcOpenCrossProfileDef_);
        *   the association between a profile definition and its definition sources such as superelevation and width events (_IfcRelAssociatesProfileDef_);
        *   the placement entity (_IfcLinearSpanPlacement_);
        *   the built element type and occurrence entities (_IfcKerb\[Type\]_).
    *   9 from the Ports and Waterways domains to support:
        *   the spatial structure (_IfcMarineFacility_);
        *   Built element occurrence and type entities covering mooring (_IfcMooringDevice\[Type\]_), Navigation (_IfcNavigationElement\[Type\]_);
        *   Distribution element occurrence and type entities covering Conveyor Systems (_IfcConveyorSegment\[Type\]_) and Liquid transport systems (_IfcLiquidTerminal\[Type\]_).
    *   294 new predefined types have been created:
        *   68 by the Shared Infrastructure domain;
        *   121 by the Railway domain;
        *   39 by the Road domain;
        *   66 by the Ports and Waterways domains.
    *   40 items have been modified, generally only in their description.
    *   24 entities have been deprecated; the major ones are:
        *   _IfcBuildingElement_, replaced by _IfcBuiltElement;_
        *   _IfcCivilElement;_
        *   _IfcVibrationIsolator_, now contained in _IfcImpactProtectionDevice;_
        *   _IfcElectricDistributionBoard_, replaced with the generic _IfcDistributionBoard;_
        *   _IfcGeographicElementTypeEnum;_
        *   _IfcBridgePart_, now covered by _IfcFaciltyPart_ via an EXPRESS SELECT;
        *   _IfcBuildingSystem_, replaced by _IfcBuiltSystem;_
        *   _IfcVibrationDamper_, now contained in _IfcImpactProtectionDevice;_
        *   _IfcRelServicesBuildings;_
        *   _IfcBuildingElementProxy._

**NOTE:** The schema, as represented by the EXP and XSD files, is complete. The "RC1" version indication is due to final revisions/fixes being made to the HTML documentation.

* * *

### IFC4.2 (4.2.0.0)

The main purpose of IFC4.2 is to extend the IFC schema to include the description of bridge constructions. Extensions made to the IFC4.1 schema include:

*   The spatial structure was extended by _IfcFacility_ and _IfcFacilityPart_ as a basis to describe the spatial breakdown structure of infrastructure facilities.
*   _IfcBridge_ and _IfcBridge_ part were added to represent bridges and bridge parts.
*   Bridge elements have been integrated into a number of predefined types of building elements.
*   _IfcBearing_, _IfcDeepFoundation_, _IfcVibrationDamper_ and _IfcTendonConduit_ were added to represent the respective bridge elements.
*   _IfcRelPositions_ was added to better support positioning along the alignment.

* * *

### IFC4.1 (4.1.0.0)

The main purpose of IFC4.1 is to provide a basis for the various infrastructure domain extensions currently being developed (e.g. Rail, Road, Tunnel, Ports & Waterways). Extensions made to the IFC4 schema include:

*   Description of alignment as a combination of horizontal and vertical alignment
*   Linear Placement according to ISO 19148
*   IfcSectionedSolidHorizontal as a new geometry representation particular useful for describing infrastructure facilities

* * *

### IFC4 Add2 TC1 (4.0.2.1)

The main purpose of IFC4 Addendum 2 Technical Corrigendum 1 is to provide corrections and clarifications to the documentation of the schema and its constituent parts.

* * *

### IFC4 Add2 (4.0.2.0)

The main purposes of the IFC4 Addendum 2 are the improvement of the IFC4 Add 1 specification documentation and the necessary enhancements of the schema and property sets that resulted from the ongoing pilot implementations of the first two Model View Definitions, the Reference View and the Design Transfer View. The main change related to improvements to the tessellated geometry for the Reference View, and the advanced boundary representation geometry for the Design Transfer View. All changes made are downward compatible.

*   *   Two additional schema enhancements have been added after intensive discussions and considerations:
        *   new subtype of tessellated geometry enabling planar and polygonal boundaries with inner loops
        *   new elementary surfaces and intersection curves for more stable definitions of advanced b-rep's (NURBS)
    *   The documentation format has been further improved for readability. More interlinked definitions, now including property and quantity sets, ifcXML files for all examples, in addition to IFC files, etc.;
    *   The use of concept templates (chapter 4) improved, updated to Version 1.1 of the mvdXML specification and including the snippet of the mvdXML for each template;
    *   The use of concepts at relevant IFC Entities, including the snippets of the mvdXML specification for each concept root, optimized for documentation of the requested functionalities;
        *   NOTE This part is currently still experimental and focuses on documentation of concepts, it requires further improvements before being used for automatic IFC file validation purposes;
    *   A Change Log is provided in the HTML documentation

* * *

### IFC4 Add1 (4.0.1.0)

A minor update for IFC4 has been published taking into account the experiences and feedback from the pilot implementations and the first Model View definitions. Since 10.07.2015 the IFC4 Addendum 1 is a buildingSMART Final Standard and superseeds the IFC4 Final release.

The main purposes of the IFC4 Addendum 1 are the improvement of the specification documentation and the necessary enhancements of the schema that resulted from the pilot implementations and the first Model View definitions. All changes made are downward compatible.

*   *   The documentation format has been further improved for readability. A language independent section to describe the entities and types with their attributes and relationships is now available and separate to the EXPRESS and XSD code;
    *   The use of concept templates (chapter 4) and concepts is greatly enhanced, based on the mvdXML specification to enable better MVD developments and validation;
    *   Minor schema enhancements reflect the experience from pilot implementations of the IFC4 enhancements;
    *   One additional schema enhancement has been added after intensive discussions and considerations, a simplified and far more compact definition of poly lines with arc segments
        *   See the following »summary« of the rationale behind adding this additional geometry definition
    *   A Change Log is provided in the HTML documentation

* * *

### IFC4 (4.0.0.0)

Improvements made to the IFC schema include:

*   *   Full ISO standard (not a PAS)
    *   Enhanced capability of the IFC specification in its main architectural, building service and structural elements with new geometric, parametric and other features
    *   Enabled numerous new BIM workflows – including 4D and 5D model exchanges, manufacturer, product libraries, BIM to GIS interoperability, enhanced thermal simulations and sustainability assessments
    *   Linking all IFC property definitions to the buildingSMART data dictionary
    *   Improving readability and ease of access to the documentation with numerous implementation concepts and fully linked examples
    *   Containment of ifcXML4 schema, fully integrated into the IFC specification in addition to the EXPRESS schema
    *   Full integration with new mvdXML technology and allows easy definition of data validation services for IFC4 data submissions
    *   Correction of technical problems found since the release of the IFC2x3
    *   Enabling the extension of IFC to infrastructure and other parts of the built environment
    *   Multilingual translations of the schema

* * *

### IFC2x3 TC1 (2.3.0.1)

Since July 2007 the IFC2x release (as all previous releases of IFC) was superseded by the IFC2x3 Technical Corrigendum 1 - it is strongly recommended to download and use IFC2x3 Technical Corrigendum 1 from now on.

The purpose of this technical corrigendum was to correct several known minor technical problems found since the release of the IFC2x Edition 3 specification and to improve the documentation generally.

Technical corrections include the deletion, modification, or addition of a number of where rules in the EXPRESS schema. As well, a number of functions in the EXPRESS schema have been modified and a new one added. Several derived attributes have been removed from the EXPRESS schema because of ambiguity that could not be resolved satisfactorily.

The modification of the defined type _IfcCompoundPlaneAngleMeasure_ to allow optionally for the expression of angles to a fraction of a second is the only change of the EXPRESS schema that is reflected in the exchange file. This change therefore affects the specification (and existing software implementations) minimally but is an important first step in bringing the IFC and geospatial information specifications into alignment.

Clarifications were introduced to the accompanying documentation in a number of places. All these changes were made to realize the intent of the specification developers and to remove difficulties that implementers were having with data creation and validation. The IFC2x3 to IFC2x3 TC1 change log should be consulted for more details.

* * *

### IFC2x3 (2.3.0.0)

The IFC2x3 release was published in Feb 2006 as a successor of IFC2x2 Edition 2. It soon was established as the common ground of IFC implementations, combining previous IFC2x and IFC2x2 implementation threads. IFC2x3 was mainly a quality improvement release not adding scope but refinements on top of IFC2x2.

* * *

### IFC2x2 (2.2.0.0)

The initial IFC2x2 release was published in Mai 2003 as the first successor of the new IFC platform IFC2x. It introduced many extensions to better support the building service and structural domain, e.g. it contains the first IFC sub model for structural analysis, and many extensions for electrical, plumbing and building control definitions. Also the inclusion of 2D content within the model space of a BIM model (line, text, symbols) and presentation information (color, hatching, surface properties, like shading and rendering) are new in IFC2x2.

* * *

### IFC2x2 Add1 (2.2.1.0)

Issues with the initial IFC2x2 release were fixed within the IFC2x2 Addendum 1 release, published in July 2004. The required fixes led to an upward compatible schema change. The IFC2x2 Addendum 1 release was recommended for implementation and certification.

* * *

### IFC2x Add1 (2.1.1.0)

Issues with the initial IFC2x release were fixed within the IFC2x Addendum 1 release, published in Nov 2001. The required fixes led to an upward compatible schema change. The IFC2x Addendum 1 release was recommended for implementation and certification.

* * *

### IFC2x (2.1.0.0)

The initial IFC2x release was published in Nov 2000 as the first IFC platform release. It introduced the concept of a core model and domain extensions. It had been the first IFC release that got a broader implementation base and implementations had been certified using an earlier certification program.
