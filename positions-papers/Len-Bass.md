Position paper for SATURN workshop on software architecture design

Len Bass

I am interpreting the workshop call as asking the question “what knowledge should a software
architect have to do good design?”

My position is that an architect needs a good understanding of five things:

1. The environment in which their system is intended to run. For cloud based systems this is an
understanding of distributed system principles, virtualization, networking, containerization,
failure in the cloud, and security. They don’t need deep expertise in these areas, but they
need more than casual knowledge. In particular, they need to know how the environment
will affect the system they are designing.

2. Architectural design principles. These are: quality attribute requirements drive design
choices, business goals lead to quality attribute requirements, and design choices are
constrained by the environment and by business considerations. Implied in this is an
understanding of quality attributes and the business for which the system is being built.

3. Processes to make the design principles concrete. Translating an architectural design
principle into a design repeatedly requires a process. Knowing that quality attributes drive
design does not get you a design. What it gets you are a series of questions: what are the
important quality attribute requirements, what are the options for realizing those
requirements, and what are the trade offs among the requirements that result from these
options? A process provides a structure for asking these questions and processing the
responses.

4. Architectural styles. Systems are not derived from first principles. Knowing the strengths and
weaknesses of various architectural styles allows the designer to take advantage of the
experiences of the field. Staying with cloud based systems, the designer must have
knowledge of microservice architecture. The designer must also understand the role of state
and its maintenance within different components of the system.

5. The tools to be used in the development, deployment, and forensic processes. Current tool
suites have the side effect of deskilling software engineers. To paraphrase a respected
member of our community: “I don’t need to understand containers, I write my function and
the tool chain takes care of containerization and what that entails”. Software architects
must understand the tool suite and their characteristics. Current key tools are Kubernetes
for packaging, deploying and scaling containers, protocol buffers for supporting message
based systems and generating logs used in forensics, and configuration management tools
for maintaining consistency among a fleet of servers.
