The buildingSMART Validation Service can be found on [validation.buildingsmart.org](https://validate.buildingsmart.org/).

### What is it?
The bSI Validation Service is a free, online platform for validating IFC files, developed by buildingSMART – with the help of software vendors and bSI projects.

### What does it do?
Given an IFC file, the Validation Service provides a judgment of conformity for such file against the IFC standard (schema and specification).

### What is being checked?
The IFC file is valid when it conforms to:
- **Syntax**. The STEP Physical File syntax
- **Schema**. The IFC schema referenced in the file including formal propositions encoded in the EXPRESS where rule and function language
- **Rules**. Other normative rules of the IFC specification (e.g. implementer agreements and informal propositions)
- **bSDD**. Does your IFC file contain references to the bSDD? The Validation Service can check if IFC's data match the referenced classification from bSDD

### What is not being cheked?
Outside of the constraints encoded in bSDD, the bSI Validation Service does not check project-specific, national-specific, organization-specific rules or constraints. Case-specific validation is where the mandate of the bSI Validation Service ends - and where other solutions like [IDS](https://technical.buildingsmart.org/projects/information-delivery-specification-ids/) can help.

### Support for software certification
When IFC files are checked by users through the Validation Service, metrics on the quality of these files are extracted. buildingSMART uses such metrics from IFC files to generate a report on the reliability and consistency of the producing software.

### Visualisation
For multiple reasons, geometric visualisation is not within the scope nor the mandate of the Validation Service. Many errors are invisible in a viewer or unrelated to a geometric representation or prevent visualisation altogether.

### Who can use the Validation Service?
The bSI Validation Service is designed to serve a broad range of users, including software developers, architects, engineers, consultants, and clients who need to validate and verify IFC files for various purposes. Keeping in mind the scope and the limits of the Validation Service's mandate, here are some examples.

- **Software developers** may use it to test and debug their IFC file export or import functions, and ensure that their software products can interoperate with other applications that use IFC files.
- **Architects & Engineers** may use it to verify that the IFC files they receive from different design disciplines conform to the IFC standard, and report any errors or warnings that may indicate non-compliance. This serves as enabler for further assessments of compliance with project requirements (out of scope for bSI Validation Service).
- **Consultants** may use it to review and audit the IFC files for quality assurance and quality control purposes, and provide feedback or recommendations to the design team or the project owner.
- **Clients** may use it to verify and validate that the IFC files they receive from the project stakeholders meet the IFC standard's constraints. And ensure that they can be used for further downstream purposes, such as data exchange, interoperability, or asset management.
