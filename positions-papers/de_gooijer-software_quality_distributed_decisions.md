# Software Quality through Distributed Decision Making
Thijmen de Gooijer (thijmen@acm.org), IT Architect at Kommuninvest, Örebro (Sweden)
Submission to the SATURN 2019 workshop: Architecture Island, May 6th, 2019 in Pittsburgh, PA, USA.

_Disclaimer: the views expressed in this position paper are my own and do not reflect those of my employer._

## Why Software Architecture?
### Indispensable to progress and productivity
Software is easy to copy and reuse. Every developer reuses code in the form of libraries whether open source, commercial SDK or earlier internal work. More and more software services are commodities sold as subscriptions: cloud services. Yet, we spend a lot of time writing programs for unique problems. Planning software development through software architecture means teams can make progress on complex system development despite dependencies on cloud services, code libraries, and other teams.

### Important for sustainable systems
As long as the organization lives, software evolves. Software development is never "done". Not only because needs change but also because the understanding of the needs improves with time. Unfortunately, it is difficult to change the domain and data models that describe these needs once embodied in the software. It is through both up-front and continuous work with the software architecture that we can create systems that can adapt to change.

Many systems live increasingly long lives, which means that technology advances quicker than software systems retire. Software architects guide their teams and organizations in decisions that help adapt new technology. Architects steer clear of the latest hype and limit unnecessary creativity among developers but enable the system to embrace shifts that benefit the users. 

### Unique communication challenge
The job of a software architect is as much a social role as a technical one. Grounded in the reality of code on one end and in the abstract ideas of future endeavors on the other. The work requires the ability to think systematically using abstractions and communicate these through models. Reasoning about impact of technology choices, future business ideas, and facts created by decisions from the past. The architect uses a mathematical mind to reason about the impact of the CAP theorem, time, and cryptography; and a social skill to communicate with the stakeholders in the system.

##  Teams Own Architectures, Architects Coach Teams
The philosophy of my own architecture practice is that everybody on the team contributes to the architecture. Everybody is an architect: developers, requirements engineers, UX designers, product owners. The architect's job is to bring all these different disciplines together to create and implement a sustainable architecture. The architect coaches the team to work within the constraints of the chosen technologies to deliver the quality properties that stakeholders need. Therefore, I believe in providing guiding principles for distributed decision making, rather than writing proverbial clay tablets to pass from the mountain top with decrees on how things shall be. The challenge is of course to equip others with the core knowledge to make the right design decisions. 

## Software Architecture Core Knowledge

### What do software architects create?
Software architects make design decisions to create sustainable software systems. The design decisions encode trade-offs among conflicting quality attributes. The decisions direct to use a certain technology, algorithm, data structure, etcetera, over another one that exhibits different properties. Unfortunately, many of these trade-offs are wicked problems without a single ideal or optimal solution.
>**Concept 1** Software architectures strife to implement desired quality attributes and reduce undesired qualities.

>**Idea 1** Software architecture is a decision making practice. Architects decide on trade-offs among quality attributes.

>**Idea 2** Most systems cannot exhibit all or even many qualities at once.

### How are architecture tasks defined and delimited?
Conceptual or abstract models help architects create boundaries among software parts that do not exist yet. These boundaries typically are around components or microservices. We want data and logic inside a boundary to be cohesive and have only loose coupling to other data and logic outside of it. Different ways of setting these boundaries exist and architects should know at least a couple. Simon Brown's C4 models set boundaries around containers or units of code that one can deploy independently of another. Technical people easily relate to setting boundaries in this way. Domain-driven design sets boundaries based on concepts from the problem domain. Domain concepts often have names and structures that are familiar to non-technical stakeholders. Data-flow diagrams, state machines, and process models give us yet other ways to delimit boundaries.

>**Method 1** Context to code decomposition with the C4 model.

>**Method 2** Domain-driven design.

>**Concept 2** Modeling of logic and information flows.

Goals for the software architecture are expressed in quality requirements. The architect's task is to try to maximize fulfillment of these requirements. Quality requirements are only useful or satisfiable when expressed rather precisely. A system cannot have good performance but can serve requests with a maximum latency of two seconds. Architects should therefore be familiar with one or more ways to define quality requirements, for example quality attribute scenarios.

>**Method 3** Quality attribute scenarios

### How do architects prioritize their tasks?
Eltjo Poort tied together the notions of risk and cost for focusing the architect's attention. Both concepts have been mentioned multiple times before. George Fairbanks wrote about risk as an important factor in his book "Just Enough Software Architecture". Grady Booch defined architectural decisions as those costly to change. Just to give two earlier examples. Architects may find it challenging to put exact numbers on risk and costs involved in construction of a component or a specific decision, but often an approximation will be good enough to help focus the attention.

>**Strategy 1** Risk and cost-driven architecture

### How do architects produce and communicate results?
Just like software code, architectures often benefit from iterative improvement of their design. Ideally, iteration can happen before committing to a decision. There are many ways to find flaws in design decisions, for example, analyzing models, and implementation of prototypes. More mature designs benefit from structured analysis for example by applying the ATAM (Architecture Trade-Off Analysis Method).

>**Method 4** Iterative design

>**Method 5** Architecture analysis with ATAM

While an architect can perform analysis, preparation and other creative tasks alone, it is important to engage with stakeholders throughout the design process. Early in the process the architect has to discover and understand requirements, later in the process developers have to become familiar with the design to implement it. Certain costly or risky decisions can have a big impact and require that the architect communicates about these with senior leaders in the organization. Gregor Hophe aptly called this riding the architect elevator. In my own practice I touch code (albeit less frequently than I'd like) and report to the executive committee and the board of our organization. Architects have to be organizational polyglots to successfully deliver an architecture.

>**Strategy 2** Riding the architecture elevator


## Contemplation Questions
While writing this paper, many questions came to me about things I didn't touch upon, was uncertain about, question, or don't know. I want to share the following, each with a short explanation. The questions hint at my own doubts about the position I take in the paper.

### What is the goal of software architecture?
Put differently, why do we practice software architecture? And, what things other than quality attributes define software architecture? Some of my answers:
	- Enable future speed of development by timely design decisions
	- Limit (future) technical debt through design decisions
	- Improve or maintain the quality of software through timely design decisions
Can we formulate a precise and single goal?

### What is the difference between software architecture and engineering?
What defines a software engineer? Do we want to separate software engineers and developers, or are they the same profession and do they have the same skill level? These questions came up as I pondered about:
- Do design patterns differ substantially between software engineering and software architecture?

### What is the relation between software architecture and computer architecture?
Computer architecture is to a large extend about hardware. I wonder though whether we can define such a clear distinction when software depends on hardware and hardware get loaded with more and more 'firmware' and 'microcode' which seem just other words for software.
