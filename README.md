# Independent Federal IT Modernization Case Study

## Federal Environmental Review Management Platform

This repository is an independent case study and working software prototype showing how a government IT consulting team could improve the internal management of federal environmental review and permitting projects.

The project is designed for readers who have no prior knowledge of environmental review, federal permitting, or government project-management systems. This README explains the problem, the real federal process, the proposed solution, the software, the research basis, and why the project was created.

---

## 1. What this project is

Large infrastructure projects—such as transmission lines, rail improvements, ports, broadband networks, pipelines, and energy facilities—often require several federal environmental reviews, permits, and authorizations before construction can proceed.

Those reviews may involve:

- a lead federal agency;
- multiple participating agencies;
- environmental studies;
- public notices and comment periods;
- permits and authorizations;
- project documents;
- milestone deadlines;
- schedule changes;
- dependencies between agencies; and
- pauses caused by project redesign, missing information, litigation, or other events.

This project does **not** make environmental decisions or issue permits.

It builds a management platform that helps the people coordinating those reviews answer simple operational questions:

- What projects are active?
- What is due next?
- Which agency owns each milestone?
- What is late?
- Why did a deadline change?
- Which projects are paused?
- What issues need management attention?
- What changed recently?

The simplest comparison is:

> This is project-management software—similar in purpose to Jira, Asana, or Microsoft Project—but structured around the real concepts used in federal environmental review and permitting.

---

## 2. Why this federal office and process were chosen

### The office being modeled

This case study models a **fictional federal infrastructure coordination office** whose work is based on the publicly documented process administered across government through the **Federal Permitting Improvement Steering Council**, commonly called the **Permitting Council**.

The fictional office was used rather than claiming to reproduce one agency's private internal process. That keeps the project accurate and honest: the public sources show how the cross-government process is structured, but they do not reveal every internal system, spreadsheet, email workflow, or staffing practice used by each agency.

The Permitting Council is a strong basis for the case study because it is specifically responsible for improving the transparency, predictability, and coordination of federal environmental reviews and authorizations for major infrastructure projects.

### Why this process was selected

This process was selected because it is:

1. **Real and publicly documented.**  
   The federal government publishes projects, agencies, actions, milestones, target dates, schedule changes, and pause information through the Federal Permitting Dashboard.

2. **Cross-agency.**  
   One project may require work from several federal agencies, which creates a genuine coordination and information-management challenge.

3. **Actively being modernized.**  
   The Permitting Council has publicly described plans to make the Dashboard more dynamic, user-centered, automated, analytically useful, and cost-effective.

4. **Relevant to federal IT consulting.**  
   The work involves process analysis, requirements gathering, project management, workflow design, data modeling, application development, testing, reporting, and implementation planning.

5. **Appropriate for a portfolio project.**  
   It is complex enough to demonstrate consulting and technical skills, but it can be studied without using classified, proprietary, or personal data.

---

## 3. The real process in simple terms

Imagine the federal government is reviewing a proposed electricity transmission line.

The government cannot simply approve construction immediately. Several reviews and authorizations may be required.

### Real-world workflow

```text
A company or public agency proposes an infrastructure project
                            ↓
A lead federal agency is identified
                            ↓
Other participating agencies are identified
                            ↓
The required environmental reviews, permits, and authorizations are listed
                            ↓
Each review or authorization is divided into major milestones
                            ↓
Each milestone receives an owner and a target date
                            ↓
Agencies perform studies, review documents, consult stakeholders,
and complete their assigned milestones
                            ↓
Project managers monitor deadlines and dependencies
                            ↓
When a date changes, the reason and explanation are recorded
                            ↓
When outside circumstances stop progress, the project may be paused
                            ↓
The project resumes when a reliable schedule can be established
                            ↓
The required reviews and authorizations are completed
                            ↓
The agency makes its decision and the project leaves the review process
```

### What the key terms mean

**Project**  
The infrastructure proposal being reviewed, such as a rail expansion or power line.

**Action**  
A specific environmental review, permit, or authorization required for the project.

**Milestone**  
An important step within an action, such as publishing a draft document, completing consultation, or issuing a final decision.

**Lead agency**  
The federal agency coordinating the overall review.

**Participating agency**  
Another agency responsible for part of the review or an authorization.

**Target date**  
The current expected completion date for a milestone.

**Dependency**  
A relationship where one milestone cannot proceed until another is completed.

**Pause**  
A formal period when meaningful progress cannot continue and the timetable cannot be reliably maintained.

**Portfolio**  
The complete group of projects being managed by leadership.

---

## 4. Why the government chose this area for modernization

The federal government has already identified permitting coordination and technology as modernization priorities.

Public federal materials describe several needs:

- transparent and predictable project schedules;
- coordinated timetables across agencies;
- better data quality and completeness;
- earlier identification and resolution of risks;
- automated notifications;
- clearer explanations for schedule changes;
- stronger analytics;
- more user-centered technology; and
- a more dynamic and cost-effective Permitting Dashboard.

A 2017 Permitting Council report described technical improvements such as automated notifications when milestone target dates were approaching. More recent budget and annual-report materials describe a need for a more dynamic platform that can streamline and automate workflows, improve data integrity, strengthen analytics, and better track causes of delay.

This matters because infrastructure reviews are not a single linear task performed by one person. They are coordinated programs with many organizations, documents, dates, and dependencies. Technology cannot replace environmental judgment, but it can make the coordination work clearer and more reliable.

---

## 5. The current public system

The Federal Permitting Dashboard already provides important capabilities:

- public project listings;
- project descriptions and sectors;
- lead and participating agencies;
- environmental reviews and authorizations;
- major milestones;
- target and completion dates;
- timetable changes;
- project status;
- public data downloads; and
- transparency for sponsors and the public.

The Dashboard is valuable and this case study does not propose replacing it.

### The operational gap explored by this case study

A public transparency dashboard is not necessarily the same as an internal project-management workspace.

An internal team may also need:

- detailed ownership;
- issue escalation;
- milestone dependencies;
- internal notes;
- document coordination;
- controlled project pause and resume actions;
- audit history;
- portfolio health;
- workload views; and
- management alerts.

The case study asks:

> What would a practical internal management companion to the public Dashboard look like?

---

## 6. Our proposed changes

The proposed future state keeps the real federal structure but makes it easier to manage internally.

### Proposed workflow

```text
Create one authoritative project record
                    ↓
Record the lead and participating agencies
                    ↓
List each required review, permit, or authorization
                    ↓
Create milestones with owners, dates, and dependencies
                    ↓
Display the next actions and overdue work
                    ↓
Log issues that could affect the schedule
                    ↓
Require a reason and explanation when a target date changes
                    ↓
Pause and resume projects through controlled status changes
                    ↓
Preserve every material change in an audit log
                    ↓
Show managers both individual project details and portfolio-wide risks
                    ↓
Publish only approved public information to the external Dashboard
```

### Main changes proposed

1. **Plain-language portfolio dashboard**  
   Leadership can immediately see active, paused, and at-risk projects.

2. **Structured project records**  
   Every project has a clear lead agency, status, sector, location, milestones, and issues.

3. **Milestone ownership**  
   Every major step has an owner agency and target date.

4. **Dependency management**  
   The system can represent work that cannot begin until another milestone finishes.

5. **Controlled schedule extensions**  
   A target date cannot simply be overwritten. The new date, old date, reason, explanation, actor, and timestamp are retained.

6. **Formal pause and resume process**  
   A paused project is distinguished from a late project.

7. **Issue and risk visibility**  
   Problems are recorded with priority, owner, due date, and description.

8. **Audit history**  
   Users can see who changed what and when.

9. **Project and portfolio views**  
   Working-level staff see individual tasks and milestones; managers see patterns across all projects.

10. **Human decision authority**  
    The software organizes the process but never makes environmental, legal, or permitting decisions.

---

## 7. What is being changed in real life

### Federal Permitting Council modernization

The most directly relevant real-world effort is the government's own modernization of the Federal Permitting Dashboard.

Public materials describe desired changes that include:

- more automated workflows;
- improved data integrity;
- stronger analytics;
- better tracking of delay causes;
- improved transparency and predictability;
- a more dynamic and user-centered platform; and
- continued active project management by the Permitting Council.

These plans are closely aligned with this case study's emphasis on structured data, schedule management, exceptions, and reporting.

### Earlier federal improvements

The Permitting Council has also described earlier improvements such as:

- automated notifications for approaching target dates;
- quarterly data-quality assessments;
- coordination with agencies to correct missing or inaccurate timetable data; and
- more detailed explanations for schedule changes.

### Contractor examples from related federal modernization work

Publicly available sources do **not** clearly identify which contractor or contractors built the current Federal Permitting Dashboard. This project therefore does not claim that a named company is implementing this exact platform.

However, public case studies show how federal contractors implement similar modernization patterns.

#### Accenture Federal Services and the Bureau of Land Management

Accenture Federal Services publicly describes work with the Bureau of Land Management to modernize decades-old land-management systems. The reported problems included:

- manual processes and paperwork;
- slow customer service;
- legacy systems;
- difficult code-based workflows;
- weak data validation;
- human-error risk; and
- outdated payment and records capabilities.

The modernization focused on streamlined digital processes, improved validation, easier customer interaction, and more transparent access to land records.

#### Booz Allen and Recreation.gov

Booz Allen publicly describes helping federal partners replace and improve the Recreation.gov reservation-services platform. The work focused on a more reliable digital platform, improved customer experience, and a different outcomes-oriented delivery model.

This is not an environmental-review system, but it demonstrates the same broader government-contractor pattern:

```text
Old or fragmented public service
                ↓
Research user and agency needs
                ↓
Redesign the workflow and customer experience
                ↓
Build a more reliable digital platform
                ↓
Measure service outcomes
```

#### Accenture infrastructure and permitting services

Accenture also publicly describes infrastructure and capital-project services that coordinate permitting requirements, studies, compliance processes, and project timelines. This provides a direct industry example of contractors supporting the management side of permitting.

---

## 8. Comparing our proposal with real modernization

| Area | This case study | Real federal modernization |
|---|---|---|
| Project structure | Projects, actions, milestones, agencies | Federal Dashboard uses projects, reviews/authorizations, milestones, and agencies |
| Timetable management | Planned, target, and actual dates | Government publishes permitting timetables and target dates |
| Schedule changes | Reason, explanation, old date, new date, audit entry | Government requires explanations for timetable modifications |
| Notifications | Represented as a future capability | Earlier federal improvements included approaching-date notifications |
| Pauses | Controlled pause and resume workflow | Federal guidance explicitly supports project pause status |
| Analytics | Portfolio metrics and overdue counts | Current federal plans emphasize stronger analytics and delay-cause tracking |
| Internal operations | Issues, dependencies, internal history | Public materials focus primarily on published project and timetable information |
| Public transparency | Designed as a future approved-data integration | The existing Dashboard is already a public transparency tool |
| Legal decisions | Always human | Real agencies retain environmental and permitting authority |
| Deployment | Local educational prototype | Real systems require enterprise security, accessibility, records, hosting, and integration |

### Main similarity

Both approaches treat permitting modernization as a coordination and information problem—not as an attempt to remove environmental review.

### Main difference

The real Dashboard is a government-wide public system. This prototype is an educational model of an **internal management companion** with more emphasis on day-to-day project operations.

---

## 9. Benefits of the real changes

The government's modernization approach can provide:

- consistent public transparency;
- government-wide project visibility;
- stronger accountability;
- standardized data;
- improved milestone conformance;
- more predictable schedules;
- better identification of delay patterns; and
- improved coordination across agencies.

Because it operates across the federal government, the real Dashboard can create a common language and reporting structure for projects managed by different agencies.

---

## 10. Benefits of our proposed changes

The proposed internal platform can provide:

- faster understanding of project status;
- clearer milestone ownership;
- earlier discovery of overdue work;
- visible dependencies;
- consistent extension explanations;
- formal distinction between paused and delayed work;
- easier issue escalation;
- a complete audit trail;
- better management reporting; and
- structured information that could later feed a public dashboard.

The value is not that the software makes decisions faster by itself. The value is that staff spend less time reconstructing status and more time resolving the actual work blocking progress.

---

## 11. Simple explanation of the software

The software has six navigation pages.

### How It Works

A beginner-friendly explanation of the federal workflow, the software terms, and the relationship between projects, actions, milestones, issues, and audit history.

### Portfolio

A management summary of all projects.

It answers:

- How many projects exist?
- How many are active?
- How many are paused?
- How many milestones are late?
- What is the overall completion rate?

### Projects

The master record for each infrastructure project.

A user can:

- create a project;
- view its description and lead agency;
- see its current status;
- pause it with a reason; and
- resume it later.

### Milestones

The schedule of major work.

A user can:

- view milestones for one project;
- see the responsible agency;
- see planned, target, and actual dates;
- add a milestone;
- mark it complete; or
- extend the target date with a documented reason.

### Issues

The list of problems requiring attention.

Examples include:

- a delayed survey;
- missing project information;
- unresolved consultation;
- incomplete sponsor documents; or
- a dependency blocking another agency.

### Audit Log

The chronological record of material changes.

It answers:

- Who created the project?
- Who changed a deadline?
- Why was it changed?
- When was a project paused?
- When was an issue added?

### About

A short explanation of the case-study purpose, limitations, and synthetic data.

---

## 12. Why I made this

I created this project to learn and demonstrate the work performed in federal IT modernization and government consulting.

I am a Data Science and Finance student at St. Lawrence University based in Northern Virginia. I am interested in government consulting, IT consulting, data, process improvement, and the modernization of older public-sector systems.

Rather than building an unrelated coding exercise, I wanted to complete the full lifecycle of a realistic consulting engagement:

```text
Research a real federal process
                ↓
Understand the users and operating problem
                ↓
Document the current state
                ↓
Identify pain points
                ↓
Design a future state
                ↓
Translate the design into software requirements
                ↓
Build a working prototype
                ↓
Test the business rules
                ↓
Document the technical and business decisions
                ↓
Present the result as a consulting case study
```

The project is intended to show that I can connect business needs with technology—not simply write code.

---

## 13. What the prototype currently does

- Displays a portfolio of synthetic infrastructure projects
- Tracks active, paused, planning, and completed status
- Creates new projects
- Tracks lead agency, sector, state, and description
- Creates milestones within environmental reviews and authorizations
- Stores planned, target, and actual dates
- Tracks owner agencies
- Supports milestone dependencies in the service layer
- Detects overdue milestones
- Requires reasons and explanations for deadline extensions
- Pauses and resumes projects
- Creates issues with priority and ownership
- Records audit history
- Seeds a synthetic demonstration dataset

---

## 14. What the prototype deliberately does not do

- Make environmental findings
- Determine whether impacts are significant
- Approve projects
- Issue permits
- Interpret statutes or regulations
- Store real government data
- Authenticate federal users
- Meet production federal cybersecurity requirements
- Replace the Federal Permitting Dashboard
- Claim endorsement by a federal agency or contractor

---

## 15. Run and test the project

Create and activate a virtual environment, then run:

```bash
python -m pip install -r requirements.txt
python -m pytest -v
python -m streamlit run app/main.py
```

The test suite validates database creation, project rules, milestone-date rules, dependencies, target-date extensions, pause and resume behavior, overdue detection, issue validation, audit history, and required repository documentation.

---

## 16. Repository structure

```text
app/             Working application and business logic
data/            Local synthetic demonstration database
tests/           Automated test suite
docs/            Consulting and technical deliverables
diagrams/        Current-state, future-state, and data-model diagrams
presentation/    Executive presentation, demo script, and interview materials
```

---

## 17. Official and industry sources

### Official federal sources

- Federal Permitting Dashboard — https://www.permits.performance.gov/projects
- Permitting Dashboard Full Dataset — https://data.permits.performance.gov/Permitting-Project/Permitting-Dashboard-Full-Dataset/mcm3-xbid
- Permitting Council current FAST-41 portfolio — https://www.permitting.gov/projects/current-fast-41-portfolio
- Permitting Council FY 2025 Annual Report — https://www.permitting.gov/sites/default/files/2026-04/Permitting-Council-FY-2025-Annual-Report-to-Congress.pdf
- Permitting Council FY 2026 Budget Request — https://www.permitting.gov/sites/default/files/2025-06/Permitting-Council-FY26-Budget-Request_508_.pdf
- FAST-41 guidance — https://www.permitting.gov/sites/default/files/2025-01/M-25-09-FAST-41-Guidance.pdf
- Pausing Projects guidance — https://www.permits.performance.gov/documentation/pausing-projects
- EPA explanation of NEPA — https://www.epa.gov/nepa/what-national-environmental-policy-act

### Contractor and industry examples

- Accenture Federal Services: Modernizing Public Land Management — https://www.accenture.com/us-en/case-studies/us-federal-government/bureau-land-management
- Accenture Infrastructure and Capital Projects — https://www.accenture.com/us-en/services/infrastructure-capital-projects
- Booz Allen: Reinventing the Recreation.gov Customer Experience — https://www.boozallen.com/s/insight/thought-leadership/reinventing-the-recreation-gov-customer-experience.html

---

## Author

**Preston Mcarthy**  
St. Lawrence University  
Data Science and Finance
