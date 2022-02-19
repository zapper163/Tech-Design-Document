## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/zapper163/Tech-Design-Document/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.



# TECH DESIGN DOCUMENT (TDD)

[How to write a better technical design document](https://www.range.co/blog/better-tech-specs)<--Mirar

[How to write technical design docs](https://dev.to/mage_ai/how-to-write-technical-design-docs-c02)
### General Info

A Technical Design Document (TDD) is written by the development team and describes the minute detail of either the entire design or specific parts of it, such as:

- The signature of an interface, including all data types/structures required (input data types, output data types, exceptions)
- Detailed class models that include all methods, attributes, dependencies, and associations
- The specific algorithms that a component employs and how they work
- Physical data models that include attributes and types of each entity/data type

In short, the functional design specifies how a program will behave to outside agents and the technical design describes how that functionality is to be implemented in code. The Technical Design Document must be approved by the IT project sponsor before proceeding to the development/integration phase.
A technical design doc describes a solution to a given technical problem. It is a specification, or “design blueprint”, for a software program or feature.

[Source](https://uit.stanford.edu/pmo/technical-design)


The primary function of a TDD is to communicate the technical details of the work to be done to members of the team.

However, there is a second purpose which is just as important: the process of writing the TDD forces you to organize your thoughts and consider every aspect of the design, ensuring that you haven’t left anything out.

Technical design docs are often part of a larger process which typically has the following steps:
1. **Product requirements are defined**
These will typically be represented by a Product Requirements Document (PRD). The PRD specifies what the system needs to do, from the perspective of a user or outside agent.

2. **Technical requirements are defined**
The product requirements are translated into technical requirements — what the system needs to accomplish, but now how it does it. The output of this step is a Technical Requirements Document (TRD).

3. **Technical design**
This contains a technical description of the solution to the requirements outlined in the previous steps. The TDD is the output of this step.

4. **Implementation**
This is the stage where the solution is actually built.

5. **Testing**
The system is tested against the PRD and TRD to ensure that it actually fulfills the specified requirements.

Between each of these stages there is typically a review process to ensure that no mistakes were made. If any errors, misunderstandings, or ambiguities are detected, these must be corrected before proceeding to the next step.

This process is highly variable; the set of steps listed here will change on a case-by-case basis. For example:
For smaller features that don’t involve a lot of complexity, steps 2 and 3 will often be combined into a single document.
If the feature involves a large number of unknowns or some level of research, it may be necessary to construct a proof-of-concept implementation before finalizing the technical design.

This process also happens at different scales and levels of granularity. A PRD / TRD / TDD may concern the design of an entire system, or just a single feature. In most environments, the process is also cyclic — each design/implement cycle builds on the work of the previous one.

[Source](https://medium.com/machine-words/writing-technical-design-docs-71f446e42f2e)


## TDD Template

1. **Description of the Problem**
Give a brief (one paragraph) summary of the problem you are solving. Work to keep away from technical detail. Try instead to talk about this in terms of the problem as it pertains to your customers. At the end of reading this document, any team member should be able to understand the problem, how you intend to solve it, and who are the stakeholders.

2. **Solution Requirements**
Briefly describe what is required of a solution which addresses the problem. Try to steer clear of the how (implementation detail) and concentrate on what is required any solution in order to address the problem outlined above.

3. **Glossary**
Link to the service wide glossary, and define any new terms used in this document.

4. **Out of Scope (Non-goals)**
Explicitly call out what is not in scope (Sometimes articulating what you are not going to do is an easier way to define scope than to talk about what you are going to do.)

5. **Assumptions**
What are you assuming will be true or in place to make your solution successful?

6. **Solution**
Your solution goes here.

Start by including a high level diagram and decompose from there. Please diagram (where possible) how your solution interacts with other subsystems and services (including sequence diagrams for complex interactions).

Aim to answer:
- What are you going to deliver?
- What are your upstream and downstream dependencies?
- How does it fit in to the broader service?
- How will it scale?
- What are the limits of your solution?
- How will you ensure fault tolerance and quick recovery after failure?
- How might your solution evolve to meet future requirements?

7. **Security Considerations**
What are the security implications of your solution? If your solution is large enough in scope to warrant its own threat model, please add it here, otherwise please describe how your solution impacts existing threat models.

8. **Cost Analysis**
A high level analysis of the costs that will be incurred in running your chosen solution on a day-to-day basis.

9. **Cross-region Considerations**
If applicable, how does your solution optimize or is compatible with cross-region requirements. This includes data transfer costs between regions, availability of the service in different data centers, latency issues, etc.

10. **Operational Readiness Considerations**
Discuss how your solution will support operational excellence, ensuring customer satisfaction with a frugal level of support.

Aim to answer:
- How your chosen solution will be deployed?
- What metrics and alarms will be key to monitoring the health of your solution?
- How are your solution limits enforced?
- Will there be any throttling or blacklisting mechanisms in place?
- Will there be any data recovery mechanisms in place?
- If this is a multi-tenant solution, how are you dealing with noisy neighbor issues?
- How will your solution be debugged when problems occur?
- How will your solution recover in case of a brown-out?
- Are there any operational tools required for your solution?

11. **Risks and Open Issues**
If there are any risks or unknowns, list them here. Are there any open questions which could impact your design for which you do not currently have answers? How are you going to get answers? Will any required team members be loaned to other teams during the time slated for implementation? Are all of required dependencies available in all the regions you need them? What are the one way doors, and are we sure we want to go through them?
12. **Solutions considered and discarded**
What alternatives have you have considered and discarded? Why don’t these work? Be brief, linking to other documents for details is ok, but always provide a summary inline.
Only alternative solutions that an impartial observer would deem credible need be documented.
If an alternative solution is not appropriate now, but may be in the future, please discuss potential migration paths.

13. **Work Required**
Include a high level breakdown of the work required to implement your proposed solution where appropriate. Also, specifically call out if this solution requires resources from other teams to be completed (away teams, dependencies etc.)

14. **High-level Test Plan**
At a high level, describe how your chosen solution be tested.

15. **References**
Links to any other documents that may be relevant, or sources you wish to cite.


























### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).
