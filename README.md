# Independent Federal Environmental Review Management Modernization Case Study

A complete federal IT modernization case study and working software prototype for managing infrastructure environmental reviews, permits, authorizations, milestones, dependencies, issues, pauses, and portfolio reporting.

## What this demonstrates

- Federal-process research using official public sources
- Current-state analysis
- Pain-point and root-cause analysis
- Future-state workflow design
- Product requirements and data modeling
- Python application development
- SQLite database design
- Automated testing
- Implementation planning
- Consulting-style communication

## Case-study framing

A fictional federal infrastructure office needs a stronger internal way to coordinate environmental reviews and authorizations across multiple agencies. The proposed platform supplements—not replaces—the public Federal Permitting Dashboard.

This project does not make environmental findings, issue permits, interpret law, or represent an official federal system. All application data is synthetic.

## Working features

- Portfolio dashboard
- Project creation and status management
- Lead-agency tracking
- Environmental review and authorization milestones
- Planned, target, and actual dates
- Milestone dependencies
- Schedule-extension reasons and explanations
- Project pause and resume workflow
- Issue and risk register
- Automatic overdue detection
- Audit logging
- Synthetic demonstration dataset

## Run locally

```bash
python -m venv .venv
```

Activate the environment:

Windows:

```bash
.venv\Scripts\activate
```

macOS/Linux:

```bash
source .venv/bin/activate
```

Install and test:

```bash
pip install -r requirements.txt
pytest
```

Start the application:

```bash
streamlit run app/main.py
```

## Repository guide

- `app/` — application and business logic
- `tests/` — automated test suite
- `data/` — generated local database and sample data
- `docs/` — consulting and technical deliverables
- `diagrams/` — Mermaid process and architecture diagrams
- `presentation/` — executive presentation and demo script

## Official public basis

The design is grounded in official federal sources including the Federal Permitting Dashboard, its public dataset and data-management guidance, the Permitting Council, CEQ/NEPA resources, and EPA's NEPA process guidance.

## Author

Preston Mcarthy  
St. Lawrence University, Data Science and Finance, Current Rising Sophomore
