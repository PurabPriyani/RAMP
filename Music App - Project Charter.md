# Project Charter

| | |
|---|---|
| **Project Title** | XXXXXXXXX - "Making Music Social" |
| **Sponsor by** | RAMP LLC. |
| **Project Start Date** | September 7th, 2026 |
| **Budget Allocation** | TBD |

## **Content table**

- [Project Objectives](#project-objectives)
- [Project Success Criteria](#project-success-criteria)
- [Scope](#scope)
- [Out-of-Scope](#out-of-scope)
- [Milestones](#milestones)
- [Business Context Summary](#business-context-summary)
- [Problem Statement](#problem-statement)
- [Impact](#impact)
- [Assumptions](#assumptions)
- [Constraints](#constraints)
- [Still Unknown](#still-unknown)
- [Risk and Mitigation Plan](#risk-and-mitigation-plan)
- [Stakeholder Register](#stakeholder-register)
- [Team-Agreement](#team-agreement)
- [Repository-&-Workspace-Evidence](#repository--workspace-evidence)


## Project Objectives
**Project Name:** [App Name] - "Making Music Social"

This project aims to *design, build,* and *launch* a music streaming platform with integrated social, artist-facing features, and monetizing guided by the following **Primary objectives:**

1. Launch a functional streaming platform within 2 semesters that supports on-demand listening and offline downloading for 5000 concurrent users.
2. Design a personalized recommendation system aiming to increase average engagement session compared to a non-personalized baseline.
3. Enable social engagement features (Friends tab, activity feed, posts) that drive a target a portion of active users to interact socially (follow, post, or view friend activity).
4. Provide lyrics & song-context features with synced lyrics & backstories for at least 80% of the music catalog at launch.
5. Intergrate a an Artist Type Portal enabling users to create a Artist account to upload tracks and access analytics dashboards, integrated in the app for Artist accounts only.
6. Implement a secure payments and monetization system supporting subscriptions and ability to monetize content based on engagement metrics of users with Artist content.
7. Establish a scalable technical architecture (microservices, backend/frontend APIs) capable of supporting 5000 users with 95% uptime and response times under 600ms.

**Optional/TBD objectives:**
    - Deliver an instrument learning module (starting with guitar) enabling users to learn to play a defined set of songs, measured by feature adoption rate.
    - Implement a real-time sync infrastructure (Optional/TBD) allowing syncronous listning to music for at least 2 friends concurrently.

## Project Success Criteria
1. **Functional Completeness**
- Core features are implemented and demonstrable: music streaming, downloading, lyrics sync, recommendations, social feed/friends tab, artist upload portal, and payments flow.
- App runs end-to-end without critical bugs during final demo/evaluation.

2. **Technical Architecture Quality**
- Backend built using microservices architecture with clearly defined, documented APIs.
- System is designed to scale to 5,000 concurrent users (validated via load testing or architectural justification, even without live-tested at that volume).
- Real-time sync infrastructure (Optional/TBD) (e.g., WebSockets or equivalent) is implemented to support synchronized multi-user playback sessions with low latency.
- Codebase follows sound engineering practices (modularity, version control, documentation) suitable for grading/review.

3. **Personalization & Recommendations**
- Recommendation engine is functional and demonstrably improves content relevance (e.g., shown via a demo comparing personalized vs. generic results).

4. **Social & Engagement Features**
- Friends tab, activity sharing, and posts are functional and demonstrable in a live or simulated multi-user scenario.
- Syncronous Listening: for at least 2 friends can join a shared listening session where playback (play/pause/seek) is synced in real time across all participants' devices, with any participant able to control playback.
- Synced session maintains acceptable audio sync tolerance (e.g., within [X] ms/seconds) across participants during the demo.

5. **Artist Portal**
- Artists can upload tracks and view basic analytics (plays, likes, etc.) in a working dashboard.

6. **Monetization Flow**
- Payment/subscription flow is implemented and functional in at least a sandbox/test environment (e.g., Stripe test mode), even if not live/public.

7. **Learning Module** (TBD)
- Instrument-learning feature (e.g., guitar) is functional for at least a limited song set, demonstrating the concept works end-to-end.

8. **Academic & Presentation Criteria**
- Project meets all capstone deliverable requirements (documentation, presentation, demo, source code submission) by August 2027.
- Team can clearly articulate architecture decisions, trade-offs, and scalability plan (e.g., "how this would support 5,000 real users") during defense/presentation.

9. **Future Viability (Stretch Goal)**
- App is structured such that it could be deployed publicly with minimal rework i.e., architecture and infrastructure decisions don't block a future real-world launch.

## Scope
1. **Platform**
- Web application (primary platform, responsive design for desktop/mobile browsers)

2. **Core Music Experience**
- Music streaming (on-demand playback)
- Music downloading (offline listening)
- Synced lyrics display
- Song description / backstory content
- Personalized recommendation engine

3. **Social Features**
- Friends tab and listening activity feed
- Social posts (sharing songs, activity, updates)
- Synced group listening (2+ friends, shared real-time playback control) — feature name TBD

4. **Learning Feature**
- Instrument-learning module (starting with guitar), covering a limited, defined song set

5. **Artist Tools**
- Artist upload portal (music upload)
- Basic artist analytics dashboard (plays, likes, engagement)

6. **Monetization**
- Payment/subscription flow (implemented in sandbox/test environment)

7. **Technical Architecture**
- Backend built on microservices architecture
- Documented backend/frontend APIs
- Real-time sync infrastructure to support synced listening sessions
- System designed (and where feasible, tested) to scale toward 5,000 concurrent users

8. **Academic Deliverables**
- Full documentation (architecture, design decisions, trade-offs)
- Final working demo/prototype
- Capstone presentation/defense materials
- Source code submission

## Out of Scope
1. **Product & Business**
- Public commercial launch or App Store/Play Store release (unless pursued voluntarily post-capstone)
- Real revenue generation or live financial transactions (payments will run in test mode only)
- Marketing or growth campaigns
- Real catalog licensing is out of scope; project will use royalty-free or placeholder audio content.
- Customer support infrastructure

2. **Technical**
- Native Android app; possible stretch goal, not confirmed for MVP; to be assessed based on time/resources after core web app is complete.
- Native iOS app (not being considered at this stage)
- Multi-region infrastructure / global CDN deployment
- Advanced content moderation systems for social posts/uploads
- Support for live/broadcast audio (radio-style)
- Multi-language support

## Milestones
| Week | Milestone | Deliverables / Evidence |
|---|---|---|
| **Week 1** | Project Charter | Project Charter document (Objectives, Success Criteria, Scope, Stakeholders, etc.) |
| **Week 2** | Current-System Analysis | - Current-System Analysis<br>- As-Is Process Diagram<br>- System Context Diagram<br>- Current-System Limitations Table<br>- Technology Workspace Evidence<br>- Repository docs updated with above components |
| **Week 3** | Requirements/Design | Requirements Specification, Process Diagram, or initial system/architecture design |
| **Week 4** | Design/Planning | System Architecture Design, Data Model/ERD, or UI wireframes |

## Business Context Summary
Most music streaming platforms (Spotify, Apple Music, YouTube Music) treat listening as a solitary activity, with only surface-level social features. Inspired by Strava's success turning fitness into a shared, community-driven experience, this project applies the same model to music; making listening, discovery, and learning a connected, social experience rather than a passive one.  

## Problem Statement
Music listening today is largely a solitary, passive experience. While streaming platforms offer vast catalogs and basic sharing features, they lack real-time, shared listening experiences that let friends enjoy music together the way they might share a run or workout.

This creates a gap between how people consume music and how they want to connect around it, socially, actively, and meaningfully. This project addresses that gap by building a music platform that combines streaming, synced social listening, personalized discovery, instrument learning, and artist tools into a single, connected experience.

## Impact
**Users**
- Turns solo listening into a shared, social experience; Deepening engagement through lyrics, song context, and personalized discovery
- Bridges listening with active skill-building via the instrument-learning module

**Artists**
- Direct channel to upload music and reach listeners
- Access to engagement analytics without relying on labels/major platforms

**Industry**
- Explores real-time synced listening — a gap in mainstream platforms
- Demonstrates a social-first approach to music consumption

**Academic**
- Showcases ability to design/build a scalable, microservices-based app
- Demonstrates handling of real-world complexity (real-time sync, recommendations, payments)
- Strong technical portfolio piece for future opportunities

## Assumptions
- Royalty-free, licensed-for-education, or placeholder audio content will be used.
- Sufficient sample content will be available or creatable.
- Chosen tech stack will support real-time synced playback without major performance issues at demo scale.
- Cloud/hosting infrastructure used will be sufficient to simulate scalability discussions.
- Third-party APIs/services (e.g., payment sandbox, hosting providers) will remain available and stable throughout development.
- The 9 active semester months (Sep 2026 – Aug 2027) will be sufficient to deliver all in-scope features at a functional level.
- Feature scope will remain stable, with major changes unlikely once development begins.
- Public launch is not required for project success.
- Stakeholders will not assess real-world user adoption.

## Constraints
- **Timeline:** Fixed 9 active semester months (Sep 2026 – Aug 2027); no flexibility on final deadline.
- **Team size/skills:** Limited to current team members' availability and skill sets; no dedicated specialists.
- **Budget:** Limited/no funding; reliant on free tiers, student licenses, and sandbox/test services.
- **Content licensing:** No access to real music catalogs; must use royalty-free or placeholder audio.
- **Infrastructure:** Limited to free/low-cost hosting and cloud resources; true 5000 user load testing likely not feasible.
- **Academic requirements:** Must align with course outline, deliverables and checkpoints, which may shift priorities.

## Still Unknown
- Final feature name and control model for synced group listening (co-host vs. single host)
- Whether Android app will be pursued (stretch goal, unconfirmed)
- Specific tech stack choices (frameworks, hosting provider, real-time sync tool)
- Exact source of sample music/audio content

## Risk and Mitigation Plan
| Risk | Mitigation |
|---|---|
| Real-time sync is technically complex and may cause delays | Treat as phase-2/stretch feature; build core streaming first |
| Team skill gaps in microservices or real-time systems | Allocate early weeks for learning; use well-documented frameworks |
| Scope creep from adding social/artist features | Lock MVP scope early; treat extras as stretch goals |
| Limited infrastructure budget affects testing at scale | Use architectural justification instead of live load testing for 5000 user claim |
| Licensing issues with real music content | Use royalty free and/or sample audio from the start |
| Fixed deadline with academic checkpoints may shift priorities | Build in buffer time each phase; re-prioritize based on instructor feedback |

## Stakeholder Register
**TBD**

## Team Agreement

**TBD**


#### **Meetings:**
- One standing team meeting per week, over Discord voice, lasting up to an hour.
- Attendance is expected. If you can't make it, you tell the team in advance and read the notes.

#### **Decision-making:**
- We talk about it and agree.
- Anything that changes scope, budget, or a milestone is escalated to the Project Lead and confirmed with the sponsor/instructor before we act on it.

#### **Task Ownership:**
- All work is tracked as GitHub Issues on a shared project board.
- Every task has one named owner and a due date. "Owned by everyone" means owned by no one, so we avoid it.
- The owner is responsible for the task getting done.

#### **Conflict resolution:**
- Talk directly and professionally with the person involved first.
- If it isn't resolved within 24 hours, bring it to the full team at the next sync (or sooner) and decide together.

#### **Missed work and absences:**
- Give as much notice as possible if you'll miss a deadline or a meeting, and propose how your part will be covered.
- A missed task is re-assigned or rescheduled by the team so the milestone isn't put at risk.

#### **Professional conduct:**
- We treat each other with respect, assume good faith, and keep feedback about the work, not the person.
- We meet the commitments we make, and we're honest early when we can't.
- We follow academic-integrity rules: the work we submit is our own, sources are cited, and every member understands the work well enough to explain and defend it.
 

## Repository & Workspace Evidence
The project workspace is a private GitHub repository that only team members and the instructor can access. It holds both the codebase and the documentation, so every decision and change is tracked and attributable.

Repository: [RAMP GitHub](https://github.com/PurabPriyani/RAMP/tree/main)  
Access: Private; team members added as collaborators with write access; instructor invited as a collaborator/viewer.