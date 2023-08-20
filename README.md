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

1. Heterogeneity. Increasingly, systems are required to operate as distributed systems across networks that include different types of computer and mobile devices. As well as running on general-purpose computers, software may also have to execute on mobile phones. You often have to integrate new software with older legacy systems written in different programming languages. The challenge here is to develop techniques for building dependable software that is flexible enough to cope with this heterogeneity.
2. Business and social change. Business and society are changing incredibly quickly as emerging economies develop and new technologies become available. They need to be able to change their existing software and to rapidly develop new software. Many traditional software engineering techniques are time consuming and delivery of new systems often takes longer than planned. They need to evolve so that the time required for software to deliver value to its customers is reduced.
3. Security and trust. As software is interwined with all aspects of our lives, it is essential that we can trust that software. This is especially true for remote software systems accessed through a web page or web service interface. We have to make sure that malicious users can not attack our software and that information security is maintained.

* Of course, these are not independent issues. For example, it may be necessary to make rapid changes to a legacy system to provide it with a web service interface. To address these challenges we will need new tools and techniques as well as innovative ways of combining and using existing software engineering methods.

## 1.1.2. Software engineering diversity
* Software engineering is a systematic approach to the production of software that takes into account practical cost, schedule, and dependendability issues, as well as the needs of software customers and producers. How this systematic approach is actually implemented varies dramatically depending on the organization developing the software, the type of software, and the people involved in the development process. There are no universal software engineering methods and techniques that are suitable for all systems and all companies. Rather, a diverse set of software engineering methods and tools has evolved over the past 50 years.
* Perhaps the most significant factor in determining which software engineering methods and techniques are most important is the type of application that is being developed. There are many different types of application including:

1. Standalone applications. These are application systems that run on a local computer, such as a PC. They include all necessary functionality and do not need to be connected to a network. Examples of such applications are office application on a PC, CAD programs, photo manipulation software, etc.
2. Interactive transaction-based applications. These are applications that execute on a remote computer and that are accessed by users from their own PCs or terminals. Obviously, these include web applications such as e-commerce applications where you can interact with a remote system to buy goods and services. This class of application also includes business systems, where a business provides access to its systems through a web browser or special-purpose client program and cloud-based services, such as mail and photo sharing. Interactive applications often incorporate a large data store that is accessed and updated in each transaction.
3. Embedded control systems. These are software control systems that control and manage hardware devices. Numerically, there are probably more embedded systems than any other type of system. Examples of embedded systems include the software in a mobile phone, software that controls anti-lock braking in a car, and software in a microwave oven to control the cooking process.
4. Batch processing systems. These are business systems taht are designed to process data in large batches. They process large numbers of individual inputs to create corresponding outputs. Examples of batch systems include periodic billing systems, such as phone billing systems, and salary payment systems.
5. Entertainment systems. These are systems that are primarily for personal use and which are intended to entertain the user. Most of these systems are games of one kind or another.The quality of the user interaction offered is the most important distinguishing characteristic of entertainment systems.
6. Systems for modeling and simulation. These are systems that are developed by scientists and engineers to model phyiscal processes or situations, which include many, separate, interacting objects. These are often computationally intensive and require high-performance parallel systems for execution.
7. Data collection systems. These are systems that collect data from their environment using a set of sensors and send that data to other systems for processing. The software has to interact with sensors and often is installed in a hostile environment such as inside an engine or in a remote location.
8. Systems of systems. These are systems that are composed of a number of other software systems. Some of these may be generic software products, such as a spreadsheet program. Other systems in the assembly may be specially written for that environment.

* Of course, the boundaries between these system types are blurred. If you develop a game for a mobile phone, you have to take into account the same constraints (power, hardware interaction) as the developers of the phone software. Batch processing systems are often used in conjunction with web-based systems. For example, in a company, travel expense claims may be submitted through a web application but processed in a batch application for monthly payment.
* You use different software engineering techniques for each type of system because the software has quite different characteristics. For example, an embedded control system in an automobile is safety-critical and is burned into ROM when installedin  the vehicle. It is therefore very expensive to change. Such a system needs very extensive verification and validation so that the chances of having to recall cars after sale to fix software probelms are minimized. user interaction is minimal (or perhaps nonexistent) so there is no need to use a development process that relies on user interact prototyping.
* For a web-based system, an approach based on iterative development and delivery may be appropriate, wit the system being composed of reusable components. However, such an approach may be impractical for **a system of systems, where detailed specifications of the system interaction have to be specified in advance so that each system can be separately developed.**
* Nevertheless, there are software engineering fundamentals that apply to all types of software system:

1. They should be developed using a managed and understood development process. The organization developing the software should plan the development process and have clear ideas of what will be produced and when it will be completed. Of course, different processes are used for different types of software.
2. Dependability and performance are important for all types of systems. Software should behave as expected, without failures and should be available for use when it is required. It should be safe in its operation and, as far as possible, should be secure against external attack. The system should perform efficiently and should not waste resources.
3. Understanding and managing the software specification and requirements (what the software should do) are important. You have to know what different customers and users of the system expect from it and you have to manage their expectations so that a useful system can be delivered within budget and to schedule.
4. You should make as effective use as possible of existing resources. This means that, where appropriate, you should reuse software that has already been developed rather than write new software.

* These fundamental notions of process, dependendability, requirements, management, and reuse are important themes of this book. Different methods reflect them in different ways but they underlie all professional software development. 
* You should notice that these fundamentals do not cover implementation and programming. I don't cover specific programming techniques in this book because these vary dramatically from one type of system to another. For example, a scripting lanaguge such as Ruby is used for web-based system programming but would be completely inappropriate for embedded systems engineering.

## 1.1.3 Software engineering and the Web
* The development of the World Wide Web has had a profound effect on all of our lives. Initially, the Web was primarily a university accessible information store and it had little effect on software systems. These systems ran on local computers and were only accessible from within an organization. Around 2000, the Web started to evolve and more and more functionality was added to browsers. This meant that web-based systems could be developed where, instead of a special-purpose user interface, these systems could be accessed using a web browser. This led to the development of a vast range of new system products that delivered innovative serices, accessed over the Web. These are often funded by adverts that are displayed on the user's screen and do not involve direct payment from users.
* As well as these system products, the development of web browsers that could run small programs and do some local processing led to an evolution in business and organizational software. Instead of writing software and deploying it on users' PCs, the software was deployed on a web server. This made it much cheaper to change also reduced costs, as user interface development is particularly expensive. Consequently, wherever it has been possible to do so, many businesses have moved to web-based interaction with company software systems.
* The next stage in the development of web-based systems was the notion of web services. Web services are software components that deliver specific, useful functionality and which are accessed over the Web. Applications are constructed by integrating these web services, which may be provided by different companies. In principle, this linking can be dynamic so that an application may use different web services each time that it is executed. I cover this approach to software development in Chapter 19.
* In the last few years, the notion of "software as a service" has been developed. It has been proposed that software will not normally run on local computers but will run on "computing clouds" that are accessed over the Internet. If you use a service such as web-based mail, you are using a cloud-based system. A computing cloud is a huge number of linked computer systems that is shared by many users. Users do not buy software but pay according to how much the software is used or are given free access in return for watching adverts that are displayed on their screen.
* The advent of the web, therefore, has led to a significant change in the way that business software is organized. Before the web, business applications were mostly monolithic, single programs running on single computers or computer clusters. Communications were local, within an organization. Now, software is highly distributed, sometimes across the world. Business applications are not programmed from scratch but involve extensive reuse of components and programs.
* This radical change in software organization has, obviously, led to changes in the ways that web-based systems are engineered. For example:

1. Software reuse has become the dominant approach for constructing web-based systems. When building these systems, you think about how you cacn assemble them from pre-existing software components and systems.
2. **It is now generally recognized that it is impractical to specify all the requirements for such systems in advance. Web-based systems should be developed and delivered incrementally.**
* User interfaces are constrained by the capabilities of web browsers. Although technologies such as AJAX mean that rich interfaces can be created within a web browser, these technologies are still difficult to use. Web forms with local scripting are more commonly used. Application interfaces on web-based systems are often poorer than the specially designed user interfaces on PC system products.

* The fundamental ideas of software engineering, discussed in the previous section, apply to web based software in the same way that they apply to other types of software system. Experience gained with large system development in the 20th century is still relevant to web-based software.

## 1.2.  Software engineering ethics
* Like other engineering disciplines, software engineering is carried out within a social and legal framework that limits the freedom of people working in that area. As a software engineer, you must accept that your job involves wider responsibilities than simply the application of technical skills. You must also behavbe in an ethical and morally responsible way if you are to be respected as a professional engineer.
* It goes without saying that you should uphold normal standards of honesty and integrity. You should not use your skills and abilities to behave in a dishonest way or in a way that will bring disrepute to the software engineering profession. However, there are areas where standards of acceptable behavior are not bound by laws but by the more tenuous notion of professional responsibility. Some of these are:

1. Confidentiality. You should normally respect the confidentiality of your employers or clients irrespective of whether or not a formal confidentiality agreement has been signed.
2. Competence. You should not misrepresent your level of competence. You should not knowingly accept work that is outside your competence.
3. Intellectual property rights. You should be aware of local laws governing the use of intellectual property such as patents and copyright. You should be careful to ensure that the intellectual property of employers and clients is protected.
4. Computer misuse. You should not use your technical skills to misuse other people's computers. Computer misuse ranges from relatively trivial (game playing on an employer's machine, say) to extremely serious (dissemination of virus or other malware)


```
Software Engineering Code of Ethics and Professional Practice

ACM/IEEE-CS Joint Task Force on Software Engineering Ethics and Professional Practices

PREAMBLE
* The short version of the code summarizes aspirations of a high level of the abstraction; the clauses that are included in teh full version give examples and details of how these aspirations change the way we act as software engineering professionals. Without the aspirations, the details can become legalistic and tedious; without the details, the aspirations can be high sounding but empty; together the aspirations and the details for a cohesive code.
* Software engineers shall commit themselves to making the analysis, specification, design, development, testing and maintenance of software a beneficial and respected profession. In accordance with their commitment to the health, safety and welfare of the public, software engineers shall adhere to the following Eight Principle

1. PUBLIC--Software engineers shall act consistently with the public interest.
2. CLIENT AND EMPLOYER--Software engineers shall act in a manner that is in the best interests of their client and employer consistent with the public interest.
3. PRODUCT--Software engineers shall ensure that their products and related modifications meet the highest professional standards possible.
4. JUDGMENT--Software engineers shall maintain integrity and independence in their professional judgment.
5. MANAGEMENT--Software engineering managers and leaders shall subscribe to and promote an ethical approach to the management of software development and maintenance.
6. PROFESSION--Software engineers shall advance the integrity and reputation of the profession consistent with the public interest
7. COLLEAGUES--Software engineers shall be fair to and supportive of their colleagues.
8. SELF--Softwware engineers shall participate in lifelong learning regarding the practice of their profession and shall promote an ethical approach to the practice of the profession.
```

* Professional societies and institutions have an important role to play in setting ethical standards. Organizations such as the ACM, **the IEEE (institute of Electrical and Electronic Engineers)**, and the British Computer Society publish a code of professional conduct or code of ethics. Members of these organizations understake t ofollow that code when they sign up for membership. These codes of conduct are generally concerned with fundamental ethical behavior.
* Professional associations, notably the ACM and the IEEE, have cooperated to produce a joint code of ethics and professional practice. This code exists in both a short form, shown in Figure 1.3, and a longer form that adds detail and substance to the shorter version. The rationale behind this code is summarized in the first two paragraph of the longer form:

                Computers have a central and growing role in commerce, industry, government, medicine, education, entertainment and society at large. Software engineers are those who contribute by direct participation or by teaching, to the analysis, specification, design, development, certification, maintenance and testing of software system. Because of their roles in developing software systems, software engineers have significant opportunities to do good or cause harm, to enable others to do good or cause harm, or to influence others to do good or cause harm. To ensure, as much as possible, that their efforts will be used for good, software engineers must commit themselves to making software engineering a beneficial and respected profession. In accordance with that commitment, software engineers shall adhere to the following Code of Ethics and Professional Practice.

                The Code contains eight Principles related to the behavior of and decisions made by professional software engineers, including practitioners, educators, managers, supervisors, and policy makers, as well as trainees and students of the profession. The Principles identify the ethically responsible relationships in which individuals, groups, and organizations participate and the primary obligations within these relationships. The Clauses of each Principle are illustrations of some of the obligations included in these relationships. These obligations are founded in the software engineer's humanity, in special care owed to people affected by the work of software engineers, and the unique elements of the practice of software engineering. The Code prescribes these as obligations of anyone claiming to be or aspiring to be a software engineer.

* In any situation where different people have different views and objectives you are likely to be faced with ethical dilemmas. For example, if you disagree, in principle, with the policies of more senior management in the company, how should you react? Clearly, this depends on the particular individuals and the nature of the disagreement. Is it best to argue a case for your position from within the organization or to resign in principle? If you feel that there are problems with a software project, when do you reveal these to management? If you discuss these while they are just a suspicion, you may be overreacting to a situation; if you leave it too late, it may be impossible to resolve the difficulties.
* Such ethical dilemmas face all of us in our professional lives and, fortunately, in most cases they are either relatively minor or can be resolved without too much difficulty. Where they can not be resolved, the engineer is faced with, perhaps, another problem. The principled action may be to resign from their job but this may well affect others such as their partner or their children.
* A particular difficult situation for professional engineers arises when their employers acts in an unethical way. Say a company is responsible for developing a safety-critical system and, because of time pressure, falsifies the safety validation records. Is the engineer's responsibility to maintain confidentiality or to alert the customer or publicize, in some way, that the delivered system may be unsafe?
* The problem here is that there are no absolutes when it comes to safety. Although the system may not have been validated according to predefined criteria, these criteria may be too strict. The system may actually operate safely throughout its lifetime. It is also the case that, even when properly validated, the system may fail and cause an accident. Early disclosure of problems may result in damage to the employer and other employees; failure to disclose problems may result in damage to others.
* You must make up your own mind in these matters. The appropriate ethical position here depends entirely on the views of the individuals who are involved. In this case, the potential for damage, the extent of the damage, and the people affected by the damaage should influence the decision. If the situation is very dangerous, it may be justified to publicize it using the national press (say). However, you should always try to resolve the situation while respecting the rights of your employer.
* Another ethical issue is participation in the development of military and nuclear systems. Some people feel strongly about these issues and do not wish to participate in any systems development associated with military systems. Others will work on military systems but not on weapons systems. Yet others feel that national security is an overriding principle and have no ethical objections to working on weapons systems.
* In this situation, it is importan that both employers and employees should make their views known to each other in advance. Where an organization is invovled in military or nuclear work, they should be able to specify that employees must be willing to accept any work assignment. Equally, if an employee is taken on and makes clear that they do not wish to work on such systems, employers should not put pressure on them to do so at some later date.
* The general area of ethics and professional responsibility is becoming more important as software-intensive systems pervade every aspect of work and everyday life. It can be considered from philosopihcal standpoint where the basic principles of ethics are considered and software engineering ethics are discussed with reference to these basic principles. This is the approach taken by Laudon and to a lesser extent by Huff and Martin. Johnson's text on computer ethics also approaches the topic from a philosophical perspective.
* However, I find that this philosophical approach is too abstract and difficult to relate to everyday experience. I prefer the more concrete approach embodied in codes of conduct and practice. I think that ethics are best discussed in a software engineering context and not as a subject in their own right. In this book, therefore, I do not include abstract ethical discussions but, where appropriate, include examples in the exercises that can be the starting point for a group discussion on ethical issues.

## 1.3. Case studies
* To illustrate software engineering concepts, I use examples from three different types of systems throughout the book. The reason why I have not used a single case study is that one of the key messages in this book is that software engineering practice depends on the types of systems being produced. I therefore choose an appropriate example when discussing concepts such as safety and dependability, system modeling, reuse, etc.
* The three types of systems that I use as case studies are:

1. An embedded system. This is a system where the software controls a hardware device and is embedded in that device. Issues in embedded systems typically include physical size, responsiveness, power management, etc. The example of an embedded system that I use is a software system to control a medical device.
2. An information system. This is a system whose primary purpose is to manage and provide access to a database of information. Issues in information systems include security, usability, privacy, and maintaining data integrity. The example of an information system that I use is a medical records system.
3. A sensor-based data collection system. This is a system whose primary purpose is to collect data from a set of sensors and process that data in some way. The key requirements of such systems are reliability, even in hostile environmental conditions, and maintainability. The example of a data collection system that I use is a wilderness weather station.

* I introduce each of these systems in this chapter, with more information about each of them available on the Web.

#### 1.3.1. An insulin pump control system
* An insulin pump is a medical system that simulates the operation of the pancreas (an internal organ). The software controlling this system is an embedded system, which collects information from a sensor and controls a pump that delivers a controlled dose of insulin to a user.
* People who suffer from diabetes use the system. Diabetes is a relatively common condition where the human pancreas is unable to produce sufficient quantities of a hormone called insulin. Insulin metabolises glucose (sugar) in the blood. The conventional treatment of diabetes involves regular injections of genetically engineered insulin. Diabetics measure their blood sugar levels using an external meter and then calculate the dose of insulin that they should inject.
* The problem with this treatment is that the level of insulin required does not just depend on the blood glucose level but also on the time of the last insulin injection. This can lead to very low levels of blood glucose (if there is too much insulin) or very high levels of blood sugar (if there is too little insulin). Low blood glucose, in the short term, a more serious condition as it can result in temporary brain malfunctioning and, ultimately, unconsciousness and death. In the long term, however, continual high level of blood glucose can lead to eye damage, kidney damage, and heart problems.
* Current advances in developing miniaturized sensors have meant that it is now possible to develop automated insulin delivery systems. These systems monitor blood sugar levels and deliver an appropriate dose of insulin when required. Insulin delivery systems like this already exist for the treatment of hospital patients. In the future, it may be possible for many diabetics to have such systems permanently attached to their bodies.
* A software-controlled insulin delivery system might work by using a microsensor embedded in the patient to measure some blood parameter that is proportional to the sugar level. This is then sent to the pump controller. This controller computes the sugar level and the amount of insulin that is needed. It then sends signals to a miniaturized pump to deliver the insulin via a permanently attached needle.
* Figure 1.4 shows the hardware components and organization of the insulin pump. To understand the examples in this book, all you need to know is that the blood sensor measures the electrical conductivity of the blood under different conditions and that these values can be related to the blood sugar level. The insulin pump delivers one unit of insulin in response to a single pulse from a controller. Therefore, to deliver 10 units of insulin, the controller sends 10 pulses to the pump. Figure 1.5 is a UML activity model that illustrates how the software transforms an input blood sugar level to a sequence of commands that drive the insulin pump.
* Clearly, this is a safety-critical system. If the pump fails to operate or does not operate correctly, then the user's health may be damaged or they may fall into a coma because their blood sugar levels are too high or too low. There are, therefore, two essential high-level requirements that this system must meet:

                1. The system shall be available to deliver insulin when required.
                2. The system shall perform reliably and deliver the correct amount of insulin to counteract the current level of blood sugar.

* The system must therefore be designed and implemented to ensure that the system always meets these requirements. More detailed requirements and discussions of how to ensure that the system is safe are discussed in later chapters.

#### 1.3.2 A patient information system for mental health care
* A patient information system to support mental health care is a medical information system that maintains information about patients suffering from mental health problems and the treatments that they have received. Most mental health patients do not require dedicated hospital treamtn but need to attend specialst clinic regularly where they can meet a doctor who has detailed knowledge of their problems. To make it easier for patients to attend, these clinic are not just run in hospitals. They may also be held in local medical practices or community centers.
* The MHC-PMS (Mental Health Care-Patient Management System) is an information system that is intended for use in clinic. It makes use of a centralized database of patient information but has also been designed to run on a PC, so that it may be accessed and used from sites that do not have secure network connectivity. When the local system have secure network access, they use patient information in the database but they can download and use local copies of patient records when they are disconnected. The system is not a complete medical records system dso does not maintain information about other medical conditions. However, it may interact and exchange data with other clinical information systems. Figure 1.6 illustrates the organization of the MHC-PMS.
* THe MHC-PMS has two overall goals:

                1. To generate management information that allows health service managers to assess performance against local and government targets.
                2. To provide medical staff with timely information to support the treatment of patients.


* The nature of mental health problems is such that patients are often disorganized so may miss appointments, deliberately or accidentally lose prescriptions and medication, forget instructions, and make unreasonable demands on medical staff. They may drop in on clinics unexpectedly. In a minority of cases, they may be a danger to themselves or to other people. They may regularly change address or may be homeless on a long-term or short-term basis. Where patients are dangerous, they may need to be "sectioned"--confined to a secure hospital for treatment and observation.
* Users of the system include clinical staff such as doctors, nurses, and health visitors (nurses who visit people at home to check on their treatment). Nonmedical users include receptionists who make appointments, medical records staff who maintain the records system, and administrative staff who generate reports.
* The system is used to record information about patients (name, address, age, next of kin, etc), consultations (date, doctor seen, subjective impressions of the patient, etc), conditions and treatments. Reports are generated at regular intervals for medical staff and health authority managers. Typically, reports for medical staff focus on information about individual patients whereas management reports are anonymized and are concerned with conditions, costs of treatment, etc.
* The key features of the system are:

1. Individual care management. Clinicians can create records for patients, edit the information in the system, view patient history, etc. The system supports data summaries so that doctors who have not previously met a patient can quickly learn about the key problems and treatments that have been prescribed.
2. Patient monitoring. The system regularly monitors the records of patients that are involved in treatment and issues warnings if possible problems are detected. Therefore, if a patient has not seen a doctor for some time, a warning may be issued. One of the most important elements of the monitoring system is to keep track of patients who have been sectioned and to ensure that the legally required checks are carried out at the right time.
3. Administrative reporting. The system generates monthly management reports showing the number of patients treated at each clinic, the number of patients who have entered and left the care system, number of patients sectioned, the drugs prescribed and their costs, etc.

* Two different laws affect the system. These are laws on data protection that govern the confidentiality of personal information and mental health laws that govern the compulsory detention of patients deemed to be a danger to themselves or others. Mental health is unique in this respect as it is the only medical speciality that can recommend the detention of patients against their will. This is subject ot very strict legislative safeguards. One of the aims of the MHC-PMS is to ensure that staff always act in accordance with the law and that their decisions are recorded for judicial review if necessary.
* As in all medical systems, privacy is a critical system requirement. It is essential that patient information is confidential and is never disclosed to anyone apart from authorized medical staff and the patient themselves. The MHC-PMS is also a safety-critical system. Some mental illnessess cause patients to become suicidal or a danger to other people. Wherever possible, the system should warn medical staff about potentially suicidal or dangerous patients.
* The overall design of the system has to take into account privacy and safety requirements. The system must be available when needed otherwise safety may be compromised and it may be impossible to prescribe the correct medication to patients. There is a potential conflict here--privacy is easiest to maintain when there is only a single copy of the system data. However, to ensure availability in the event of server failure or when disconnected from a network, multiple copies of the data should be maintained. I discuss the trade-offs between these requirements in later chapters.

#### 1.3.3 A wilderness weather station
* To help monitor climate change and to improve the accuracy of weather forecasts in remote areas, the government of a country with large areas of wilderness decides to deploy several hundred weather stations in remote areas. These weather stations collect data from a set of instruments that measure temerature and pressure, sunshine, rainfall, wind speed, and wind direction. 
* Wilderness weather stations are part of a large system, which is a weather information system that collect data from weather stations and makes it available to other systems for processing. The systems in Figure 1.7 are:

1. The weather station system. This is responsible for collecting weather data, carrying out some initial data processing, and transmitting it to the data management system.
2. The data management and archiving system. This system collects the data from all of the wilderness weather stations, carries out data processing and analysis, and archives the data in a form that can be retrieved by other systems, such as weather forecasting systems.
3. The station maintenance system. This system can communicate by satellite with all wilderness weather stations to monitor the health of these systems and provide reports of problems. It can update the embedded software in these systems. In the event of system problems, this system can also be used to remotely control a wilderness weather system.
* In Figure 1.7, I have used the UML package system to indicate that each system is a collection of components and have identified the separate systems, using the UML stereotyp <<system>>. The association betwteen the packages indiciate there is an exchange of information but, at this stage, there is no need to define them in any more detail.
* Each weather station includes a number of instruments that measure weather parameters such as the wind speed and direction, the ground and air temperatures, the barometric pressure, and the rainfall over a 24-hour period. Each of these instruments is controlled by a software system that takes parameter readings periodically and manages the data collected from the instruments.
* The weather station system operates by collecting weather observations at frequent intervals--for example, temperatures are measured every minutes. However, because the bandwidth to the satellite is realtively narrow, the weather station carries out some loccal processing and aggregation of the data. It then transmits this aggregated data when requested by the data collection system. If, for whatever reason, it is impossible to make a connection, then the weather station maintains the data locally until communication can be resumed.
* Each weather station is battery-powered and must be entirely self-contained--there are no external power or network cables available. All communications are through a relatively slow-speed satellite link and the weather station must include some mechanism (solar or wind power) to charge its batteries. As they are deployed in wilderness areas, they are exposed to severe environmental conditions and may be damaged by animals. The station software is therefore not just concerned with data collection. It must also:

1. Monitor the instruments, power, and communication hardware and report faults to the management system.
2. Manage the system power, ensuring the batteries are charged whenever the environmental conditions permit but also that generators are shut down in potentially damaging weather conditions, such as high wind.
3. Allow for dynamic reconfiguration where parts of the software are replaced with new versions and where backup instruments are switched into the system in the even of system failure.

* Because weather stations have to be self-contained and unattended, this means that the software installed is complex, even though the data collection functionality is fairly simple.

# Chapter 2: Software Processes




page 27



















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
