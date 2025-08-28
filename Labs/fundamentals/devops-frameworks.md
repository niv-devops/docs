# DevOps Framework

Like every movement or philosophy, DevOps frameworks guide practitioners to implement the practices effectively and efficiently.

## CALMS Framework

The CALMS Framework (Culture, Automation, Lean, Measurement, Sharing) assesses a company's ability to adopt DevOps and measures success during transformation.

!!! info "Culture"
	- DevOps is a culture change focused on collaboration.
	- Product-oriented teams (development, QA, product management, design, operations, etc.) work together.
	- Collaboration is fostered by sharing goals and planning together.
	- Incident post-mortems focus on improvement, not blame.
	- DevOps is everyone's job, not just one team's.

!!! tip "Automation"
	- Eliminates manual work, creates reliable systems, and enables repeatable processes.
	- Start with build, test, deploy, and provisioning automation.
	- Continuous delivery and configuration as code break down barriers between development and operations.
	- Automated deployments and tests catch bugs and security flaws early.

!!! note "Lean"
	- Focus on continuous improvement and embracing failure.
	- Hold regular retrospectives and experiment with new approaches.
	- Failure is inevitable; build for fast detection and recovery.
	- Postmortems strengthen processes, not punish individuals.

!!! info "Measurement"
	- Use data to prove improvement and guide decisions.
	- Start with basics: time to deploy, bug frequency, recovery time, user metrics.
	- Share metrics across teams to build consensus and support roadmaps.

!!! tip "Sharing"
	- DevOps transformation requires practices, culture, and tools.
	- Sharing responsibility and success bridges the gap between development and operations.
	- "You build it, you run it" (YBIYRI) encourages hands-on collaboration.
	- Peer-reviewed code and rotating support roles build trust and mutual respect.


### You Build It, You Run It (YBIYRI)

- The phrase "you built it, you run it" fosters a hands-on approach across teams.
- Developers and operators pair throughout the application lifecycle, not just as separate roles.
- Peer-reviewed code and products lead to better delivery and performance.
- Rotating support roles help developers address urgent customer issues and learn how the application is used in the wild.
- High availability and collaboration between development and operations build trust and mutual respect.

## DevOps Metrics

DevOps practitioners rely on four key metrics, developed by DORA, to measure the efficacy of their DevOps practices.

DevOps metrics are data points that directly reveal the performance of a DevOps software
development pipeline and help quickly identify and remove any bottlenecks in the process.

These metrics can be used to track both technical capabilities and team processes.
At its core, DevOps focuses on blurring the line between development and operations teams, enabling greater collaboration between developers and system administrators.

Metrics allows DevOps teams to measure and assess collaborative workflows and track progress of achieving high-level goals including increased quality, faster release cycles, and improved application performance.

### Four critical DevOps metrics

Though there are numerous metrics used to measure DevOps performance, the following are four key metrics every DevOps team should measure.

1. **Lead time for changes** - The length of time between when a code change is committed to the trunk branch and when it is in a deployable state. For example, when code passes all necessary pre-release tests.

2. **Change failure rate** - The change failure rate is the percentage of code changes that require hot fixes or other remediation after production. This does not measure failures caught by testing and fixed before code is deployed.

3. **Deployment frequency** - Understanding the frequency of how often new code is deployed into production is critical to understanding DevOps success. Many practitioners use the term “delivery” to mean code changes that are released into a pre-production staging environment, and reserve “deployment” to refer to code changes that are released into production.

4. **Mean time to recovery** - Mean time to recovery (MTTR) measures how long it takes to recover from a partial service interruption or total failure. This is an important metric to track, regardless of whether theinterruption is the result of a recent  deployment or an isolated system failure.
