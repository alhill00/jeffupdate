# MXY Chief of Staff — Project Brief
*Last updated: 2026-08-21 | Maintained by Claude Code for use in Claude mobile app*

Upload this file to your MXY Chief of Staff project Knowledge on claude.ai to give mobile Claude full context on everything built in terminal sessions.

---

## Who You Are
**Alex Hill** — Senior Manager, Learning & Development at Breeze Airways. 6 years at Breeze. Reports to CPO Jeff Weber. Manages Carlin Clark (PhD, HCM). People-oriented leader, not a coder — uses Claude Code to build tools and programs that would otherwise require a dev team. Working toward VP readiness.

**Key relationships:** Jeff Weber (CPO, direct leader), Dina (TMX, partner on career pathing), Brent (assessment/consulting partner), Carlin Clark (direct report, program delivery), Cam (career pathing advocate), Yakir (exec onboarding guinea pig)

---

## Active Projects & Current State

### 1. Breeze Leader Guide (`breeze-leader-guide.html`)
**What it is:** A single offline HTML file — the central leadership development platform for 266 Breeze leaders. Self-contained, no server required, works in any browser.

**Current state (as of Aug 21):**
- 6 tabs: My Journey, First 90 Days, Next 90 Days, My Skills, Onboard My Team, Resources
- Level selector (Supervisor / Manager / Director / VP) personalizes content
- **5 leadership values** displayed as a persistent strip in the sticky nav bar — always visible
- **51 training modules** — 6-step interactive modules for every skill card
- **Skills tab** reorganized: all skills mapped to the 5 leadership values as group headers
- **LD Offerings section** added to My Journey tab: 10 offering cards
- **First 90 Days** restructured: 4 phases — Week 1: Start Here (new), First Month, Month 2, Month 3
- Week 1 links directly to Onboard My Team tab for new leaders
- **Resources tab:** Full Workday Job Req guide embedded with FAQ, process table, and talent team contacts
- **Skill counts:** Supervisor 11 | Manager 15 | Director 13 | VP 12
- **GitHub:** Pushed to github.com/alhill00/leaderguide — GitHub Pages enabled at alhill00.github.io/leaderguide

**Not yet done:**
- Hiring & Selection skill (waiting on recruiting team materials)
- Resource URLs for skill cards (all currently null — Phase 2)

**File location:** `C:\Users\AlexHill\OneDrive - Breeze Aviation Group\Documents\Breeze\claude code\breeze-leader-guide.html`

---

### 2. My Skills Deep-Dive Courses (`course_[level]_[skill].html`)
**What it is:** 17-screen interactive HTML courses for every skill in the Leader Guide. One course per skill card. Self-contained offline files, organized by level for SharePoint deployment.

**Architecture:** TOTAL=17, SECTION_MAP=[0,0,0,1,0,1,1,2,2,2,3,3,3,3,3,4,5], 6 sections: Foundation → Framework → Practice → Pulse Check → Apply It → Complete. localStorage persistence, no server required.

**Color schemes by level:**
- Supervisor: `--accent:#0077A8` (teal), `--accent-light:#d0eef7`, header `#0a3d4a→#000633`, body `#f4fbfd`
- Manager: `--accent:#174DFF` (Breeze Blue), `--accent-light:#e0e8ff`, header `#000633→#0d1f6e`, body `#f5f7ff`
- Director: `--accent:#6D28D9` (purple), `--accent-light:#ede9fe`, header `#1a0a3d→#000633`, body `#faf8ff`
- VP: `--accent:#000633` (dark navy), `--accent-light:#eef2ff`, header `#000633→#000d4d`, body `#ffffff` — near-monochrome, Breeze Blue (#174DFF) used only for progress bar and active pill

**Current build status (as of Aug 21):**

**SUPERVISOR (7/7 — COMPLETE)**
- course_sv_effective_1on1s.html
- course_sv_eq.html
- course_sv_communicating_clearly.html
- course_sv_running_meetings.html
- course_sv_managing_former_peers.html
- course_sv_time_management.html
- course_sv_recognizing_team.html

**MANAGER (15/15 — COMPLETE)**
- course_mg_coaching_performance.html ← also serves as template
- course_mg_delegating.html
- course_mg_psych_safety.html
- course_mg_reading_room.html
- course_mg_sustainable_leadership.html
- course_mg_performance_reviews.html
- course_mg_managing_conflict.html
- course_mg_goal_setting.html
- course_mg_decision_making.html
- course_mg_communicating_clearly.html
- course_mg_running_meetings.html
- course_mg_cross_functional.html
- course_mg_change_management.html
- course_mg_managing_up.html
- course_mg_developing_reports.html
- course_mg_retention_conversations.html

**DIRECTOR (10/12 built — 2 in progress)**
Built:
- course_dr_high_performing_culture.html
- course_dr_influencing_without_authority.html
- course_dr_data_driven_decisions.html
- course_dr_blind_spots_at_scale.html
- course_dr_communicating_clearly.html
- course_dr_running_meetings.html
- course_dr_managing_up.html
- course_dr_executive_presence.html
- course_dr_change_management.html
- course_dr_financial_acumen.html
In progress (agent running):
- course_dr_coaching_managers.html
- course_dr_succession_planning.html

**VP (8/12 built — 5 in progress)**
Built:
- course_vp_culture_architecture.html
- course_vp_presence_under_pressure.html
- course_vp_exec_presence_scale.html
- course_vp_growth_change.html
- course_vp_comms_at_scale.html
- course_vp_stakeholder_comms.html
- course_vp_leading_uncertainty.html
- course_vp_vision.html
In progress (agent running):
- course_vp_org_design.html
- course_vp_business_owner.html
- course_vp_senior_teams.html
- course_vp_talent_strategy.html
- course_vp_leadership_pipeline.html

**Next steps after build complete:**
- Commit all course_*.html files to leaderguide GitHub repo
- Update breeze-leader-guide.html skill card resource URLs with SharePoint links (Phase 2)
- Upload courses to SharePoint organized by level folder

---

### 3. Leadership in 5 (`Leadership_in_5_*.html`)
**What it is:** Weekly Tuesday microlearning — one leadership concept, 5 minutes, delivered via HTML email/page.

**Current state:** Built through Sep 1 (RepairAfterConflict). Monthly Sway book breakdowns also built. Engagement tracking strategy in place.

---

### 4. New Leader Orientation (NLO)
**What it is:** 6-week intensive + 6-month coaching for new leaders.

**Current state:** 5 files built (CBTs, Session 1, facilitator guide, scripts, schedule). Still to build: Sessions 2, 3, and Capstone live session HTMLs.

---

### 5. Breeze Pulse
**What it is:** Quarterly team engagement survey system. 4 survey types, question-to-heatmap mapping, dashboard tiers.

**Current state:** Architecture designed. Launch slides built. CXO presentation built.

---

### 6. Leader Scorecard (`breeze-pulse-leader-scorecard.html`)
**What it is:** Individual leader feedback dashboard — quarterly 360-style from their team.

**Current state:** Generator script built. Pilot = Parker Tyler (June 2026). Can be run for any leader by changing 2 lines.

---

### 7. Career Pathing
**What it is:** Dina-led initiative (NPS response). Skills + Primers + Signals framework. Alex is co-admin.

**Current state:** Planning & Revenue (Max Baris) is the first department. Frame as skill development, NOT promotion timelines. TMX is the point person — Brent flagged comp/timeline expectation-setting needed (same title ≠ same comp, no rigid timelines).

---

### 8. Flight Ops Leadership Course
**What it is:** 6-module curriculum for technical-to-people leaders. John Russack initiative (retiring Oct 15). CRM as the conceptual bridge.

**Current state:** Outline built. Module 1 HTML built. Outline was due ~Aug 18.

---

### 9. 30-60-90 Onboarding App (`onboarding-journey/`)
**What it is:** Leader + new hire + admin onboarding tool. localStorage-based.

**Current state:** Built and functional. Dina presented to CXO mid-July. Cloudflare deployment needed for full rollout.

---

### 10. OCC Leadership Program
**What it is:** Operations Control Center leadership sessions — 4-session program.

**Current state:** All 4 session companions + facilitator display + takeaway cards built.

---

### 11. Promotion Readiness Program (separate from My Skills courses)
**What it is:** 20 interactive HTML training modules (5 per level) using a different 4-section structure: Hook → Concept → Scenario → Pulse Check. Different from the 17-screen My Skills courses.

**Current state:** Supervisor 5 modules complete. Manager 5 modules in progress. Director/VP planned.

**Color schemes for THIS program (different from My Skills courses):**
- Supervisor: `#174DFF` Blue, bg `#f4f6fb`
- Manager: `#000633` Navy, `#FED4A4` Tan accent, bg `#f7f5f1`
- Director: `#FF527B` Red, Tan surfaces, bg `#FFF5BD` (planned)
- VP: near-monochrome `#000633`, bg `#FFFFFF` (planned)

---

## Key Strategic Context

**The core gap (confirmed by Brent + Jeff):** Tools and programs exist. Leaders don't know. Visibility is the problem, not the content. Jeff wants a "mini PR campaign." Yakir is the guinea pig for the leader guide rollout.

**Brent's Aug 12 findings:**
- L&D visibility is the gap (not the programs)
- Career pathing: needs expectation-setting on comp and timelines
- Exec onboarding: limited by the "David Factor" (David pulls new leaders to operational fires immediately)
- Succession: Jeff/Mark/Brent conversation at exec level
- JetBlue hire risk: Donna hiring almost exclusively from JetBlue — institutional knowledge concern

**Jeff's priorities:** eNPS visibility, career pathing, leader guide rollout, succession planning structure.

---

## Tools & Technical Notes
- All HTML files are self-contained (offline, no server needed)
- localStorage for all persistence in interactive tools
- File save location: `Documents\Breeze\claude code\`
- GitHub repos:
  - `github.com/alhill00/jeffupdate` — general work
  - `github.com/alhill00/leaderguide` — leader guide + courses (Pages enabled at alhill00.github.io/leaderguide)
- OneDrive sync means files are accessible on iPhone via Files app
- Course file naming: `course_[sv/mg/dr/vp]_[skill_slug].html`

---

## How to Use This Brief on Mobile
When starting a phone conversation in the MXY project, Claude will already know everything above. You can:
- Ask about the status of any project
- Continue building (describe what you want and Claude will draft it for you to bring back to terminal)
- Use Claude to think through decisions, draft communications, or plan next steps
- Ask Claude to draft additions to the Leader Guide — you can paste them into a terminal session to implement

*Re-upload this file to project Knowledge when it gets significantly out of date.*
