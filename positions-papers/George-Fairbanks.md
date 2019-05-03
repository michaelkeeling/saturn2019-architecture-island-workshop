# What are the big ideas in software architecture?

George Fairbanks

3 May 2019

In this workshop, we'll be discussing which ideas about software architecture we'd keep and 
which ones we'd be forced to abandon as we confront the dangers on Architecture Island (rather 
like the TV show Survivor).  It seems like a good idea to survey some of the most popular books 
on software architecture to create an inventory of what ideas we are starting with.  

I intended to survey about a dozen books but it took more time than I’d expected so I (so far) 
have only done two plus my [Intro to Software Architecture lecture](https://www.georgefairbanks.com/blog/cu-boulder-intro-to-software-architecture-video/) from 2012.  For this workshop, 
any list is better than no list, but I’d find it interesting to see which ideas span all or most 
of the books on software architecture.

I picked up [Documenting Software Architectures (2nd edition)](https://www.amazon.com/Documenting-Software-Architectures-Views-Beyond/dp/0321552687) first as I remembered it as being 
much like a catalog itself.  I skimmed the book and jotted down ideas or topics.  There’s a fair 
amount of bias in this activity: in my haste I may not have noticed an idea, a different reader 
might notice different ideas, and of course names differ across books and I was trying to align 
them while jotting down notes.  Then I did the same for [Software Architecture in Practice (3rd 
edition)](https://www.amazon.com/Software-Architecture-Practice-3rd-Engineering/dp/0321815734) 
and my intro lecture.  I merged those lists into a table, doing some more subjective 
merging and omitting of topics.  If by chance any of the workshop participants notice errors or 
omissions (I’m looking at you Len Bass) then please let me know and I’ll fix up the table.


Notation:  A question mark in the table indicates that I don’t think the topic was covered but 
I wouldn’t be surprised if I’d overlooked it.  The asterisk in the table is meant to be a bullet
that nests under the line above, but my efforts to make it render that way have not yet worked.


I included that intro lecture not because it’s in the same league as the two books but because as 
of 2012 it was my idea of what I’d keep on Architecture Island and I was curious what I’d left out. 



|Topic                                                                                                | DSA 2nd Edition | SAP 3rd Edition | Intro to SA |
|------------------------------------------------------------------------------------------------------|:---------------:|:---------------:|:-----------:|
| Views (module, C&C / Runtime, Allocation)                                                            |       Yes       |       Yes       |     Yes     |
| * Master model unifies views                                                                         |        No       |        No       |     Yes     |
| Stakeholders                                                                                         |       Yes       |       Yes       |      No     |
| Quality attributes (vs functionality)                                                                |       Yes       |       Yes       |     Yes     |
| * Architecture inhibits or enables                                                                   |       Yes       |       Yes       |     Yes     |
| * Tied to failure risks                                                                              |        ?        |        ?        |     Yes     |
| Requirements: QA vs feature                                                                          |       Yes       |       Yes       |     Yes     |
| * QA requirements drive architecture                                                                 |       Yes       |       Yes       |     Yes     |
| * QA scenarios                                                                                       |        No       |       Yes       |     Yes     |
| * Argument: How this architecture meets requirements                                                 |       Yes       |        No       |      No     |
| * Architecturally significant requirements (ASRs)                                                    |        ?        |       Yes       |     Yes     |
| Architecture is a subset of design                                                                   |       Yes       |        ?        |     Yes     |
| Contexts: Technical, lifecycle, business, professional                                               |        No       |       Yes       |      No     |
| Architectural styles / patterns                                                                      |       Yes       |       Yes       |     Yes     |
| * Module style: decomposition, uses, generalization, layers, aspects, data model                     |       Yes       |        No       |      No     |
| * Runtime style: pipe and filter, client-server, peer-to-peer, SOA, pub-sub, shared-data, multi-tier |       Yes       |        No       |      No     |
| * Allocation: deployment, install, work assignment                                                   |       Yes       |        No       |      No     |
| Tactics                                                                                              |        No       |       Yes       |      No     |
| * Attribute driven design                                                                            |        No       |       Yes       |      No     |
| Architecture diagrams (vs cartoons)                                                                  |       Yes       |        ?        |      No     |
| Notaions and ADLs: element catalog                                                                   |       Yes       |        No       |      No     |
| Product line architectures                                                                           |       Yes       |       Yes       |      No     |
| Architectural decisions                                                                              |       Yes       |        ?        |      No     |
| * Rational architecture decisions                                                                    |        No       |        No       |     Yes     |
| Interfaces: provided and required                                                                    |       Yes       |        No       |      No     |
| Design reviews                                                                                       |       Yes       |       Yes       |      No     |
| Align architecture and business goals                                                                |        No       |       Yes       |      No     |
| Tradeoffs (and ATAM)                                                                                 |        No       |       Yes       |     Yes     |
| Separate: Architecture, architects, architecting                                                     |        No       |       Yes       |     Yes     |
| Constraints / guiderails                                                                             |       Yes       |       Yes       |     Yes     |
| Conceptual model of architecture                                                                     |       Yes       |       Yes       |     Yes     |
| Architecturally evident coding style                                                                 |        No       |        No       |     Yes     |
| Architectural hoisting                                                                               |        No       |        No       |      No     |
