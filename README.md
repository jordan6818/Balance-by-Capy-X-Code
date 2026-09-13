# Balance-by-Capy-X-Code
An application designed to help students who are experiencing schedule fatigue. It is devoted to measuring students' stress levels and recommending better daily schedule modifications to minimise users's stress levels.
# Balance by Capy X Code

**Team:** Shing Zhun Kit, Cheang Xin Yan, Hew Wei Cheng, Lau Jin Yee  
**Problem Statement:** [Stress & Workload Manager]  
**Video Presentation:** [Unlisted Youtube Link]  
**Presentation Slides:** [https://canva.link/5e49afzrq498irj](https://canva.link/5e49afzrq498irj)

---

## 1. Project Overview

### The problem:
University students have to handle academic work, part-time jobs, personal errands, and social commitments all at the same time, but rarely have visibility into how these demands add up across their week. Burnout doesn't come from one overwhelming event, it builds gradually as tasks, deadlines, and commitments accumulate silently across separate areas of life (academic, work, social, personal) until the total load becomes unsustainable. The problem is not simply having too many tasks. The problem is that students often cannot see how all these commitments interact with their available time.

### Causes:
- Lack a single place to see their full workload clearly.
- Lack of a single place to view academic, work, personal and social commitments together.
- Students may underestimate the total amount of time required to complete their tasks.
- Existing productivity tools often focus on individual tasks or events rather than the user's overall workload.
- Deadlines may accumulate within a short period of time.
- Students may have limited visibility of their actual available time.
- Schedule conflicts may only become obvious after commitments have already been made.
- Recovery and free time are often treated as leftover time rather than something that should be protected.
- Students may know that they are busy but do not know which changes would actually make their schedule more manageable.

**Stakeholders:** University student

### Similar app:
Existing solutions address only fragments of this problem. Task management apps like Todoist help users track and organize tasks, but they treat every task as a to-do list item without accounting for the user's actual available time, energy, or how workload is distributed across different life categories. A student using Todoist can see what they need to do, but not whether their week is realistically overloaded. It also offers no mechanism for identifying overload proactively or suggesting how to rebalance a schedule before it becomes unmanageable.

### Our Solution:
Balance is a workload and stress management app for university students. The goal is not to medically diagnose or directly measure psychological stress. Instead, Balance helps students understand their workload, identify periods of overload, intelligently rebalance their schedules, and protect recovery time.

### Feature set:
1. **Workload Check-in** - Users input their upcoming tasks, estimated hours, deadlines, classes, work shifts, and personal/social commitments, giving Balance a real picture of their week.
2. **Workload Score** - A visual, at-a-glance status (e.g. HIGH / MODERATE / LOW) showing how loaded the student's week is relative to their available time, paired with a plain-language explanation of why.
3. **Overload Detection** - Balance identifies specific overload conditions (e.g. deadline clustering, planned hours exceeding available time, insufficient recovery time) and explains the reasons behind the overload rather than issuing a vague warning.
4. **AI Rebalancing** - Balance's AI analyzes the workload and proposes concrete adjustments - moving flexible tasks, reducing non-essential commitments, prioritizing what matters most, and breaking large tasks into manageable steps.
5. **What-If Simulation** - Users can test a hypothetical schedule change (e.g. "move this assignment to Friday") and see how it affects their workload score before committing to it.

---

## 2. Ideation & Process

### 2.1 Ideas We Considered

Table of every distinct idea generated, with why each was kept or dropped, ordered so that chosen ideas are listed first:

| Idea | Why it was dropped / kept |
| :--- | :--- |
| **Data-Driven Workload Tracker (Chosen)**<br>Users input objective workload data, and the system calculates and visualizes their overall load, with AI suggesting how to rebalance tasks. | **Chosen** because it directly targets the core problem - students lacking visibility into their total load, and it produces concrete, actionable output rather than just emotional support. |
| **Mood-First Journaling App**<br>Centered on daily mood journaling or voice logs | **Dropped** because it addresses how students feel without addressing why - it doesn't help users see or fix the actual overload causing the stress, so it risks becoming a tracker without a real intervention. |
| **Environmental Intervention App**<br>Focused on removing users from overload environments directly, using auto-blocking notifications, locking the phone for set periods, or suggesting nearby places to unwind. | **Dropped** because it treats the symptom (inability to disengage) without addressing the root cause (the student not knowing their workload is unsustainable in the first place), and relies on phone-level permissions that add technical complexity without adding insight. |

---

### 2.2 Ideation Boards

![Mindmap](mindmap.jpg)
*Image 1. Product Mind Map*

This flow diagrams a product strategy framework for a task management tool designed to prevent burnout while boosting productivity.

#### 1. Problem Space (The "Why")
- **User Problem:** Core pain points centered on overwhelm, poor visibility over workload, and the toxic cycle of high productivity leading to burnout.
- **Target Users:** Students, young adults, and individuals balancing complex, overlapping commitments who need lightweight, low-friction systems.

#### 2. Core Strategy (The "Bridge")
- **Balance:** Acts as the strategic pivot point, aligning user needs directly with brainstorming solutions.
- **User Needs vs. Ideation:** Pairs fundamental user requirements (e.g., organise, stay motivated) against conceptual feature ideas (e.g., AI assistance, gamification) to ensure every feature addresses a real demand.

#### 3. Solution Execution (The "How")
The strategy translates ideation into five functional feature pillars under Selected Solutions:
- **Task Management:** Core CRUD actions (adding, categorizing, prioritizing, and completing tasks).
- **Weekly Balance:** High-level capacity planning to visualize and manage workload intensity (Low, Moderate, High).
- **AI Support:** Smart automation to handle task creation and structural suggestions, reducing cognitive load.
- **Gamification:** Weekly results to sustain long-term engagement and detailed statistics.
- **Progress & Feedback:** Visual feedback loops tracking completion metrics and personal growth.

#### 4. Outcome (The "Impact")
- **Expected Impact:** The downstream results of the system—shifting users from feeling overwhelmed to achieving structured organization, clearer prioritization, workload self-awareness, and a sustainable productivity routine.

---

### 2.3 Mentor Consultation

| Date | Mentor | Feedback Received | What Was Changed |
| :--- | :--- | :--- | :--- |
| **11/09/2026** | **Daniel Koh Yu Hang** | **Prototype Feedback Summary**<br><br>**1. Overall scoring / score calculation**<br>- Clarify how the overall score is calculated. Explain the breakdown of the score, including how the AI or algorithm contributes to the final score.<br>- Make the scoring criteria more consistent and transparent so users understand why they received a particular score.<br><br>**2. AI-generated recommendations**<br>- Introduce a strict and structured set of instructions for the AI so that its recommendations are consistent.<br>- The AI should explain or make clear why it is making a particular decision/recommendation.<br>- Consider making the AI's decision-making more controlled rather than allowing overly open-ended recommendations.<br><br>**3. Calendar integration**<br>- Add a calendar feature directly into the app.<br>- Allow users to sync their existing calendars, particularly: Google Calendar & Apple Calendar. This would make the recommendations more actionable by allowing users to incorporate suggested activities/tasks into their schedules.<br><br>**4. AI chatbot**<br>- The current chatbot was seen as not engaging enough.<br>- Improve the chatbot so it feels more interactive and useful rather than simply responding to users.<br>- Consider adding functionality where the AI can automatically extract a task from a conversation and turn it into something actionable.<br>- For example, if the user mentions a task/deadline in conversation, the AI could recognise it and potentially create a task/reminder.<br><br>**5. Rewards / streak system**<br>- The streak feature is currently not implemented and was identified as something that could be developed further.<br>- User engagement and continued app usage should be driven primarily by the strength of the system flow and UX itself, not by an external reward mechanic like a daily streak counter.<br><br>**6. Score analysis / wellbeing recommendations**<br>- The prototype currently shows something like a current score vs. target score.<br>- The feedback suggests making this more useful by providing personalised recommendations based on the user's situation.<br>- For example, if the user's score indicates they are overwhelmed/stressed, the app could recommend: Taking a break, Going for a walk, or other appropriate wellbeing activities.<br>- Also consider providing more ways to interpret or explore the statistics, rather than only presenting one score. | All feedback received during the prototype evaluation has been carefully reviewed, considered, and addressed accordingly. Each identified area for improvement was evaluated based on its relevance to the user experience and the overall objectives of the application.<br><br>The prototype has subsequently been modified and enhanced to reflect the feedback received, with the relevant improvements implemented accordingly. These changes include improvements to the scoring system, AI recommendations and decision-making, calendar integration, AI chatbot functionality, personalised recommendations, and statistics/analysis.<br><br>The modifications were not implemented superficially. Each change was thoroughly considered in terms of its purpose, usability, and contribution to solving the identified problems. The revised prototype therefore demonstrates how the feedback has been translated into tangible improvements rather than simply being acknowledged.<br><br>Overall, the updated prototype aims to provide a more transparent, engaging, personalised, and actionable user experience, while ensuring that the proposed features remain aligned with the original problem statement and target users. |

---

## 3. Design & Prototype

**UI Prototype:** [LINK TO PROTOTYPE]

*Check that it opens in an incognito window. This can be a link to Figma, Canva, Netlify, Vercel or any other board where you showcase your UI. It can be clickable with hyperlinks or simply ordered screenshots.*

*We recommend you embed or link 4-8 key screens as images, with a caption on each explaining the interaction.*

| Screen 1 | Screen 2 |
| :---: | :---: |
| ![Login Page](login_page.png)<br>**Login Page** | ![Show Workload Score, Upcoming Task](dashboard.png)<br>**Show Workload Score, Upcoming Task** |
| ![Add Task](add_task.png)<br>**Add Task** | ![Weekly Overview](weekly_overview.png)<br>**Weekly Overview** |
| ![AI Rebalancing](ai_rebalancing.png)<br>**AI Rebalancing** - AI analyzes the workload and proposes concrete adjustments | ![What-if Simulation](what_if_simulation.png)<br>**What-if Simulation** - Test a hypothetical schedule change and see how it affects workload score before committing |
| ![AI Chatbot](ai_chatbot.png)<br>**AI Chatbot** | ![Overload Detection](overload_detection.png)<br>**Overload Detection** - Show main pressure point, most urgent tasks |

---

## 4. What Makes It Different

Compared to conventional tools, this prototype acts as an active workload balancer and motivation engine rather than a passive list or calendar. Traditional options record what you need to do, but leave the mental overhead of prioritizing, pacing, and preventing burnout entirely on you.

### Key Differentiators
- **Active Workload Balancing:** Unlike Google Calendar or Apple Calendar—which let you endlessly stack events until your day is overbooked—this system tracks workload density (Low, Moderate, High) to highlight overcommitment before burnout happens.
- **AI Assistance & Structuring:** Tools like Notes, paper, or basic sticky notes are completely manual. The prototype uses AI to auto-create tasks, suggest structures, and lower the friction of entering data.
- **Built-in Gamification & Motivation:** Standard calendar and note apps treat task completion as binary checkmarks. This system builds in behavioral rewards (badges, progress insights, achievements) to keep young adults and students engaged over long periods.
- **Dynamic Prioritization vs. Static Notes:** Sticky notes and paper planners quickly become messy, static lists that offer no automatic re-prioritization. This prototype breaks tasks into actionable categories with visual priority structures.

### Comparison Table

| Feature / Metric | Our Prototype | Google / Apple Calendar | Notes Apps (Apple Notes, Keep) | Paper / Sticky Notes |
| :--- | :--- | :--- | :--- | :--- |
| **Primary Focus** | Balanced productivity & burnout prevention | Time-blocking & scheduling | Unstructured thoughts & quick lists | Low-tech capture & tactile focus |
| **Workload Awareness** | **High:** Explicitly measures low/moderate/high density | **Low:** Shows time, but doesn't prevent overbooking | **None:** Raw list length without time/capacity context | **None:** Relies entirely on manual visual estimation |
| **AI Task Structuring** | **Yes:** Suggests structure & auto-creates tasks | **No:** Manual entry (or basic parsing) | **No:** Plain text entry | **No:** Fully manual handwriting |
| **Burnout Safeguards** | **Built-in:** Balance tier connects needs to workload limits | **None:** Permits infinite overlapping events | **None:** No dynamic workload tracking | **None:** Static format leads to overwhelming lists |
| **Motivation System** | **Gamified:** Badges, achievements, progress feedback | **None:** Functional calendar blocks | **None:** Simple checkable circles | **Tactile:** High satisfaction from physically crossing off |
| **Input Friction** | **Low:** AI assists entry and categorization | **Moderate:** Requires time, date, and detail fields | **Low:** Fast typing, but lacks organization | **Low:** Instant writing, but messy to update/rearrange |

*Table 1. Comparison Table*

---

## 5. Technical Architecture & Feasibility

### Tech Stack & Architecture

#### 1. Technology Choices & Constraints
- **Frontend:** Next.js (React) with Tailwind CSS & shadcn/ui
  - *Why:* Fast server-side rendering, component modularity, and rapid UI development tailored for dashboards and micro-interactions.
  - *Constraints:* Managing complex client-side state for real-time drag-and-drop task ordering alongside server-rendered data hydration can add state complexity.
- **Backend:** Next.js API Routes (Node.js Serverless Functions)
  - *Why:* Keeps full-stack development in a single unified codebase, eliminating separate server maintenance.
  - *Constraints:* Vercel serverless functions have execution time limits (10-15 seconds). Longer AI generations will require streaming responses via server-sent events (SSE) rather than traditional waiting calls.
- **Database & Authentication:** Supabase (PostgreSQL + Supabase Auth)
  - *Why:* Built-in Row Level Security (RLS) ensures tenant data isolation, instantly handles OAuth/Email login, and Postgres allows easy relational queries across users, tasks, and weekly metrics.
  - *Constraints:* The free tier pauses inactive projects after extended idle periods and caps connection pools. A connection proxy (Supabase HyperGBound/Supabase Pooler) is required for serverless connections.
- **APIs & AI Services:** OpenAI API (`gpt-4o-mini`) via Vercel AI SDK
  - *Why:* `gpt-4o-mini` offers near-instant structured JSON parsing for breaking down vague text inputs into dynamic micro-tasks at an affordable operational cost.
  - *Constraints:* API latency and rate-limiting require strict client-side validation, error handling fallbacks, and token budgeting.
- **Hosting & Infrastructure:** Vercel (Frontend & Serverless Backend)
  - *Why:* Out-of-the-box integration with GitHub, zero-config CI/CD previews, global edge routing, and seamless deployment for Next.js apps.
  - *Constraints:* Bandwidth and execution limits on free/hobby tiers require strict optimization of payload sizes.
- **Cost:** Low cost implementation requirement.

---

#### 2. System Architecture Diagram

```
+-------------------------------------------------------+
|                    Client (Browser)                   |
|     Next.js (React) UI + Tailwind CSS + Framer Motion  |
+---------------------------+---------------------------+
                            |
       (Auth / Data Sync)   |   (AI Prompts / Streaming)
               +------------+------------+
               |                         |
               v                         v
+------------------------------+ +------------------------------+
|       Supabase Engine        | |     Next.js API Routes       |
| +--------------------------+ | |    (Vercel Serverless)       |
| |   Supabase Auth (JWT)    | | +--------------+---------------+
| +--------------------------+ |                |
| |   PostgreSQL Database    | |                | (OpenAI SDK)
| |   (Tasks, Users, Stats)  | |                v
| +--------------------------+ | +------------------------------+
+------------------------------+ |          OpenAI API          |
                                 |     (gpt-4o-mini Parsing)    |
                                 +------------------------------+
```
*Image 2. System Architecture Diagram*

---

#### 3. Build Plan & Scope (MVP Phase)

To ensure delivery within a realistic timeframe, the building phase will focus exclusively on core task balancing and foundational AI support, reserving advanced social gamification features for post-MVP releases.

##### In Scope (What We Will Build):
- **Auth & User Profile:** Email/Password authentication and basic profile onboarding.
- **Task CRUD & Prioritization:** Ability to add, categorize, set priorities, and mark tasks as complete.
- **Weekly Balance Indicator:** A visual metric dashboard calculating daily task load and categorizing overall capacity (Low, Moderate, High).
- **AI Task Creator (1-Click Breakdown):** Input prompt (e.g., "Finish physics project") parses into 3-4 sub-tasks automatically structured by priority.
- **Basic Gamification & Progress:** Streak counters and progress completion percentages (badges deferred).

##### Out of Scope (Deferred to Next Iterations):
- Complex social leaderboards, custom achievement badges, and multiplayer team capabilities.
- Third-party calendar sync integrations (Google Calendar / Outlook API integration).
