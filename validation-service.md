The buildingSMART Validation Service can be found on [validation.buildingsmart.org](https://validate.buildingsmart.org/).

### What is it?
The IFC Validation Service is a free online platform for validating IFC files, developed by buildingSMART – with the help of software vendors and bSI projects.

### What does it do?
Given an IFC file, the Validation Service provides a judgment of conformity for such file against the IFC standard (schema and specification).

### What is being checked?

The IFC file is valid when it conforms to:
- **STEP Syntax**. The STEP Physical File syntax
- **IFC Schema**. An up-to-date (not withdrawn and latest revision) IFC schema referenced in the file, including formal propositions and functions encoded in the EXPRESS schema language
- **Normative IFC Rules**. Other normative rules of the IFC specification (e.g. implementer agreements and informal propositions)

Additionally, the Validation Service performs non-normative checks, including:
- **Industry Practices**. Checking the IFC file against common practice and sensible defaults. None of these checks render the IFC file invalid. Therefore, any issues identified result in warnings rather than errors
- **bSDD Compliance**. Checking whether references to classifications and properties from bSDD, found in an IFC file, comply with the source definitions in bSDD

### What is not being checked?
Outside of the constraints encoded in bSDD, the IFC Validation Service does not check project-specific, national-specific, organization-specific rules or constraints. Case-specific validation is where the mandate of the bSI Validation Service ends - and where other solutions like [IDS](https://technical.buildingsmart.org/projects/information-delivery-specification-ids/) can help.

### Support for software certification
When IFC files are checked by users through the Validation Service, metrics on the quality of these files are extracted. buildingSMART uses such metrics from IFC files to generate a report on the reliability and consistency of the producing software. Read more about this in the [buildingSMART International Software Certification Program](https://technical.buildingsmart.org/services/certification/).

### Visualisation
For multiple reasons, geometric visualisation is not within the scope or the mandate of the Validation Service. Many errors are invisible in a viewer or unrelated to a geometric representation or prevent visualisation altogether.

### Who can use the Validation Service?
The bSI Validation Service is designed to serve a broad range of users, including software developers, architects, engineers, consultants, and clients who need to validate and verify IFC files for various purposes. Keeping in mind the scope and the limits of the Validation Service's mandate, here are some examples.

- **Software developers** may use it to test and debug their IFC file export or import functions, and ensure that their software products can interoperate with other applications that use IFC files.
- **Architects & Engineers** may use it to verify that the IFC files they receive from different design disciplines conform to the IFC standard, and report any errors or warnings that may indicate non-compliance. This serves as enabler for further assessments of compliance with project requirements (out of scope for bSI Validation Service).
- **Consultants** may use it to review and audit the IFC files for quality assurance and quality control purposes, as well as provide feedback or recommendations to the design team or the project owner.
- **Clients** may use it to verify and validate that the IFC files they receive from the project stakeholders meet the IFC standard's constraints. And ensure that they can be used for further downstream purposes, such as data exchange, interoperability, or asset management.

### Recommended workflow
The IFC Validation Service aims to ensure IFC files adhere to the standard, irrespective of design intent specifics. For this reason, **it is most effective when applied at the outset of any IFC model validation process**. In this way, it serves as an enabler for all subsequent checks, ensuring that these can rely on a valid IFC data structure. 

![vs-workflow](https://github.com/buildingSMART/technical.buildingsmart.org/assets/62438551/5c66d189-7a17-4ff2-922f-4c1a4a1dc4f7)

While the IFC Validation Service alone is not sufficient to verify that IFC models meet all requirements, it serves as a base, complementary component to the overall validation procedure.
