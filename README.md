## GSoC 2024: Integrating OpenELIS with a FHIR-Based Open Client Registry
- **Project Title**: Integrating OpenELIS with a FHIR-Based Open Client Registry
- **Primary Mentor**: @reagan 
- **Backup Mentor**: @mozzymutesa 
- **Project Report**: pending...

### Overview
This integration is designed to seamlessly connect **OpenELIS**, a laboratory information system, with a FHIR-Based Open Client Registry. The primary objective is to enhance patient data management by facilitating patient searches within the local OpenELIS system. When a user initiates a patient search within OpenELIS, the system will first attempt to locate the patient within its own database. 

If the patient cannot be found locally, the integration will extend the search to the central Open Client Registry. This central registry serves as a repository of patient information, allowing OpenELIS to query and retrieve patient details from this broader database. Once the patient information is located in the client registry, it will be imported into OpenELIS, ensuring that the local system is updated with the most current and complete patient data.

In summary, this integration allows users to efficiently find patient records within their local OpenELIS system and, if necessary, access and import patient information from a central client registry, thus ensuring that patient data is both comprehensive and up-to-date across systems.

### Objectives

- Set up a repository on which I will use docker-compose to bring different pieces of
the OpenCR like hapi fhir, elastic search together with OpenElis.

- Set up using docker-compose the OpenHim mediator to act as the interoperability
layer between OpenCR and OpenElis, make all the configurations like channels,
mediators, clients, etc.

- Set up using docker-compose the OpenCR client and all the different components it
needs to function properly,i.e hapi-fhir, elastic search, etc and make all the necessary
configurations.
- Set up using docker-compose the OpenElis client and all the different components it
needs to function properly.

### What did i do? (Contributions)
During the project, I worked on various code repositories and pull requests to bring together the required functionality and meet the goals.

### Repositories
- https://github.com/mherman22/OpenELIS-OpenCR-HIE-Setup
- https://github.com/intrahealth/client-registry
- https://github.com/I-TECH-UW/OpenELIS-Global-2

### Pull Requests
- https://github.com/intrahealth/client-registry/pull/148
- https://github.com/intrahealth/client-registry/pull/137
- https://github.com/I-TECH-UW/OpenELIS-Global-2/pull/1219
- https://github.com/I-TECH-UW/OpenELIS-Global-2/pull/1065
- https://github.com/I-TECH-UW/OpenELIS-Global-2/pull/1065/commits/96605f8c8be0a77e05a22ea1aef7b75d1e94535c

### Final Video Presentation

[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.youtube.com/watch?v=Sa9EJm0a8Ks)

### What’s left to do? 
- Polish up on the Querying of the client registry and get [this pull request](https://github.com/I-TECH-UW/OpenELIS-Global-2/pull/1219) merged.
- Thereafter, we can import the patient information from openclient registry into **OpenELIS**

### Any challenges or important things i learned during the project.
I will talk about the important things i have learned which include everything about docker, configurations of opencr, openhim, fhir, etc.

### Resources 
- https://www.openclientregistry.org/ 
- https://intrahealth.github.io/client-registry-docs/dev/installation_full/ 
- https://intrahealth.github.io/client-registry/ 
- http://openhim.org/ - https://hapifhir.io/ 

## Thoughts on GSoC:
Participating in GSoC 2024 on the OpenELIS platform has been an incredibly enlightening experience. The guidance of esteemed mentors like Reagan and Moses has been pivotal in my growth. I've gained valuable insights into healthcare informatics, API optimization, and collaborative open-source development. As I look ahead, GSoC has laid a strong foundation for my continued commitment to advancing healthcare technology, deepening my knowledge of FHIR standards, OpenCR, OpenHIM, and more.

A heartfelt thanks to GSoC, OpenELIS, my mentors, and the  community for the lessons and opportunities. :star2::globe_with_meridians:


