# Knowledge Area: Requirements Engineering

In SWEBOKv4, a software requirement is defined as "a condition or capability needed by a user to solve a problem or achieve an objective". Furthermore, it is "a condition or capability that must be met by a system, system component to satisfy a contract, standard, specification or other formally imposed document". Finally, the software requirement is "a documented representation or capability as in" the above two statements. 

The relevant aspects of above sentences are
- it is about conditions and capabilities,
- which MUST be described formally,
- in approriate representations (e.g. contract, document, spec, ...)

SWEBOKv4 includes a breakdown of topics for the software requirements knowledge area from fundamental and elicitation to analysis, sepcification and validation, and more. Regarding the use of Generative AI, focus should be on assistance in elicitation and requirements, as well as in the specification. 

## Practises

### Dinstinguish between categories of software requirements

* *Functional requirements* can be considered closer to e.g. Use Cases, with concrete description of inputs, prerequisites, usage pathways, outputs, pre- and postconditions, and more. When using GenAI to produce code, a likely approach is to go by use case (i.e. one after the other).
* *Nonfunctional requirements*  might be applicable to larger parts of or even the whole solution (e.g. Usability). AI needs to take nonfunctional requirements into account for many or even all use cases, so they have to be made available each time.
* *Constraints* such as technology and quality of service constraints have a significant impact on the codebase, since they cannot be easily changed afterwards.

Chapter 1-5/1.8 of SWEBOK introduces to the rationale of the above differentation: Requirements are analysed/specified/validated differently, depending on their category.

> Use different files and folders for each category. Use a file naming convention for different categories.

### Use a requirement specification template

There are different categorisation systems for nonfunctional requirements. Examples of this are

* [Volere Requirements Specification Template](https://www.volere.org/templates/volere-requirements-specification-template/)
* ...

> Use a requirements specification template

### Uniform pattern for use case specification

* [EAST (Easy Approach to Requirements Syntax)](https://alistairmavin.com/ears/)

> When specifying use cases, use a template with a semi-formal pattern, uniform across the solution.

### Describe technology constraints

> Constrain GenAI to your desired technology stack by explicitly formulating it.

### Capture language of the business domain

> Create a dictionary with basic description of all business entities that the solution needs to integrate or interact with. 

> If available, provide a domain model (e.g. UML or E/R). 

> If available when using DDD, provide a (C4) Model of Bounded Contexts.