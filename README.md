There are many books needed to be read relating to Software Engineering. The "Object-Oriented Software Engineering" by Lethbridge, "Software Engineering" by Sommerville,  the "Object-Oriented Software Engineering" by Bruegge, and "Software Requirement" by Wiegers, and "Professional Software Engineering" by Mcconnel.

All of them are required or recommended materials for some university courses at SFU. Should I do it?

With this much time spent, I could do many things. It might be a test to see if someone is serious about software engineering. Hopefully it's just all soft theory and nothing too dense.

Without further ado,let the learning begin :)

First book: "Object-Oriented Software Engineering" by Lethbridge

Web version: https://ifs.host.cs.st-andrews.ac.uk/Books/SE9/

# Chapter 1: Introduction to Software Engineering
* The notion of "software engineering" was first proposed in 1968 at a conference discussing what was then called the "software crisis". It became clear individual approaches to program development did not scale up to large and complex software system. These were unreliable, cost more than expected, and were delivered late.
* Throughout the 1970 and 1980, a variety of new software engineering techniques and methods were developed, such as structured programming, information hiding, and object-oriented development
* system documentation: describe the structure of the system
* user documentation: explain how to use the system
* This is one of the important differences between professional and amateur software development. If you are writing a programi for yourself, no one else will use it and you don't have to worry about writing program guides, documenting the program design, etc. However, if you are writing software that other people will use and other engineers will change then you usually have to provide additional information as well as the code of the program 
* maintainability, dependability and security (reliability, security, and safety), efficiency, acceptability
* The systematic approach that is used in software engineering is sometimes called a software process. A software process is a sequence of activities that lead to the production of a software product. There are four fundamental activities that are common to all software processes. These activities are: software specification(where customers and engineers define the software that is to be produced and the constraints on its operation), software development(where the software is designed and programmed), software validation(where the software is checked to ensure that it is what the customer requries), software evolution(where the software is modified to reflect changing customer and market requirement).
* different types of systems need different development processes. For example, real-time softwrae in an aircraft has to be completely specified before development begins. In e-commerce system, the specification and the program are usually developed together. 
* There are three general issues that affect many different types of software: heterogeneity, cope with different devices and systems; business and social change, able to cope with the changing business and society and develop as rapidly; security and trust: it is essential that we can trust the software because it interwined with all aspects of our lives. This is especially true for remote software systems accessed through a web page or web service interface. We have to make sure that malicious users can not attack our software and that information security is maintained
* different types of application: stand-alone application: run on a local computer, such as a PC. they include all necessary funcationlity and do not need to be connected to a network. Ex: office applicaiton, CAD program, photo manipulation software; 2. Interactive transaction-based application: e-commerce, mail, photo sharing; 3. embedded control system: software control systems that control and manage hardware devices; 4. batch processing system: busienss system that are designed to process data in large batches, ex: periodic billing system, or salary payment system; 5. entertainment system: intended to entertain the user; 6. system for modeling and simulation: system that are developed by scientist and engeineers to model physical processes or situations; 7. data collection system: systems that use a set of sensor, ex. installed in a hostile environment such as inside an engine or in a remote location; 8. systems of systems: ex: a spreadsheet program


MY: (https://www.cleverism.com/management-information-systems-mis/) this is different from the definition in MIS. MIS deals with information system that is used in business: 1. transaction processing system: MYex: a receipt machine; 2. decision support system: computer supported cooperative work, group decision support system, logistics system and financial planning system; 3. executive information system; 4. management information system: process control system, human resource management system, sales and marketing system, inventory control system, office automation system, enterprise resource planning system, accounting and finance system, and management reporting systems

MY: Therefore, it is a total different categorization of definitions

* web service: is software component that deliver specific, useful functionality and which are accessed over the Web. Applications are constructed by integrating these web services, which may be provided by different companies.
* The radical change toward the web has led to changes in the ways that web-based systems are engineered: 1. software reuse has become the dominant approach for constructing web-based system. When building these systems, you think about how you can assemble them from pre-existing software components and systems; 2. it is now generally recognized that it is impractical to specify all the requirements for such system in advance. Web-based systems should be developed and delivered incrementally; 4. User interfaces are constrained by the capability of web browsers.

### Software engineering ethics
* confidentiality: respect the confidentiality of your employers or clients
* compoetence: should not misrepresent your level of competence 
* intellectual property rights
* computer misuse

MY: From ACM and the IEEE, because of their roles in developing software system, software engineers have significant opportunities to do good or cause harm, to enable others to do good or cause harm, or to influence others to do good or cause harm. 

# Chapter 2: Software processes
* Waterfall model: in principle, the waterfall model should only be used when the requirements are well understood and unlikely to change radically during system development.
* incremental development: lots of advantages, but: the process is not visible. Managers need regular deliverables to measure progress; system structure tends to degrade as new increments are added. The problem of incremental development become particularly acute for large, complex, long-lifetime system, where different team develop different parts of the system. Large systems need a stable framework or architecture and the responsibilities of the different team working on parts of the system need to be clearly defined with respect to that architecture. This has to be planned in advanced rather than developed incrementally. || You can develop a system incrementally and expose it to customers for comment, without actually delivering it and deploying it in the customer's environment. 
* reuse-oriented software engineering: reply on a large base of reuseable software components and an integrating framework for the composition of these components. Stages: 1. component analysis: given the requirement spcification, a search is made for components to implement that specification. Usually, there is no exact match and the components that may be used only provide some of the functionality required. 2. requirements modification: during this stage, the requirement are analyzed using information about the components that have been discovered. They are then modified to reflect the available components. When modificaitons are impossible, the component analysis activity may be re-entered to search for alternative solutions. 3. System design with reuse: during this phase, the framework of the system is designed or an existing framework is reused. The designers take into account the components that are reused and organize the framework to cater for this. Some new software may have to be designed if reusable components are not available. 4. Development and integration: Software that can not be externally procured is developed, and the components and COTS system are integrated to create the new system. System integration, in this model, may be part of the development process rather than a separate activity. || There are three types of software component that maybe used in a reuse-oriented process: 1. web services; 2. collections of object that are developed as a package to be integrated with a component framework such as .NET or j2EE; 3. Stand-alone software system taht are configured for use in a particular environment.
* testing stages: development testing: tested by people developing the system, system testing: testing for integration; acceptance testing:  the system is tested with data supplied by the system customer rather than with simulated test data. Acceptance testing may reveal errors and omissions in the system requirements definition.
* Prototyping: SKIM
* Incremental delivery: SKIM
* Boehm's spiral model: SKIM
* Rational Unified Process: SKIM

# Chapter 3: Agile software development

Page 57