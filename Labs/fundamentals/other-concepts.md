# Other concepts

This section overviews Agile & Scrum, SRE, DevSecOps, Platform Engineering and Cloud Engineering.

## Agile

Agile is an iterative approach to project management and software development that focuses on collaboration, customer feedback, and rapid releases. It arose in the early 2000s from the software development industry, helping development teams react and adapt to changing market conditions and
customer demands.

In an agile approach, some planning and design is done upfront, but the development proceeds in small batches and involves close collaboration with stakeholders. Changes are incorporated continuously and a usable version of a product is often released quicker compared to products developed through the waterfall methodology. This provides many benefits, with arguably the most important being that if software doesn’t meet the needs or expectations of the customer, it can be remediated in real-time.

Agile is a collection of methodologies, not a single approach to development. It is an aggregation of scrum, eXtreme Programming (XP), and other systems of practice that developers used in years prior, and resulted from those practitioners coming together to unify these approaches into a single set of principles. The result of this unification effort was the Agile Manifesto, which consists of 12 principles, based on four core values:

!!! info "The Agile Manifesto’s four core values"
    1. Individuals and interactions - over processes and tools
    2. Working software - over comprehensive documentation
    3. Customer collaboration - over contract negotiation
    4. Responding to change - over following a plan

!!! quote "Agile Principles"

    **The values are based on these principles:**

    1. Customer satisfaction by early and continuous delivery of valuable software.
    2. Welcome changing requirements, even in late development.
    3. Deliver working software frequently (weeks rather than months).
    4. Close, daily cooperation between business people and developers.
    5. Projects are built around motivated individuals, who should be trusted.
    6. Face-to-face conversation is the best form of communication (co-location).
    7. Working software is the primary measure of progress.
    8. Sustainable development, able to maintain a constant pace.
    9. Continuous attention to technical excellence and good design.
    10. Simplicity—the art of maximizing the amount of work not done—is essential.
    11. Best architectures, requirements, and designs emerge from self-organizing teams.
    12. Regularly, the team reflects on how to become more effective, and adjusts accordingly.

**Enter DevOps** - DevOps is an approach to software development that enables teams to build, test, and release software faster and more reliably by incorporating agile principles and practices, such as increased automation and improved collaboration between development and operations teams. Development, testing, and deployment occur in both agile and DevOps. Yet traditional agile stops short of operations, which is an integral part of DevOps.

### Scrum

Scrum prescribes for teams to break work into goals to be completed within time-boxed iterations, called sprints. Each sprint is no longer than one month and commonly lasts two weeks. The scrum team assesses progress in time-boxed, stand-up meetings of up to 15 minutes, called daily scrums. At the end of the sprint, the team holds two further meetings: one sprint review to demonstrate the work for stakeholders and solicit feedback, and one internal sprint retrospective. A person in charge of a scrum team is typically called a scrum master.

## SRE - Site Reliability Engineering

SRE is a discipline in the field of Software Engineering and IT infrastructure support that monitors and improves the availability and performance of deployed software systems and large software services. There is typically a focus on automation and an infrastructure as Code methodology.

!!! note "SRE vs DevOps"
    SRE is considered a specific implementation of DevOps;[14] focusing specifically on building reliable systems, whereas DevOps covers a broader scope of operations.

### SLA (Service Level Agreement)

SLA is a commitment between service provider and customer. SLA is expressed as
percentage % of availability/error, how often the system is up and how often it's down. Very few services need 100% SLA, Achieving it is difficult and expensive. SLA usually defined by the number of 9s ("4 nines": 99.99%).

Engineers and business people who are the end users decides how much downtime is acceptable or how many requests must be successful, according to market benchmarks, user feedbacks, competition, etc...

Engineers will define SLAs on technical level and integrate them into DevOps & SRE processes, while business people will define SLAs on a higher level.

## DevSecOps

