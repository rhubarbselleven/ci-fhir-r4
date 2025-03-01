The purpose of this profile is to provide a core representation of a procedure for the electronic exchange of health information between individuals, healthcare providers, and the My Health Record system infrastructure in Australia.

This profile identifies the additional constraints, extensions, and value sets that build on and extend [Procedure](http://hl7.org/fhir/R4/procedure.html) that are supported. 

This profile is designed to set a core Procedure standard for:
* Query for procedures performed for a patient
* Record or update a procedure performed for a patient

This profile is used by the following APIs:
* [insert API endpoint](StructureDefinition-TBD-1.html)


#### Profile specific guidance
- `Procedure.category` provides an efficient way of supporting system interactions, e.g. restricting searches. Implementers need to understand that data categorisation is somewhat subjective. The categorisation applied by the source may not align with a receiver’s expectations.
- In an exchange with the My Health Record system `Procedure.status` is "completed".
- The Procedure resource can represent a reason as a code with `Procedure.reasonCode`, or a reference with `Procedure.reasonReference` to a Condition or other resource.
  - Although both are marked as must support, sending systems are not required to support both a code and a reference, but they **SHALL** support *at least one* of these elements.
  - A receiving or persisting system **SHALL** support both elements.
- A procedure including an implantable device should use `Procedure.focalDevice` with a reference to a Device resource.


#### Boundaries and relationships
This profile is referenced by 
[ADHA Core Bundle](StructureDefinition-dh-bundle-core-1.html), 
[ADHA Event Summary Composition](StructureDefinition-dh-composition-es-1.html), 
[ADHA Event Summary Mixed Narrative and Structure](StructureDefinition-dh-composition-es-mix-1.html), 
[ADHA Shared Health Summary Composition](StructureDefinition-dh-composition-shs-1.html), 
[ADHA Core Encounter](StructureDefinition-dh-encounter-core-1.html), 
[ADHA Core Flag](StructureDefinition-dh-flag-core-1.html), and 
[ADHA Core Procedure](StructureDefinition-dh-procedure-core-1.html). 
