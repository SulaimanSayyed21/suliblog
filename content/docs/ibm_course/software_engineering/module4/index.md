---
date: 2022-09-06T22:42:23+08:00
title: Softwae Architecture
linkTitle: Module 4
nav_weight: 4
series: 
  - Guide
categories:
  - Installation
tags:
  - Windows
images:
  - sdlc.webp
featured: false
authors:
  - Sulaiman
nav_icon:
  vendor: bs
  name: book
  color: indigo
---
### **Foundations of Software Architecture**


Software architecture forms the backbone of any software system, acting as both its blueprint and its guiding framework. It organizes the fundamental structures and defines how components interact, shaping the system’s behavior and aligning with key principles. During the software development lifecycle (SDLC), architectural design captures critical early decisions that influence not only the system’s functionality but also its scalability, security, and adaptability.  

A well-crafted architecture balances stakeholder needs, facilitates communication among teams, and serves as a foundation for technology stack and production environment decisions. This video introduces the essential concepts of software architecture, explores its impact on design decisions, and outlines the artifacts—such as architectural diagrams and UML diagrams—that communicate design choices effectively. By the end, you’ll understand how strong architecture underpins robust, maintainable, and scalable software systems.  

**Software Design and Modeling:**  
Software design involves defining the structural components and behavioral attributes of a system before development. A key part of this process is **modeling**, where visual representations of a system’s structure and interactions are created. Unified Modeling Language (UML) is a standardized method for this, offering structural and behavioral diagrams. UML helps teams plan features, save time and money, and communicate effectively across technical and non-technical audiences.  

**Structured design** focuses on dividing software into well-organized modules. Good design ensures **cohesion** (grouping related functions) and **loose coupling** (minimizing dependencies between modules). Behavioral models describe system behavior without detailing implementation, often using diagrams like:  
- **State transition diagrams**: Show system states and transitions triggered by events (e.g., a patient moving through a clinic workflow).  
- **Interaction diagrams**: Visualize dynamic interactions among system components over time (e.g., scheduling an appointment via an online portal).  

The modularity and clarity provided by UML are especially beneficial in large, complex systems, allowing developers to navigate source code and onboard new team members efficiently.

---

**Application Deployment Environments:**  
Applications are deployed in distinct environments: **development**, **testing/QA**, **staging**, and **production**. Each serves a specific purpose:  
- **Development** is for active coding, often on individual workstations.  
- **QA** enables testing by the quality assurance team to identify issues.  
- **Staging** closely mimics production for pre-release validation but is not accessed by users.  
- **Production** is the live environment, designed for user access and optimized for load, scalability, security, and reliability.  

Applications can be deployed via different models:  
1. **On-premises**: Infrastructure is hosted within the organization for greater control but at higher costs.  
2. **Public cloud**: Shared resources managed by providers (e.g., AWS, Azure), offering cost efficiency and scalability.  
3. **Private cloud**: Dedicated infrastructure for one organization, prioritizing security and customization.  
4. **Hybrid cloud**: Combines public and private cloud benefits for flexibility, scalability, and security.  

---

**Architectural Patterns in Software:**  
Architectural patterns provide standardized solutions to common design challenges. Key patterns include:  
1. **2-tier (client-server):** Clients request data/services from a centralized server (e.g., messaging apps).  
2. **3-tier:** Separates applications into layers for the user interface (presentation), business logic (application), and data management (e.g., most web applications).  
3. **Peer-to-peer (P2P):** Decentralized nodes act as clients and servers, suitable for file sharing and cryptocurrencies like Bitcoin.  
4. **Event-driven:** Components produce and consume events, useful in dynamic systems like ride-sharing apps.  
5. **Microservices:** Applications are broken into independent services interacting via APIs (e.g., social media platforms).  

Some patterns can be combined (e.g., microservices within a 3-tier system) to leverage multiple benefits, though some (e.g., P2P and 2-tier) are incompatible due to structural differences.

---

**Object-Oriented Analysis and Design (OOAD):**  
OOAD is a methodology for designing software systems using object-oriented programming. The foundation of OOAD is the **object**, which encapsulates data and behaviors. Objects are instances of **classes**, which act as blueprints defining generic attributes and methods. For example, a patient object (e.g., Naya Patel) would be an instance of the patient class, which includes attributes like name and methods like scheduling an appointment.  

A **class diagram** is a structural UML tool used in OOAD to depict the relationships between classes. For example, subclasses like nurse and doctor inherit attributes from a parent class like medical personnel, while adding specialized properties. OOAD facilitates modular system development, enabling multiple teams to work simultaneously while maintaining consistency and scalability.  

---

This summary offers a structured overview of software design, environments, architectural patterns, and OOAD principles, emphasizing their roles in efficient software development.


### FAQ

{{< bs/accordion data="software_engineering.faq" flush=true >}}