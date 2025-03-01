The purpose of this profile is to define a representation of the service item claimed in a claim against the Medicare Benefits Schedule (MBS) or Department of Veterans' Affairs (DVA) for the electronic exchange of digital health information between individuals, healthcare providers, and the My Health Record system infrastructure in Australia.

This profile identifies the additional constraints, extensions, and value sets that build on and extend [ServiceRequest](http://hl7.org/fhir/R4/servicerequest.html) that are supported. 

This profile is designed to set a ServiceRequest standard for:
* Recording or updating a service item in an MBS or DVA claim (ExplanationOfBenefit) resource
* Reading a service item in an MBS or DVA claim (ExplanationOfBenefit) resource

Operations, including querying, on service items in MBS or DVA claims (ServiceRequest resource) are expected to be within the context of an ExplanationOfBenefit resource query.

This profile is used by the following APIs:
* [insert API endpoint](StructureDefinition-TBD-1.html)


#### Profile specific guidance
None.


#### Boundaries and relationships
This profile is referenced by 
[ADHA Record of Claim against MBS or DVA](StructureDefinition-dh-explanationofbenefit-medicare-mbs-1.html).
