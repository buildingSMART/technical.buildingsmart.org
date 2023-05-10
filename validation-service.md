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
