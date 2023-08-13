DISCLAIMER: This repo contains copyrighted material the use of which has not always been specifically authorized by the copyright owner. In accord with the purpose of notetaking/search/retrieval in an easy way and convenient way, we are making such material available to advance understanding of Software Engineering. We believe this constitute a "fair use" of any such copyrighted material as provided in Section 107 of the US Copyright Law. In accordance with Title 17 U.S.C Section 107, the material on this site is distributed without profit to those who have expressed a prior intereste in receiving the included information for research and educational purposes. For further information on fair use, go to https://www.law.cornell.edu/uscode/text/17/107
If you wish to use copyrighted material from this site for purposes of your own that go beyond fair use, you must obtain permission from the copyright owner.

There are many books needed to be read relating to Software Engineering. The "Object-Oriented Software Engineering" by Lethbridge, "Software Engineering" by Sommerville,  the "Object-Oriented Software Engineering" by Bruegge, and "Software Requirement" by Wiegers, and "Professional Software Engineering" by Mcconnel.

All of them are required or recommended materials for some university courses at SFU. Should I do it?

With this much time spent, I could do many things. It might be a test to see if someone is serious about software engineering. Hopefully it's just all soft theory and nothing too dense.

Without further ado,let the learning begin :)

First book: "Software Engineering" by Sommerville

Web version: https://ifs.host.cs.st-andrews.ac.uk/Books/SE9/

# Preface
* As I was writing the final chapters in this book in the summer of 2009, I realized taht software engineerring was 40 years old. The name "software engineering" was proposed in 1969 at a NATO conference to discuss the functionality needed by their users, cost more than expected, and were unreliable. I did not attend that conference but, a year later, I wrote my first program and started my professional life in software.
* Progress in software engineering has been remarkable over my professional lifetime. Our societies could not function without large, professional software systems. For building business systems, there is an alphbet soup of technologies--J2EE, .Net, SaaS, SAP, BPEL4WS, SOAP, CBSE, etc--that support the development and deployment of large enterprise applications. National utilities and infrastructure--energy, communicaitons, and transport--all reply on complex and mostly reliable computer systems. Software has allowed us to explore space and to create the World Wide Web, the most significant information system in the history of mankind. Humanity is now faced with a new set of challenges--climate change and extreme weather, declining natural resources, an increasing world population to be fed and housed, international terrorism, and the need to help elderly people lead satisfying and fulfilled lives. We need new technologies to help us address these problems and, for sure, software will play a central role in these technologies.
* Software engineering is, therefore, a critically important technology for the future of mankind. We must continue to educate software engineers and develop the discipline so that we can create more complex software systems. Of course, there are still problems with software projects. Software is still sometimes late and costs more than expected. However, we should not let these problems conceal the real successes in software engineering and the impressive software engineering methods and technologies that have been developed.
* Software engineering is now such a huge area that it is impossible to cover the whole subject in one book. My focus, therefore, is on key topics that are fundamental to all development processes and topics concerned with the development of reliable, distributed systems. There is an increased emphasis on agile methods and software reuse. I strongly believe that agile methods have t heir place but so too does "traditional" plan-driven software engineering. We need to combine the best of these approaches to build better software systems.
* Books inevitably reflect the opinions and prejudices of their authors. Some readers will inevitably disagree with my opinions and with my choice of material. Such disagreement is a healthy reflection of the diversity of the discipline and is essential for its evolution. Nevertheless, I hope that all software engineers and software engineering students can find something of interest here.

# PART 1 Introduce to Software Engineering
* My aim in this part of the book is to provide a general introduction in software engineering. I intorduce important concepts such as software processes and agile methods, and describe essential software development activities, from initial software specification through to system evolution. The chapters in this part have been designed to support a one-semester course in software engineering.
* Chapter 1 is a general introduction professional software engineering and defines some software engineering concepts. I have also written a brief discussion of ethical issues in software engineering. I think that it is important for software engineers to think about the wider implications of their work. This chapter also introduces three case studies that I use in the book, namely a system for managing records of patient undergoing treatment for mental health problems, a control system for a portable insulin pump and a wilderness weather system.
* Chapter 2 and 3 cover software engineering processes and agile development. In Chapter 2, I introduce commonly used generic software process models, such as the waterfall model, and I discuss the basic activities that are part of these processes. Chapter 3 supplements this with a discussion of agile development methods for software engineering. I mostly use Extreme Programming as an example of an agile method but also briefly introduce Scrum in this chapter.
* The remainder of the chapters in this part are extended description of the software process activities that will be introduced in Chapter 2. Chapter 4 covers the critically important topics of requirement engineering, where the requirements for what a system should do are defined. Chapter 5 introduces system modeling using the UML, where I focus on the use of use case diagrams, class diagrams, sequence diagrams, and state diagrams for modeling a software system. Chapter 6 introduces architectural design and I discuss the importance of architecture and the use of architectural pattern in software design.
* Chapter 7 introduces object-oriented design and the use of design patterns. I also introduce important implementation issues here--reuse, configuraiont management, and host-target development and discuss open source development. Chapter 8 focuses on software testing from unit testing during system development to the testing of software releases. I also discuss the use of test-driven development--an approach pioneered in agile methods but which has wide applicability. Finally, Chapter 9 presents an overview of software evolution issues. I cover evolution processes, software maintence, and legacy system management.

# Introduction

## Objectives
* The objectives of this chapter are to introduce software engineering and to provide a framework for understanding the rest of the book. When you have read this chapter you will:

        * Understand what software engineering is and why it is important;
        * understand that the development of different types of softawre systems may require different software engineering techniques;
        * understand some ethical and professional issues taht are important for software engineers;
        * have been introduced to three systems, of different types, that will be used as examples throughout the book.

* We can't run the modern world without software. National infrastructures and utilities are controlled by computer-based systems and most electrical products include a computer and controlling software. Industrial manufacturing and distribution is completely computerized, as is the financial system. Entertainment, including the music industry, computer games, and film and television, is softare intensive. Therefore, softawre engineering is essential for the functioning of national and international societies.
* Software systems are abstract and intangible. They are not constrained by the properties of materials, governed by phyiscal laws, or by manufacturing processes. This simplifies software engineering, as there are no natural limits to the potential of software. However, because of the lact of physical constraints, softare systems can quickly become extremely complex, difficult to understand, and expensive to change.
* There are many different types of software systems, from simple embeded systems to complex, worldwide information systems. It is pointless to look for universal notations, methods, or techniques for software engineering because different types of software require different approaches. Developing an organizaitonal information system is completely different from developing a controller for a scientific instrument. Neither of these systems has much in common with a graphics-intensive computer game. All of these applications need software engineering; they do not all need the same software engineering techniques.
* There are still many reports of software projects going wrong and "software failures". Software engineering is criticized as inadequate for modern softare development. However, in my view, many of these so-called software failures are a consequence of two factors:

1. Increasing demands. As new software engineering techniques help us to build larger, more complex systems, the demands change. Systems have to be built and delivered more quickly, larger, even more complex systems are required; systems have to have new capabilities that were previously thought to be impossible. Existing software engineering methods can not cope and new software engineering techniques have to be developed to meet new these new demands.
2. Low expectation. It is relatively easy to write computer programs without using software engienering methods and techniques. Many companies have drifted into software development as their products and services have evolved. They do not use software engineering methods in their everyday work. Consequentl, their software is often more expensive and less reliable than it should be. We need better software engineering education and training to address this problem.

* Software engineers can be rightly proud of their achievements. Of courese we still have problems developing complex software but, without software engineering, we would not have explored space, would not have the Internet of modern telecommuniations. All forms of travel would be more dangerous and expensive. Software engineering has contributed a great deal and i am convinced that its contribution in the 21st century will be even greater.

```
History of software engineering
* The notion of "software engineering" was first proposed in 1968 at a conference discussing what was then called the "software crisis". It became clear individual approaches to program development did not scale up to large and complex software system. These were unreliable, cost more than expected, and were delivered late.
* Throughout the 1970 and 1980, a variety of new software engineering techniques and methods were developed, such as structured programming, information hiding, and object-oriented development. Tools and standard notations were developed and are now extensively used.
 
```

## 1.1 Professional Software Development
* Lots of people write programs. People in business write spreadsheet programs to simplify their jobs, scientists and engineers write programs to process their experimental data, and hobbyists write programs for their own interest and enjoyment. However, the vast majority of software development is a professional activity where software is developed for specific business purposes, for inclusion in other devices, or as software products such as information systems, CAD systems, etc. Professional software, intended for use by someone apart from its developer, is usually developed by teams rather than individuals. It is maintained and changed throughout its life.
* Software engineering is intended to support professional software development, rather than individual programming. It includes techniques that support program specification, design, and evolution, none of which are normally relevant for personal software development. To help you to get a board view of what software engineering is about, I have summarized some frequently asked questions in Figure 1.1.
* Many people think that software is simply another word for computer programs. However, when we are talking about software engineering, software is not just the programs themselves but also all associated documentation and configuration data that is required to make these programs operate correctly. A professional developed software system is often more than a single program. The system usually consists of a number of separate programs and configuration files that are used to set up these programs. It may include system documentation, which describes the structure of  the system; user documentation, which explains how to use the system, and websites for users to download recent product information.
* **This is one of the important differences between professional and amateur software development. If you are writing a program for yourself, no one else will use it and you don't have to worry about writing program guides, documenting the program design, etc. However, if you are writing software that other people will use and other engineers will change then you usually have to provide additional information as well as the code of the program.**

```
Figure 1.1 Frequently asked questions about software
* Q: What is software? A: Computer programs and associated documentation. Software product may be developed for a particular customer or may be developed for a general market.
* Q: What are the attributes of good software. A: Good software should deliver the required functionality and performance to the user and should be maintainable, dependable, and usable.
* What is software engineering? A: Software engineering is an engineering discipline that is concerned with all aspects of software production.
* What are the fundamental software engineering activities? A: Software specification, software development, software validation, and software evolution.
* What is the difference between software engineering and computer science? A: Computer science focuses on theory and fundamentals; software engineering is concerned with the practicalities of developing and delivering useful software.
* What is the difference between software engineering and system engineering? A: System engineering is concerned with all aspects of computer-based systems development including hardware, software, and process engineering. Software engineering is part of this more general process.
* What are the costs of software engineering? A: Roughly 60% of software costs are development costs; 40% are testing costs. For custom software, evolution costs often exceed development costs.
* What are the best software engineering techniques and methods? A: While all software projects have to be professionally managed and developed, different techniques are appropriate for different types of system. For example, games should always be developed using a series of prototypes whereas safety critical control systems require a complete and analyzable specification to be developed. You can't, therefore, say that one method is better than another.

```

* Software engineers are concerned with developing software products (i.e., software which can be sold to a customer). There are two kinds of software products:

1. Generic products. These are standalone systems that are produced by a development organization and sold on the open market to any customer who is able to buy them. Examples of thiis type of product include software for PCs such as databases, word processors, drawing packages, and project management t ools. It also includes so-called vertical application designed for some specific purpose such as library information systems, accounting systems, and systems for maintaining dental records.
2. Customized (or bespoke) products. These are systems that are commissioned bny a particular customer. A software contractor develops the software especially for that customer. Examples of this type of software include control systems for electronic devices, system written to support a particular business process, and air traffic control systems.

* An important difference between these types of software is that, in generic products, the organization that develosp the software controls the software specification. For custom products, the specification is usually developed and controlled by the organization that is buying the software. The software develoeprs must work to that specificaiton.
* However, the distinction between these system product tpyes is becoming increasingly blurred. More and more systems are now being built with a generic product as a base, which is then adapted to suit the requirements of a customer. Enterprise Resource Planning (ERP) systems, such as the SAP system, are the best examples of this approach. Here, a large and complex system is adapted for a company by incorporating information about business rules and processes, reports required, and so on.
* When we talk about the quality of professional software, we have to take into account that the software is used and changed by people apart from its developers. Quality is therefore not just concerned with what the software does. Rather, it has to include the software's behavior while it is executing and the structure and organization of the system programs and associated documentation. This is reflected in so-called quality or non-functional software attributes. Examples of these attributes are the software's response time to a user query and the understandability of the program code.
* The specific set of attributes that you might expect from a software system obviously depends on its applicatoin. Therefore, a banking system must be secure, an interactive game must be responsive, a telephone switching system must be reliable, and so on. These can be generalized into the set of attributes shown in Figure 1.2, which I believe are the essential characteristics of a professional software system.

### 1.1.1 Software engineering
* Software engineering is an engineering discipline that is concerned with all aspects of software production from the early stages of system specification through to maintaining the system after it has gone into use. In this definition, there are two key phrases:

1. Engineering discipline. Engineers make things work. They apply theories, methods, and tools where these are appropriate. However, they use them selectively and always try to discover solutions to problems even when there are no applicable theories and methods. Engineers also recognize that they must work to organizational and financial constraints so they look for solutions within these constraints.
2. All aspects of software production. Software engineering is not just concerned with the technical processes of software development. It also includes activities such as software project management and the development of tools, methods, and theories to support software production.

```
Figure 1.2. Essential attributes of good software 
* Maintainability: Software should be written in such a way so that it can evolve to meet the changing needs of customers. This is critical attribute because software change is an inevitable requirement of a changing business environment.
* Dependability and security: Software dependability includes a range of characteristics including reliability, security, and safety. Dependable software should not cause physical or economic damage in the event of system failure. Malicious users should not be able to access or damage the system.
* Efficiency: Software should not make wasteful use of system resources such as memory and processor cycles. Efficiency theory includes responsiveness, processing time, memory utilization, etc.
* Acceptability: Software must be acceptable to the type of users for which it is designed. This means that it must be understandable, useable, and compatible with other systems that they use.

```

* Engineering is about getting results of the required quality within the schedule and budget. This often involves making compromises--engineers can not be perfectionists. People writing programs for themselves, however, can spend as much time as they wish on the program development.
* In general, software engineers adopt a systematic and organized approach to their work, as this is often the most effective way to produce high-quality software. However, engineering is all about selecting the most appropriate method for a set of circumstances so a more creative, less formal approach to development may be effective in some circumstances. Less formal development is particularly appropriate for the development of web-based systems, which requires a blend of software and graphical design skills.
* Software engineering is important for two reasons:

1. More and more, individuals and society rely on advanced software systems. We need to be able to produce reliable and trustworthy systems economically and quickly.
2. It is usually cheaper, in the long run, to use software engineering methods and techniques for software systems rather than just write the programs as if it was a personal programming project. For most types of systems, the majority of costs and the costs of changing the software after it has gone into use.

* The systematic approach that is used in software engineering is sometimes called a software process. A software process is a sequence of activities that leads to the production of a software product. There are four fundamental activities that are common to all software processes. These activities are:

1. Software specification, where customers and engineers define the software that is to be produced and the constraints on its operation.
2. Software development, where the software is designed and programmed.
3. Software validation, where the software is checked to ensure that it is what the customer requires.
4. Software evolution, where the software is modified to reflect changing customer and market requirements.

* Different types of systems need different development processes. For example, real-time software in an aircraft has to be completely specified before development begins. In e-commerce systems, the specification and the program are usually developed together. Consequently, these generic activities may be organized in different ways and described at different levels of detail depending on the type of software being developed. I describe software processes in more detail in Chapter 2.
* Software engineering is related to both computer science and systems engineering:

1. Computer science is concerned with the theories and methods that underlie computers and software systems, whereas software engineering is concerned with the practical problems of producing software. Some knowledge of computer science is essential for software engineers in the same way that some knowledge of physics is essential for electrical engineers. Computer science theory, however, is often most applicable to relatively small programs. Elegant theories of computer science can not always be applied to large, complex problems that require a software solution.
2. System engineering is concerned with all aspects of the development and evolution of complex systems where software plays a major role. System engineering is therefore concerned with hardware development, policy and process design and system deployment, as well as software engineering. Systems engineers are involved in specifying the system, defining its overall architecture, and then integrating the difference parts to create the finished system. They are less concerned with the engineering of the system components (hardware, software, etc)

* As I discuss in the next section, there are many different types of software. There is no universal software engineering method or technique that is applicable for all of these. However, there are three general issues that affect many different types of software:

page 10



















===

Everything before


# Chapter 1: Introduction to Software Engineering
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
