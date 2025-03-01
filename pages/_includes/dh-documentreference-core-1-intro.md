The purpose of this profile is to provide a core representation of a document reference for the electronic exchange of health information between individuals, healthcare providers, and the My Health Record system infrastructure in Australia. This profile supports describing a generic document that is made available to a system and is used for documents that are not authored and assembled in FHIR e.g. documents whose form is an attachment.

This profile identifies the additional constraints, extensions, and value sets that build on and extend [DocumentReference](http://hl7.org/fhir/R4/documentreference.html) that are supported. 

Where a more specific DocumentReference profile is applicable, e.g. advance care plan , an implementation **SHALL** ensure the resource conforms to that specific profile.

This profile is designed to set a core DocumentReference standard for:
* Query for a generic document reference for a patient
* Record or update a generic document reference belonging to a patient

This profile is used by the following APIs:
* [insert API endpoint](StructureDefinition-TBD-1.html)


#### Profile specific guidance
None.


#### Boundaries and relationships
This profile is referenced by 
[ADHA Core Bundle](StructureDefinition-dh-bundle-core-1.html),
[ADHA Aged Care Transfer Summary Composition](StructureDefinition-dh-composition-acts-1.html),
[ADHA Continuity of Care Summary Composition](StructureDefinition-dh-composition-cocs-1.html),
[ADHA Discharge Summary Composition](StructureDefinition-dh-composition-ds-1.html), 
[ADHA Core Procedure](StructureDefinition-dh-procedure-core-1.html), and
[ADHA Core ServiceRequest](StructureDefinition-dh-servicerequest-core-1.html).

These profiles build on this profile ([ADHA Core DocumentReference](StructureDefinition-dh-documentreference-core-1.html)) to define specific document compositions:
* [ADHA Advance Care Planning Document DocumentReference](StructureDefinition-dh-documentreference-acp-1.html).
* [ADHA Diagnostic Report DocumentReference](StructureDefinition-dh-documentreference-dr-1.html).
