## Add Support for FHIR PATCH operations
- **Project Title**: Add Support for FHIR PATCH operations
- **Primary mentor**:  Ian Bacher @ibacher 
- **Backup mentor**:  Abert Namanya @abertnamanya 
- **Project Link**: [GSoC-2023: FHIR: Add Support for FHIR PATCH operations](https://wiki.openmrs.org/display/projects/GSoC+2023+%3A+FHIR%3A+Add+support+for+FHIR+PATCH+operations)
- **Project Report**: https://github.com/mherman22/GSOC-FinalReport

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
- https://github.com/openmrs/openmrs-module-fhir2/pull/513 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/489 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/485 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/483 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/488 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/490 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/491 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/484 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/481 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/487 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/479 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/480 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/492 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/493 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/478 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/499 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/500 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/501 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/502 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/503 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/505 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/507 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/509 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/513 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/498 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/495 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/496 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/497 - Merged ✅

### Found Issues:
- Medication Dispense was not added to the landing page of the FhirIG
- Medication was not added to the landing page of the FhirIG

### Fixed Issues:
- https://github.com/openmrs/openmrs-contrib-fhir2-ig/pull/59 - Merged ✅
- https://github.com/openmrs/openmrs-contrib-fhir2-ig/pull/60 - Merged ✅

### Other related work:
During this GSoC jouney, i was able to do other work on the FHIR module as assigned by my mentor and below are the pull requests;-
- [FM2-606: Mapping ContactPoints to OpenMRS](https://github.com/openmrs/openmrs-module-fhir2/pull/517) - Merged ✅
- [FM2-605: Add Support for ETags in the FHIR API](https://github.com/openmrs/openmrs-module-fhir2/pull/515) - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/510 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/518 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/511 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/512 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/504 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/505 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/442 - Merged ✅
- https://github.com/openmrs/openmrs-module-fhir2/pull/441 - Merged ✅

### Talk Thread links:
- https://talk.openmrs.org/t/gsoc-2023-fhir-add-support-for-fhir-patch-operations-project-updates/39555  

### Jira Epic
- https://issues.openmrs.org/browse/FM2-573

### Weekly Blog Posts:
Throughout the development cycle, I chronicled my progress and insights through weekly blog posts:

- [GSOC WEEK 12 - WRAPPING UP A FRUITFUL GSOC JOURNEY: ADDING CONTACT POINTS TO THE OPENMRS-MODULE-INITIALIZER](https://hermanmuhereza.blogspot.com/2023/08/week-12-wrapping-up-fruitful-gsoc.html)
- [GSOC WEEK 11: A JOURNEY OF REFINEMENT AND INNOVATION IN FHIR2 MODULE](https://hermanmuhereza.blogspot.com/2023/08/gsoc-2023-at-openmrs-coding-period-week_18.html)
- [GSOC WEEK 10 - EMBRACING THE FINALE: REFLECTING ON MY GSOC JOURNEY](https://hermanmuhereza.blogspot.com/2023/08/gsoc-2023-at-openmrs-coding-period-week_10.html)
- [GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 09](https://hermanmuhereza.blogspot.com/2023/08/gsoc-2023-at-openmrs-coding-period-week.html)
- [GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 08](https://hermanmuhereza.blogspot.com/2023/07/gsoc-2023-at-openmrs-coding-period-week_24.html)
- [GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 07](https://hermanmuhereza.blogspot.com/2023/07/gsoc-2023-at-openmrs-coding-period-week_0216759827.html)
- [GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 06](https://hermanmuhereza.blogspot.com/2023/07/gsoc-2023-at-openmrs-coding-period-week_10.html)
- [GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 05](https://hermanmuhereza.blogspot.com/2023/07/gsoc-2023-at-openmrs-coding-period-week.html)
- [GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 04](https://hermanmuhereza.blogspot.com/2023/06/gsoc-2023-at-openmrs-coding-period-week_26.html)
- [GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 03](https://hermanmuhereza.blogspot.com/2023/06/gsoc-2023-at-openmrs-coding-period-week_19.html)
- [GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 02](https://hermanmuhereza.blogspot.com/2023/06/gsoc-2023-at-openmrs-coding-period-week_11.html)
- [GSOC 2023 AT OPENMRS | CODING PERIOD WEEK 01](https://hermanmuhereza.blogspot.com/2023/06/gsoc-2023-at-openmrs-coding-period-week.html)
- [GSOC 2023 AT OPENMRS | COMMUNITY BONDING PERIOD](https://hermanmuhereza.blogspot.com/2023/05/gsoc-2023-at-openmrs-community-bonding.html) 

## Video(Demo)
- url

## Resources:
- [GSoC proposal](https://docs.google.com/document/d/14g2EddqKIpon3xXI71BMKXfu5zISIy6Psy9NgCp4t6Q/edit?usp=sharing)
- [Midterm evaluation video](https://www.youtube.com/watch?v=P-0gj-8LOCE&t=8s)
- https://issues.openmrs.org/browse/FM2-573

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
