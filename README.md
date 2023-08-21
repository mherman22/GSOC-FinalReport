## Add Support for FHIR PATCH operations
- Project Title: Add Support for FHIR PATCH operations
- Primary mentor:  Ian Bacher 
- Backup mentor:  Abert Namanya
- Project Link: https://wiki.openmrs.org/display/projects/GSoC+2023+%3A+FHIR%3A+Add+support+for+FHIR+PATCH+operations

## Overview
OpenMRS is using the FHIR API more and more in place of the REST API. However, the FHIR API is, by default, quite verbose. Supporting PATCH operations would allow us to support partial updates to FHIR resources without needing to send the whole resource from the client to the server.

The journey of enhancing OpenMRS through the addition of support for FHIR Patch Operations has been a remarkable experience. In light of the growing importance of the FHIR API as a replacement for the REST API, this project sought to introduce PATCH operations to enable more efficient partial updates to FHIR resources. This feature empowers users to modify specific elements within resources without the need to transmit entire resources between the client and the server.

In the context of the HAPI FHIR library, "patching" refers to the process of making partial updates to a FHIR (Fast Healthcare Interoperability Resources) resource. FHIR resources are representations of healthcare-related data, such as patient, observations, medications, etc., designed to be easily shared and exchanged between different healthcare systems.

Patching allows you to modify specific parts of a FHIR resource without having to replace the entire resource. This can be particularly useful when you want to make minor updates or corrections to a resource without sending the entire payload over the network. The PATCH operation follows the HTTP PATCH method semantics and is designed to be more efficient than the PUT or POST methods for updating resources, especially when dealing with large resources or slow network connections.

## Objectives:
- Implement JSON PATCH operations on all OpenMRS FHIR R4 resources and ensure to have the tests working perfectly. - COMPLETED ✅
- Implement JSON MERGE PATCH operations on all OpenMRS FHIR R4 resources and ensure to have the tests working perfectly. - COMPLETED ✅
- Implement XML PATCH operations on all OpenMRS FHIR R4 resources and ensure to have the tests working perfectly. - COMPLETED ✅

## Contributions:
During the project, I worked on various code repositories and pull requests to bring the functionality of PATCH operations to the FHIR API:

### Repositories: 
- https://github.com/openmrs/openmrs-module-fhir2
- https://github.com/openmrs/openmrs-contrib-fhir2-ig

### Pull Requests: 
- https://github.com/openmrs/openmrs-module-fhir2/pull/513
- https://github.com/openmrs/openmrs-module-fhir2/pull/489
- https://github.com/openmrs/openmrs-module-fhir2/pull/485
- https://github.com/openmrs/openmrs-module-fhir2/pull/483
- https://github.com/openmrs/openmrs-module-fhir2/pull/488
- https://github.com/openmrs/openmrs-module-fhir2/pull/490
- https://github.com/openmrs/openmrs-module-fhir2/pull/491
- https://github.com/openmrs/openmrs-module-fhir2/pull/484
- https://github.com/openmrs/openmrs-module-fhir2/pull/481
- https://github.com/openmrs/openmrs-module-fhir2/pull/487
- https://github.com/openmrs/openmrs-module-fhir2/pull/479
- https://github.com/openmrs/openmrs-module-fhir2/pull/480
- https://github.com/openmrs/openmrs-module-fhir2/pull/492
- https://github.com/openmrs/openmrs-module-fhir2/pull/493
- https://github.com/openmrs/openmrs-module-fhir2/pull/478
- https://github.com/openmrs/openmrs-module-fhir2/pull/499
- https://github.com/openmrs/openmrs-module-fhir2/pull/500
- https://github.com/openmrs/openmrs-module-fhir2/pull/501
- https://github.com/openmrs/openmrs-module-fhir2/pull/502
- https://github.com/openmrs/openmrs-module-fhir2/pull/503
- https://github.com/openmrs/openmrs-module-fhir2/pull/505
- https://github.com/openmrs/openmrs-module-fhir2/pull/507
- https://github.com/openmrs/openmrs-module-fhir2/pull/509
- https://github.com/openmrs/openmrs-module-fhir2/pull/513
- https://github.com/openmrs/openmrs-module-fhir2/pull/498
- https://github.com/openmrs/openmrs-module-fhir2/pull/495
- https://github.com/openmrs/openmrs-module-fhir2/pull/496
- https://github.com/openmrs/openmrs-module-fhir2/pull/497

### Found Issues:
- Medication Dispense was not added to the landing page of the FhirIG
- Medication was not added to the landing page of the FhirIG

### Fixed Issues:
- https://github.com/openmrs/openmrs-contrib-fhir2-ig/pull/59
- https://github.com/openmrs/openmrs-contrib-fhir2-ig/pull/60
  Any other work

### Other related work:
During this GSoC jouney, i was able to do other work on the FHIR module as asigned by my mentor and below are the pull requests;-
- FM2-606: Mapping ContactPoints to OpenMRS
- FM2-605: Add Support for ETags in the FHIR API
- FM2-481: Clean up parameter passing for all Service class methods

### Talk Thread links:
- https://talk.openmrs.org/t/gsoc-2023-fhir-add-support-for-fhir-patch-operations-project-updates/39555  

### Weekly Blog Posts:
Throughout the development cycle, I chronicled my progress and insights through weekly blog posts:

- GSOC WEEK 12 - WRAPPING UP A FRUITFUL GSOC JOURNEY: ADDING CONTACT POINTS TO THE OPENMRS-MODULE-INITIALIZER
- GSOC WEEK 11: A JOURNEY OF REFINEMENT AND INNOVATION IN FHIR2 MODULE
- GSOC WEEK 10 - EMBRACING THE FINALE: REFLECTING ON MY GSOC JOURNEY
- GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 09
- GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 08
- GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 07
- GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 06
- GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 05
- GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 04
- GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 03
- GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 02
- GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 01
- GSOC 2023 AT OPENMRS | COMMUNITY BONDING PERIOD

## Video(Demo)
- url

## Resources:
- GSoC proposal
- Jira Epic
- Midterm evaluation video

## Future Works:
While significant strides have been made, certain aspects require further attention. Completing the integration of PATCH operations with complex FHIR resources is a priority. Additionally, refining error handling and optimizing performance will ensure a robust implementation.

Part of the work to be worked on includes but not limited to the following;-

- Ensure Service Request resource is  fully translated 
- Ensure Service Request resource supports all the PATCHing formats implemented above.
- Write more tests in regard to the how the json documents and xml documents should be written in the attempt to give clearer error messages.(To Be Discussed)
- We could also implement the PATCH operations for the R3 resources(To Be Discussed).
  
## Thoughts on GSoC:
Participating in GSoC 2023 on the OpenMRS platform has been an enlightening journey. Working with esteemed mentors like Ian Bacher and Abert Namanya has been instrumental in my growth. I have gained insights into the world of healthcare informatics, API optimization, and collaborative open-source development. Looking forward, GSoC has paved the way for a continued commitment to enhancing healthcare technology. My knowledge in FHIR standards and OpenMRS data model and how the two integrate to complement each other has greatly grown.

A special thanks to GSoC, OpenMRS, mentors, and the vibrant community for making this journey a resounding success! 🌟🌐
