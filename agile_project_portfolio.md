---
title: Agile Project Portfolio
---

[Back to home](index.html)

# Agile Project Portfolio

**Student Name:** Sinethemba Nyimbinya  
**Student Number:** 220085870  
**Subject:** Project Presentation 3 (PRP370S / PRP371S / PRP372S)  
**Qualification:** Diploma in Information and Communication Technology  
**Faculty:** Informatics and Design, Cape Peninsula University of Technology (CPUT)  

---

## Navigation & Quick Links

- [Portfolio Overview](#portfolio-overview)
- [1. Agile Team Charter](#1-agile-team-charter)
- [2. User Stories and Tasks](#2-user-stories-and-tasks)
- [3. Product Backlog](#3-product-backlog)
- [4. Sprint Backlog](#4-sprint-backlog)
- [5. Agile Logbook](#5-agile-logbook)
- [Synthesis: Connecting It All Together](#synthesis-connecting-it-all-together)

---

## Portfolio Overview

This digital portfolio collects my Agile project management evidence and reflective analysis for our **Entrepreneurial WIL Project**. 

Following higher education e-portfolio frameworks, this collection is structured through four core learning phases:
1. **Collect:** Gathering evidence and artifacts produced during our project lifecycle.
2. **Select:** Choosing evidence that best demonstrates practical understanding of Agile methodologies.
3. **Reflect:** Analyzing successes, friction points, and key personal growth throughout the project.
4. **Connect:** Drawing meaningful connections across artifacts to summarize my development as an ICT practitioner.

### Entrepreneurial WIL Project Context
Our team set out to tackle the persistent public health and sanitation crisis in **Khayelitsha, Cape Town**. The area frequently experiences severe sewage pipe bursts and blocked infrastructure, leaving households, local schools, and small businesses without clean water or hygienic surroundings for days.

To address this, our team conceptualized and engineered a **Sewage Repair & Monitoring Service** platform designed to streamline incident reporting using geotagging, improve response dispatching for municipal infrastructure, and track repair status in real time.

#### Solution Architecture & Tech Stack
- **Frontend:** React Native (Expo), TypeScript, Tailwind CSS / NativeWind
- **Backend:** Node.js (Express.js)
- **Database:** SQL with Supabase Row-Level Security (RLS)
- **Authentication:** Supabase Authentication (Email/Password, OTP)
- **Maps & Location:** Google Maps API, Expo Location
- **Payments:** PayFast Integration (for priority local business dispatching)

#### Agile Team Structure & Roles
- **Liyema Mangaliso (230760236):** Team Leader — Overall coordination, stakeholder communication, sprint goals, final sign-off.
- **Talent Nocuze (230405886):** Researcher / Agile Lead — Community research, facilitating meetings, removing blockers, managing workflow.
- **Sinethemba Nyimbinya (220085870 - My Role):** Writer / Editor & Developer — Drafting and editing all content, frontend development, git workflow management.
- **Muso Nkuntsu (231223722):** Presenter / Analyst — Preparing/delivering presentations, analyzing community survey data.
- **Libolwethu Nokenke (222665963):** Designer / Developer — Visual design, slide/document layouts, UI prototyping.

---

## 1. Agile Team Charter

### Evidence: Agreed Social Contract
*Agreement Date: 04 May 2026*

Our Team Charter established clear operational rules and shared expectations across the project:

- **Team Purpose & Mission:** Solve frequent sewage pipe bursts in Khayelitsha by delivering a community-backed repair and monitoring business plan and mobile platform.
- **Core Values:** Respect, Transparency, Accountability, Trust, and a Learning Mindset.
- **Working Agreements:** Arrive prepared and on time, respect timeboxes, give constructive feedback, and raise blockers early.
- **Communication SLA:** 
  - *Primary Channel:* WhatsApp Group (08:00–20:00).
  - *Response Times:* **3 hours** for standard tasks; **1 hour** for urgent submission blockers.
  - *Meetings & Storage:* Google Meet / Teams for planning; Google Drive for shared docs.
- **Decision-Making Protocol:** Democratic Team Vote.
- **Definition of Done (DoD):** Written content edited by Sinethemba (Writer/Editor), design/layout verified by Libolwethu, research verified by Talent, presentation rehearsed by Muso, final approval by Liyema (Leader), and uploaded to Drive/Blackboard before the deadline.
- **Key Identified Risks:** Conflicting student academic schedules, connectivity/data limits, low community survey response rates, and limited business planning experience.

### Reflective Analysis

Drafting and living by our team charter highlighted the crucial difference between informal agreements and a formal social contract. Serving as the team's Writer and Editor, my position within the Definition of Done (DoD) made me both a vital quality checkpoint and a potential bottleneck. When team members submitted technical sections close to assignment deadlines, I had to balance thorough editorial quality against tight submission windows.

Our original charter left the formal escalation path open for unresolvable disputes. Reflecting on high-pressure sprint deadlines, establishing an explicit escalation hierarchy from Day 1 would have reduced ambiguity. Overall, enforcing our 3-hour WhatsApp response expectation maintained team momentum and prevented minor blockers from escalating into submission failures.

---

## 2. User Stories and Tasks

### Evidence: User Stories & Task Breakdowns

To ensure our solution addressed genuine community needs, we broke requirements down into structured user stories with atomic technical tasks:

#### User Story 1: Resident Leak Reporting (US-01)
> *“As a Khayelitsha resident, I want to log a localized sewage burst report with attached GPS coordinates, so that municipal repair teams can locate and clear the blockage promptly.”*
- **Task 1.1:** Design a mobile-friendly report intake form UI in React Native.
- **Task 1.2:** Integrate Expo Location API for client-side geotagging and coordinate validation.
- **Task 1.3:** Build Express backend API endpoints to post incident payloads to the database.

#### User Story 2: Priority Business Dispatching (US-02)
> *“As a local business owner (spaza shop/salon), I want to request priority paid emergency drain cleaning via PayFast, so that my business avoids costly multi-day closures.”*
- **Task 2.1:** Integrate PayFast payment gateway endpoints into the user checkout flow.
- **Task 2.2:** Configure Supabase Realtime notification alerts for emergency maintenance crews.

#### User Story 3: Municipal Operations Dashboard (US-03)
> *“As a municipal operations supervisor, I want to view an aggregated dashboard of active leaks filtered by severity, so field crews can be dispatched efficiently.”*
- **Task 3.1:** Construct a status dashboard with status cards and filtering controls.
- **Task 3.2:** Implement Role-Based Access Control (RBAC) to secure municipal accounts.

### Reflective Analysis

Adopting user story mapping shifted our engineering focus from coding arbitrary features to solving real user problems. Writing stories from the perspective of Khayelitsha residents and spaza shop owners prevented scope bloat, stopping us from developing complex features that didn't add immediate value to sanitation reporting.

Breaking stories into actionable sub-tasks improved team transparency. Assigning concrete tasks on Trello (such as UI design, API integration, or documentation) based on individual team roles allowed us to work in parallel without overlapping effort, maintaining a steady development velocity.

---

## 3. Product Backlog

### Evidence: Trello Backlog Management

Our Product Backlog was created and managed on Trello, comprising **73 prioritized cards** organized across four core epics (Submitted: 30 July).

```
+----------------------------------------------------------------------------------+
|                            TRELLO PRODUCT BACKLOG BOARD                          |
+---------------------+------------------+-------------------+---------------------+
| Product Backlog (61)| Done (12)        | User Stories (2)  | Product Backlog (8) |
+---------------------+------------------+-------------------+---------------------+
| • Present final     | • Create Project | • US 1: Fast      | • User Report       |
|   results (Oct 24)  |   repo Github    |   Reporting       |   Submission Form   |
| • Update pitch deck | • Team roles &   | • US 2: Tracking  | • GPS Geolocation   |
|   results (Oct 23)  |   responsib.     |   Repair Progress |   Tagging           |
| • Document lessons  | • Founding team  |                   | • Database Setup &  |
|   learned           |   agreement      |                   |   Reporting API     |
+---------------------+------------------+-------------------+---------------------+
```

Key backlog items included:
- Initial repository initialization and workflow configuration on GitHub.
- Field survey data aggregation and solution architecture documentation.
- Database setup, REST API development, and PayFast integration.
- Pitch deck refinements and launch results presentation.

### Reflective Analysis

Managing a 73-card backlog reinforced the importance of continuous backlog grooming using the **MoSCoW** framework (*Must have, Should have, Could have, Won't have*). Early in the project, our backlog grew excessively as we attempted to include broad administrative modules. 

Through regular backlog refinement, we prioritized critical functionalities—such as reliable geotagged reporting—over secondary analytical tools. Pruning non-essential cards ensured our team focused energy on key deliverables required for our target releases.

---

## 4. Sprint Backlog

### Evidence: Sprint 2 Taskboard & Execution
*Sprint Window: 28 July – 31 July 2026*

- **Sprint Goal:** Complete Figma prototype navigation, finalize remaining UI screens, and align Trello tasks for sprint review.
- **Selected Backlog Items:**
  1. Review Product Backlog items in Trello (*Completed*).
  2. Design remaining UI screens in Figma (*In Progress - Sinethemba*).
  3. Improve prototype screen navigation links (*Completed*).
  4. Conduct Sprint 2 team review and sign-off (*Completed*).

```
+----------------------------------------------------------------------------------+
|                                SPRINT 2 TASKBOARD                                |
+----------------------------------+------------------------+----------------------+
| Product Backlog                  | In Progress            | Completed            |
+----------------------------------+------------------------+----------------------+
| • Review Product Backlog         | • Design remaining     | • Trello Product     |
| • Design remaining UI screens    |   UI screens           |   Backlog updated    |
| • Improve prototype navigation   |   (Sinethemba)         | • UI completed       |
|                                  |                        | • Review completed   |
+----------------------------------+------------------------+----------------------+
```

### Reflective Analysis

Executing the Sprint 2 backlog demonstrated the importance of realistic capacity planning. Linking interactive screens took longer than planned, which put our sprint review deadline at risk.

By addressing the delay during a stand-up, we evaluated our velocity and focused on core user flows first. This experience showed how the sprint backlog acts as a tactical commitment: keeping the team focused on immediate sprint goals while providing flexibility to manage unexpected technical work.

---

## 5. Agile Logbook

### Evidence: Logbook Records (Sprint 2 Submission)
*Logbook Submission Date: 05 August 2026*

| Date | Day | What I Completed Since Last Stand-up | What I Plan to Complete Next | Impediments / Blockers |
| :--- | :--- | :--- | :--- | :--- |
| **28 July 2026** | Friday | Designed 2 new UI screens in Figma. | Link all UI screens to the prototype for navigation and testing. | None. |
| **29 July 2026** | Saturday | Fixed Git merge conflicts successfully. | Complete all remaining screens assigned to my role. | None. |
| **30 July 2026** | Sunday | Reviewed Trello Product Backlog alignment. | Prepare submission files and sprint walkthrough notes. | None. |
| **31 July 2026** | Monday | Finalized interactive prototype navigation. | Conduct team review and retro session. | None. |

#### Sprint Walkthrough Summary
- **Advancing Work:** Completed the interactive prototype by linking all screens together, updated Trello cards, and gathered team feedback before development.
- **Unplanned Work:** None. All team members worked strictly on planned sprint tasks.
- **Team Completion:** Finished user interface designs, verified task prioritization on Trello, and confirmed prototype readiness.
- **Blockers & Impediments:** No major blockers. Extra time was allocated to refining screen layouts and interactive link paths for smoother navigation.

### Reflective Analysis

Maintaining daily logbook records provided transparency into individual contributions. Documenting daily progress helped identify technical issues early, such as resolving the Git merge conflicts encountered on 29 July before they could disrupt the submission workflow.

Logbook retrospectives offered a reliable framework for continuous team improvement. Reviewing stand-up logs highlighted communication patterns, allowing us to refine editing handoffs between team members and keep development on track.

---

## Synthesis: Connecting It All Together

Looking back across the full arc of Project Presentation 3—from our early Business Case in April through to our Solution Architecture in August and final submission in October—the value of an integrated Agile framework is clear.

The **Agile Team Charter** established our working values, communication expectations, and Definition of Done. Those rules directly governed how we structured our **Product Backlog** and refined raw project requirements into actionable **User Stories and Tasks**. The backlog served as the primary pool from which our **Sprint Backlogs** were drawn, ensuring our immediate daily work remained aligned with high-level project goals. Finally, the **Agile Logbook** provided continuous feedback—capturing daily progress, identifying technical blockers, and driving team optimization through retrospectives.

Carrying these lessons into my future career as a developer, I recognize that technical delivery and solid software design must be paired with structured Agile processes, continuous reflection, and clear team communication.

---
[Back to top](#agile-project-portfolio) | [Back to home](index.html)
