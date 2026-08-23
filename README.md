# AI-Powered Customer Intelligence Transformation Project
 
**AnalystLab Africa - Project Management Internship, Week 3**
**Author:** Devinci Ebaha Djoki ([LinkedIn](https://linkedin.com/in/ebaha-devinci))
 
## Overview
 
This repository contains the Week 1 through Week 3 deliverables of the AnalystLab Africa Project Management Internship Programme. The project moves through initiation and planning (Week 1), execution planning (Week 2), and detailed scheduling with formal Critical Path Analysis (Week 3), applied throughout to a real Cameroonian retail company, **DOVV Distribution SA**, rather than a purely fictional case.
 
All figures related to DOVV's internal performance (churn rate, customer segments, budget) are working assumptions built for the purpose of this exercise, in the absence of access to DOVV's real internal data, a standard practice at the scoping stage in consulting.
 
## Business Scenario
 
DOVV Distribution SA, a Cameroonian retail chain established in Yaounde, does not yet have a structured system to identify customers at checkout, track purchase history over time, or personalise offers. This project designs and schedules a solution combining a loyalty identification system with an AI-driven churn prediction and personalisation engine, aimed at increasing the proportion of regular customers within the existing customer base from 15 percent to 25 percent over 16 months.
 
## Week 3: Project Scheduling, Resource Planning & Execution Planning
 
Week 3 formalises the project's schedule into a full network model: every one of the 42 activities carries a calculated Earliest Start, Earliest Finish, Latest Start, Latest Finish, and Total Float, and the Critical Path is identified and explained rather than assumed.
 
> **Note on scope:** AnalystLab Africa issued a revised Week 3 brief mid-week, removing the Resource Allocation Plan and Project Execution Plan as Week 3 deliverables (they remain valid Week 2 deliverables) and adding a Schedule Improvement Recommendations Report in their place. Both documents remain in this repository under Week 2 for portfolio completeness, and the table below reflects the deliverables covered by Week 3's final assessment criteria.
 
| Document | Description |
|---|---|
| [Part 1 - Review of Week 2 Documents](deliverables/week3/Part1_Review_Week2_Documents.pdf) | Documents two dependency corrections and the WBS granularity update surfaced while preparing this week's Critical Path Analysis |
| [Project Schedule](deliverables/week3/Dovv_Project_Schedule.xlsx) | 42 activities with Activity ID, Name, Duration, Start/Finish Date, Dependencies, and Assigned Resource |
| [Gantt Chart](deliverables/week3/Dovv_Gantt_Chart.xlsx) | Weekly-calendar Gantt chart with phase colour coding; every bar's start and end date verified programmatically against the schedule, not just visually |
| [Network Diagram](deliverables/week3/Dovv_Network_Diagram.pdf) | Activity-on-Node diagram showing ES, EF, LS, LF and Total Float for all 42 activities, critical path highlighted in red |
| [Critical Path Analysis](deliverables/week3/Dovv_Critical_Path_Analysis.pdf) | Explains why the adoption campaign chain, not the technical or data science work, controls the project's completion date |
| [Schedule Risk Assessment](deliverables/week3/Dovv_Schedule_Risk_Assessment.pdf) | Six schedule-specific risks (SR-01 to SR-06) with Risk ID, Affected Activity, probability, impact, mitigation, and contingency |
| [Schedule Improvement Recommendations Report](deliverables/week3/Dovv_Schedule_Improvement_Recommendations.pdf) | Concrete actions across six risk areas (critical activities, high-risk activities, resource constraints, dependency bottlenecks, likely delays, mitigating actions), grounded in the Critical Path Analysis and Risk Assessment |
 
### Notable design decisions - Week 3
 
- **The critical path was verified twice, not assumed once.** Every Total Float value was calculated independently through a Python reference implementation and cross-checked line by line against the Excel formulas before either was trusted, after an earlier Gantt chart iteration was found, on inspection, to render bars incorrectly despite appearing correct on screen.
- **Critical-path ownership was checked role by role, not phase by phase.** An early draft of the Execution Plan claimed only two roles carried critical-path responsibility; re-verifying against the actual Assigned Resource data showed six different roles each own at least one critical-path task at different points in the 16-month timeline. The Execution Plan and Schedule Risk Assessment were corrected accordingly.
- **Waiting periods are treated as real schedule elements, not gaps.** The three data-accumulation and three adoption-ramp-up periods are modelled as explicit tasks with duration, not implicit blank space, since they collectively account for the largest single block of critical-path time in the project (160 calendar days for the adoption ramp-up alone).
## Week 1–2: Initiation and Execution Planning
 
| Document | Description |
|---|---|
| [Project Charter](deliverables/week1/Dovv_Project_Charter.pdf) | Project mandate: background, SMART objective, scope, deliverables, sponsor, constraints, timeline, success criteria |
| [Stakeholder Register](deliverables/week1/Dovv_Stakeholder_Register.pdf) | Stakeholder mapping by influence and interest, with engagement strategies |
| [Work Breakdown Structure](deliverables/week1/Dovv_WBS.pdf) | Project decomposition into phases and tasks, updated in Week 3 to match the full 42-task granularity used in the Schedule |
| [Risk Register](deliverables/week1/Dovv_Risk_Register.pdf) | Eight identified risks across technical, organisational, legal and strategic categories, with mitigation plans |
| [Communication Plan](deliverables/week1/Dovv_Communication_Plan.pdf) | Two-layer communication structure: routine cadence tied to the WBS, and exception alerts tied to high-impact risks |
| [Project Budget](deliverables/week2/Dovv_Project_Budget.pdf) | Seven budget categories with a 15 percent contingency reserve, sized against the Risk Register's risk profile |
| [Project Execution Strategy](deliverables/week2/Dovv_Project_Execution_Strategy.pdf) | Week 2 execution approach, monitoring, risk management, communication, and change control |
| [Resource Allocation Plan (extended)](deliverables/week2/Dovv_Resource_Allocation_Plan_Week3.pdf) | Human, technical, and budget resources, extended with two roles (Business Analyst, QA Tester) found to be genuine gaps in the original plan |
| [Project Execution Plan (extended)](deliverables/week2/Dovv_Project_Execution_Plan_Week3.pdf) | Governance, communication, task assignment, and escalation, calibrated against verified critical-path ownership by role |
| [PM Deliverables Methodology Guide](deliverables/week1/Guide_Methodologique_Livrables_PM.pdf) | General reference guide on the structure and content of each core PM deliverable, independent of this specific case |
 
## Notable Design Decisions - Weeks 1-2
 
- **Retention, not acquisition.** The SMART objective explicitly targets DOVV's existing customer base, with customer acquisition marketing intentionally placed out of scope.
- **Parallel, not sequential, execution.** The WBS reflects that technical development and data collection run concurrently, and that the customer adoption campaign cannot start before the loyalty card itself is available.
- **A strategic risk, not just an operational one.** The Risk Register includes the possibility that the chosen solution itself may not be the most efficient approach, with a mitigation pointing to existing local alternatives (such as Koree or Gwassou) as a partnership option worth evaluating before building in house.
## Methodology
 
This work follows a PMBOK-aligned approach, adapted for a pilot-scale retail transformation project, including formal network scheduling (forward pass / backward pass, Activity-on-Node) for the Critical Path Analysis. AI tools were used to assist with research, drafting, and calculation verification, in line with the internship's guidelines; all reasoning, decisions, and final content were reviewed and validated by the author.
 
## Programme Context
 
Produced as part of the AnalystLab Africa Project Management Internship Programme (August–October 2026), alongside the Google and IBM Project Management and Data Analytics professional certificates (Coursera).
 
---
 
*This project is an academic exercise conducted within a structured internship programme. It does not represent an engagement commissioned by DOVV Distribution SA.*
 
