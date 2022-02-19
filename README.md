## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/zapper163/Tech-Design-Document/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.



# TECH DESIGN DOCUMENT (TDD)

### General Info
A technical design doc describes a solution to a given technical problem. It is a specification, or “design blueprint”, for a software program or feature.
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

### Title TDD
Author: Your Name

### **Introduction**
### Rationale
What are you trying to accomplish? What’s wrong with things the way they are now?
### Background
Describe any historical context that would be needed to understand the document, including legacy considerations.
### Terminology
If the document uses any special words or terms, list them here.
### Non-Goals
If there are related problems that you have decided not to address with this design, but which someone might conceivably expect you to solve, then list them here.
### Proposed Design
Start with a brief, high-level description of the solution. The following sections will go into more detail.
### System Architecture
If the design consists of a collaboration between multiple large-scale components, list those components here — or better, include a diagram.
### Data Model
Describe how the data is stored. This could include a description of the database schema.
### Interface/API Definitions
Describe how the various components talk to each other. For example, if there are REST endpoints, describe the endpoint URL and the format of the data and parameters used.
### Business Logic
If the design requires any non-trivial algorithms or logic, describe them.
### Migration Strategy
If the design incurs non-backwards-compatible changes to an existing system, describe the process whereby entities that depend on the system are going to migrate to the new design.
### Impact
Describe the potential impacts of the design on overall performance, security, and other aspects of the system.
### Risks
If there are any risks or unknowns, list them here. Also if there is additional research to be done, mention that as well.
### Alternatives
If there are other potential solutions which were considered and rejected, list them here, as well as the reason why they were not chosen.




























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

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/zapper163/Tech-Design-Document/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
