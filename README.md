<div align="center">
  
# Just Dump It by Jeys

![Logo](images/just-dump-it-logo.png)

</div>

**Team:** Jesslyn Wong Mei Chui, Janet Beh Jing Le, Lee Jean Suen, Wong Jun Hong  
**Problem Statement:** Stress & Workload Manager  
**Video Presentation:** 
<a href="https://youtu.be/6YlUAF7AdU8">
  <img src="https://img.shields.io/badge/YouTube-Video_Presentation-red.svg"/>
</a><br>
**Presentation Slides:** 
<a href="https://canva.link/82w2fdwxvyyn5ws">
  <img src="https://img.shields.io/badge/Canva-Presentation_Slides-00C4CC.svg"/>
</a>

<div align="justify">

## 1. Problem Overview

### The Problem

Students often have to balance academic work, part-time jobs, social commitments, errands and personal activities at the same time. The challenge is not always a single overwhelming task, but the cumulative load of multiple manageable commitments happening together. Students may struggle to recognise when their overall schedule is becoming unsustainable and what commitments can be adjusted when they become overloaded. This results in *stress, exhaustion, burnout, procrastination and reduced wellbeing*.

The main causes we identified are *overcommitting to their many tasks, limited awareness of cumulative workload, and difficulty deciding what to move, reduce or postpone*.

*Stakeholders:*
- *Students* — primary users who manage academic, work, social and personal commitments.
- *Educational institutions* — interested in supporting sustainable study habits and student well-being.
- *Student organisations and employers* — contribute commitments that students need to balance.

Existing planning applications such as *Sunsama* provide workload-aware daily planning and help users handle overcommitted schedules. However, its workload approach focuses primarily on planned time and workload thresholds, rather than combining workload with students' own stress experiences and helping them explore different ways to rebalance their schedules.

### Our Solution

**Just Dump It** is a student-focused workload-management planner designed to help students recognise and manage excessive workload before it becomes overwhelming. It assesses scheduled activities based on their duration, category and effort, while allowing students to record their own stress levels. When a schedule becomes too demanding, the system helps students explore ways to rebalance their commitments rather than simply warning them that they are overloaded. AI supports this process by organising unstructured tasks and suggesting possible schedule reorganisations, while students remain in control of the final changes.

**Feature Set:**
* Core Planner & Calendar
* Workload-Aware Planning
* Stress Check-ins
* Just Dump It
* Playground
* AI Reorganisation Suggestions
* Workload & Stress Insights
* Recovery Suggestions
* Google Calendar Integration

</div>

## 2. Ideation & Process

### 2.1 Ideas We Considered


| **Idea** | **Why it was dropped / kept** |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Unstructured task input | Kept. Allows students to get tasks and thoughts out of their head without deciding how to organise and create them first. |
| Playground | Kept. Students can experiment with moving and rearranging activities to make an overloaded schedule more manageable without changing the existing schedule first. |
| Workload & Stress Analytics | Kept. Combines workload and self-logged stress over time to identify personal patterns and support earlier recognition of potentially heavy days in the future. |
| Google Calendar Integration | Kept. Allows students to bring in existing calendar commitments especially from work and clubs without manually scheduling them again. |
| Smartwatch Connectivity | Dropped. Potentially useful for quick recovery interactions that can be included in future enhancements, but currently outside of the initial core scope. |
| Weighted Capacity Calculation Model | Dropped (changed). Initially explored calculating capacity using weighted Time, Mental, Physical and Social dimensions. This was simplified into the current activity-based model using Duration, Category Multiplier and Effort Multiplier |

### 2.2 Ideation Boards


**2.2.1 Understanding the Problem**

*We mapped the main causes and effects of student overload, leading us to focus on helping students understand, visualise and rebalance their overall load.*

![Understanding the Problem](images/problem-understanding.jpeg)

**2.2.2 Initial Braindump**

*Our initial brainstorming includes problem evaluation, possible feature ideas and considerations.*

![Initial Braindump](images/initial-braindump.png)

**2.2.3 Userflow**

![Userflow](images/userflow.jpeg)

**2.2.4 Refining the Workload Model**

*These are the workload calculation approaches we explored. The first image is one of our experimentation, which was later dropped, while the second image is the current approach used in our solution along with the test cases.*

![Previous Workload Model](images/workload-model-before.png)

![Current Workload Model](images/workload-model-after.png)

### 2.3 Mentor Consultation

| **Date** | **Mentor** | **Feedback Received** | **What Was Changed** |
| ------------------- | ---------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 2nd September 2026 | Mah Qing Fung | Avoid relying heavily on numerical values in the UI. | We shifted towards qualitative workload states and recommendations rather than displaying workload capacities as percentage scores to users. |
| 2nd September 2026 | Mah Qing Fung | Present the solution through a Scenario -> Demo -> Impact flow. | We revised our initial presentation structure to follow the advised flow which is more story-like compared to our initial structure which is towards a more informational structure. |
| 10th September 2026 | Khor Jia Quan (Stefan) | The Suggestion tab/button in the Playground section was too unnoticeable. | Increase the visibility of the Suggestion button by changing the location and design of it. |
| 10th September 2026 | Khor Jia Quan (Stefan) | The current colour combination was not visually appealing. | Changed the colour palette and design to be more simplistic to create a cleaner and more cohesive visual design. |

## 3. Design & Prototype

**UI Prototype:**
<a href="https://www.figma.com/proto/d9tsHy0Ib46HYgi60zU0ey/CodeNection_TeamJeys_FigmaPrototype?node-id=1158-2893&t=tjp0LcGaE0zZyzBj-1&scaling=scale-down&content-scaling=fixed&page-id=762%3A440&starting-point-node-id=1158%3A2893K">
  <img src="https://img.shields.io/badge/Figma-UI_Prototype-F24E1E.svg"/>
</a>

## 4. What Makes It Different

<div align="justify">
  
**Workload-Aware Planning**

Assesses each activity based on its duration, category and effort to identify how demanding a schedule is. When a new task makes a day too packed, the system proactively suggests moving or shifting a flexible, lower-priority task to create space, or reconsider the task.

**Playground**

Lets students experiment with different ways to rebalance their schedule without immediately changing their actual calendar. Users can move schedule blocks, see workload status change visually, and receive suggestions for better task arrangements and recovery times.

**Just Dump It**

Lets students enter tasks and thoughts freely without organising them first. AI transforms the messy unstructured input into structured activities that can be reviewed and added to the schedule.

**Stress and Workload Insights**

Combines planned workload with self-reported stress to reveal patterns over time. Students can understand when and where their schedules tend to become unsustainable. If students consistently report high stress at lower workload levels, the system can adapt their personal threshold, allowing it to flag potentially heavy days earlier and provide more personalised recommendations.

</div>

### Comparison Table

| **Factor** | **Google Calendar** | **Sunsama** | **Structured** | **Burnout Planner** |
| ------------------------------------------- | ------------------- | ----------- | -------------- | ---------------- |
| Calendar & Task Planning | / | / | / | / |
| Workload Awareness | x | / | x | / |
| Freeform Input | x | / | / | / |
| AI-Assisted Task Organisation & Rebalancing | x | / | / | / |
| Workload & Stress Insights | x | x | x | / |

<div align="justify">

*Note: Some competitor capabilities are available only under paid plans or subscriptions. For example, Structured AI and Replan are Structured Pro features, while Sunsama provides full access during its 14-day trial and requires a subscription afterward.*

</div>

## 5. Technical Architecture & Feasibility

**Tech stack**

| **Layer** | **Technology** | **Purpose** |
| ------------------- | ------------------- | --------------------------------------------------------- |
| Frontend | React Native + Expo | Mobile app interface and interactions |
| Language | TypeScript | Planner, workload and scheduling logic |
| Backend & Database | Supabase | Authentication, database and backend services |
| AI Service | Gemini API | Task organisation and schedule reorganisation suggestions |
| Calendar API | Google Calendar API | Sync existing calendar events |
| Development & Build | Expo Go + EAS | Device testing and application builds |
| Hosting | Supabase + EAS | Backend hosting and app builds |

| **Technology** | **Why We Chose It** | **Expected Constraints** |
| ------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| React Native + Expo | Cross-platform development with a simple development workflow | Team has limited prior experience |
| TypeScript | Type safety and structured development | Complex integrations, particularly AI-generated data, require careful type handling and validation |
| Supabase | Combines authentication, PostgreSQL and backend functions in one platform | Free-tier and Edge Function limitations |
| Gemini API | Supports AI-powered interpretation and recommendations | AI responses may be inconsistent or unsuitable, while API quotas and network latency may affect availability |
| Google Calendar API | Allowing commitments to be synced without additional hassle | OAuth and API quotas add integration complexity |
| Expo Go + EAS | Simplifies testing and application builds | Team has limited prior experience |

**Build plan & scope**


| **Week** | **Plan** |
| -------- | -------- |
| **1** | - Setup (React Native, Expo, Supabase)<br>- Authentication<br>- Core Screens<br>- Workload Calculation<br>- Workload Status |
| **2** | - Just Dump It<br>- Playground<br>- Gemini AI integration<br>- Stress logging<br>- Overload - stress logic<br>- Google Calendar |
| **3** | - Analytics<br>- Recovery Suggestions<br>- Connect Core Features<br>- Testing and Debugging<br>- UI Polish<br>- Prepare Final Demo |
