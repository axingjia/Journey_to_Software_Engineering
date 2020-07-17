DISCLAIMER: This repo contains copyrighted material the use of which has not always been specifically authorized by the copyright owner. In accord with the purpose of notetaking/search/retrieval in an easy way and convenient way, we are making such material available to advance understanding of Software Engineering. We believe this constitute a "fair use" of any such copyrighted material as provided in Section 107 of the US Copyright Law. In accordance with Title 17 U.S.C Section 107, the material on this site is distributed without profit to those who have expressed a prior intereste in receiving the included information for research and educational purposes. For further information on fair use, go to https://www.law.cornell.edu/uscode/text/17/107
If you wish to use copyrighted material from this site for purposes of your own that go beyond fair use, you must obtain permission from the copyright owner.

There are many books needed to be read relating to Software Engineering. The "Object-Oriented Software Engineering" by Lethbridge, "Software Engineering" by Sommerville,  the "Object-Oriented Software Engineering" by Bruegge, and "Software Requirement" by Wiegers, and "Professional Software Engineering" by Mcconnel.

All of them are required or recommended materials for some university courses at SFU. Should I do it?

With this much time spent, I could do many things. It might be a test to see if someone is serious about software engineering. Hopefully it's just all soft theory and nothing too dense.

Without further ado,let the learning begin :)

First book: "Software Engineering" by Sommerville

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
* For some types of software, such as safety-critical control system, where a complete analysis of the system is essential, a plan-driven approach is the right one.
* however, in a fast-moving business environment, this can cause real problem
* in the 1980 and early 1990, there was a widespread view that the best way to achieve better software was through careful project planning, formalized quality assurance, the use of analysis and design methods supported by CASE tools, and controlled and rigorous software development processes. This view came from the software engineering community that was responsible for developing large, long-lived software system such as aerospace and government systems.
* However, when this heavyweight, plan-driven development approach is applied to small and medium-sized business systems, the overhead involved is too large.
* Dissatisfaction with these heavyweight approach to software engineering led to a number of software developers in the 1990s to propse new "agile methods"
* Agile manifesto: When are uncovering better ways of developing software by doing it and helping others do it. Thrugh this work we have come to value: Individuals and interactions over processes and tools; working software over comprehensive documentation; customer collaboration over contract negotiation; responding to change over following a plan
* In practice, the principles underlying agile methods are sometimes difficult to realize because: 1. although the idea of customer involvement in the development process is an attractive one, its success depends on having a customer who is willing and able to spend time with the development team and who can represent all system stakeholders. 2: individual team members may not have suitable personalities for the intense involvement that is typical of agile methods, and therefore not interact well with other team members; 3. prioritizing changes can be extremely difficult, especially in system for which there are many stakeholders. Typically, each stakeholders gives different priorities to different changes; 4. maintaining simplicity requires extra work. Under pressure from delivery schedules, the team members may not have time to carry out desirable system simplifications.

#### Plan-driven and agile development
1. Is it important to have a very detail specification and design before moving to implementation? If so, you probably need to use a plan-driven approach
2. Is an incremental delivery strategy, where you deliver the software to customers and get rapid feedback from them, realisitic? If so, consider using agile methods.
3. How large is the system that is being developed? Agile methods are most effective when the system can be developed with a small co-located team who can communicate informally. This may not be possible for large system that require larger development teams so a plan-driven approach may have to be used.
4. What type of system is being developed? System that require a lot of analysis before implementation(e.g. real-time system with complex timing requirements) usually need a fairly detailed design to carry out this analysis. A plan-driven approach may be best in those circumstances.
5. What is the expected system lifetime? Long-lifetime system may require more design documentation to communicate the original intentions of the system developers to the support team. However, supporters of agile methods rightly argue that documentation is frequently not kept up to date and it is not of much use for long-term system maintenance.
6. What technologies are available to support system development? Agile methods often reply on good tools to keep track of an evolving design. If you are developing a system using an IDE that does not have good tools for program visualization and analysis, then more design documentation may be required.
7. How is the development team organized? If the development team is distributed or if part of the development is being outsourced, then you may need to develop design documents to communicate across the development teams. You may need to plan in advance what these are.
8. Are there cultural issues that may affect the system development? Traditional engineering organizations have a culture of plan-based development, as this is the norm in engineering. This usually requires extensive design documentation, rather than the informal knowledge used in agile processes.
9. How good are the designers and programmers in the development team? It is sometimes argued that agile methods require higher skill levels than plan-based approaches in which programmers simply translate a detailed design into code. If you have a team with relatively low skill levels, you may need to use the best people to develop the design, with others responsible for programming.
10. Is the system subject to external regulation? If a system has to be approved by an external regulator (e.g., the Federal Aviation Authority [FAA] approve software that is critical to the operation of an aircraft) then you will probably be required to produce detailed documentation as part of the system safety case.

#### Extreme programming
SKIM 

#### Paired programming 
SKIM 

SKIP

# Chapter 4: Requirement Engineering
* The process of finding out, analyzing, documenting and checking these services and constraints is called requirements engineering
* User requirement and system requirement: SKIM
* Non functionale requirement: reliability, response time, and store occupancy, performance, security, availability
* Metrics for specifying non-fnctional requirement: speed: processed transaction/second; user/event response time; screen refresh time; 2. size:Mbytes, number of ROM chips; 3. ease of use: training time, number of help frames; 4. reliability: mean time to failure, probability of unavailability, rate of failure occurance, availability; 5. robustness: time to restart after failure; percentage of events causing failure; probability of data corruption on failure; portability: percentage of target dependent statements, number of target system
* Requirement Specification
* use open-ended and closed-ended question, scenerio, use cases
* Requirement Validation. The cost of fixing a requirement problem by making a system change is usually much greater than repairing design or coding erros. The reason for this is that a change to the requirements usually means that the system design and implementation must also be changed. Furthermore the system must then be re-tested.
* During the requirement validation process, different types of checks should be carried out on the requirements in the requirements document. These check include: 1. validation check: check if there are additional or different functions than we think. 2. Consistency check. Requirement in the document should not conflict. That is, there should not be contradictory constraints or different descriptions of the same system function. 3. Completeness check: The requirements document should include requirements that define all functions and the constraints intended by the system user. 4. Realism. Make sure the requirement can actually be implemented. 5. Verifiability: To reduce the potential for dispute between customer and contractor, system requirements should always be written so that they are verifiable.
* There are a number of requirement validation techniques that can be used individually or in conjunction with one another: 1. requirements review. The requirements are analyzed systematically by a team of reviewers who check for errors and inconsistencies. 2. prototyping. In this approach to validation, an executable model of the system in question is demonstrated to end-users and customers. They can experiment with this model to see if it meets their real needs. 3. Test-case generation. Requirements should be testable. If the tests for the requirement are devised as part of the validation process, this often reveals requirements problems. If a test is difficult or impossible to design, this usually means that the requirements will be difficult to implement and should be reconsidered. Developing tests from the user requirements before any code is written is an integral part of extreme programming.
* Requirement management: SKIP

# Chapter 5: System Modeling
* System modeling is the process of developing abstract models of a system, with each model presenting a different view or perspective of that system.
* You may develop different models to represent the system from different perspectives. For example, 1. an external perspective, where you model the context or environment of the system. 2. An interaction perspective where you model the interactions between a system and its environment or between the components of a system. 3. A structural perspective, where you model the organization of a system or the structure of the data that is processed by the system. 4. A behavioral perspective, where you model the dynamic behavior of the system and how it responds to events.
* Krutchen's 4+1 iew will be discussed in Chapter 6.
* Activity diagram, user case diagram, sequence diagram, class diagram, state diagram

###### Context Model
* At an early stage in the specification of a system, you should decide on the system boundaries. This involves working with system stakeholders to decide what functionality should be included in the system and what is provided by the system's environment.

###### Interactino Models 
* Modeling system to system interaction highlights the communication problems that may arise. Modeling component interaction helps us understand if a proposed system structure is likely to deliver the require system performance and dependability
* Use case modeling 
* sequence diagram

###### Structural Models 
* Class diagram
* generalization empty arrowhead
* Aggregation: diamond arrowhead

###### Behavioral Models
* Data-driven modeling (data-flow model)
* Event-driven modeling
* State diagram

### Model-driven engineering
SKIP 

# Chapter 6: Architectural Design 
* Architectural design is concerned with understanding how a system should be organized and designing the overall structure of that system.
* In the model of the software development process, architectural design is the first stage in the software design process. It is the critical link between design and requirements engineering
* SKIP

# Chapter 7: Design and Implementation
SKIM Nothing important

# Chapter 8: Software Testing
"Testing can only show the presence of erros, not their absence"
* SKIP

# Chapter 9: Software Evolution
SKIP 

# Chapter 10: Sociotechnical System

page 177
