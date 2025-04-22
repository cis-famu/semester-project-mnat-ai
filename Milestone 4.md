# **Milestone 4**

**Table of Contents**
1. [Meeting Minutes](#Meeting-Minutes)
2. [Risk Register](#risk-register)
3. [Collection Relationship Diagram](#Collection-Relationship-Diagram)
4. [Data Dictionary](#Data-Dictionary)
5. [Lessons-learned report](#Lessons-learned-report)
6. [Poster](#poster)
7. [MNat.ai Poster presentation](#MNat.ai Poster presentation)
# Meeting Minutes

# Meeting Notes

---

## 2/17/2025 — 1:00 PM

**Attendance:**
- Ronnie Burns II  
- CJ Mitchell  
- Jamal Person  
- Jarrett Gilbert

**Agenda:**  
Milestone 1

**Minutes:**
- 1:00 PM — Discussed what the milestone entailed and addressed any concerns or questions.  
- 1:15 PM — Delegated tasks to appropriate members.

---

## 2/24/2025 — 5:30 PM

**Attendance:**
- CJ Mitchell  
- Jamal Person  
- Jarrett Gilbert

**Agenda:**  
Milestone 2

**Minutes:**
- 5:30 PM — Discussed milestone details and resolved any questions.  
- 6:15 PM — Delegated tasks to appropriate members.

---

## 3/17/2025 — 5:34 PM

**Attendance:**
- CJ Mitchell  
- Jamal Person  
- Jarrett Gilbert

**Agenda:**  
Milestone 3

**Minutes:**
- 5:34 PM — Discussed milestone scope and clarified responsibilities.  
- 5:44 PM — Delegated tasks to appropriate members.

---

## 3/31/2025 — 5:30 PM

**Attendance:**
- CJ Mitchell  
- Jamal Pearson

**Agenda:**  
Milestone 4

**Minutes:**
- 5:30 PM — Discussed milestone requirements and resolved questions.  
- 6:04 PM — Delegated all tasks to the appropriate members.

---

## 4/13/2025 — 1:30 PM

**Attendance:**
- CJ Mitchell  
- Jamal Pearson  
- Jarrett Gilbert  
- Ronnie Burns

**Agenda:**  
Milestone 4 – Updates and Poster Planning

**Minutes:**
- 1:30 PM — Discussed milestone updates, including revisions to prior milestones.  
- Discussed content for the poster presentation.  
- Planned next meeting.

---

## 4/14/2025 — 12:30 PM

**Attendance:**
- CJ Mitchell  
- Jamal Pearson  
- Jarrett Gilbert  
- Ronnie Burns

**Agenda:**  
Milestone 4 – Slide Preparation

**Minutes:**
- 12:30 PM — Reviewed current milestone updates.  
- 12:45 PM — Discussed the order of presentation slides.

---


## Risk Register

# Risk Assessment Table

| ID   | Risk Description                                         | Category          | Likelihood | Impact | Severity | Phase          | Mitigation Strategy                                                                 |
|------|----------------------------------------------------------|-------------------|------------|--------|----------|----------------|-------------------------------------------------------------------------------------|
| R1   | Inaccurate location data for evacuation routes          | Technical         | Medium     | High   | High     | Initial Planning | Use verified mapping APIs (e.g., Google Maps, Mapbox) and allow user correction     |
| R2   | Chatbot gives outdated or incorrect advice              | Functional        | Low        | High   | Medium   | Development     | Regularly update AI models and integrate with real-time verified sources           |
| R3   | App unavailable during an actual emergency              | Technical         | Medium     | High   | High     | Deployment       | Enable offline storage of plans and downloadable PDFs                              |
| R4   | Users don’t print or save their plans ahead of time     | User Behavior     | High       | Medium | High     | Deployment       | In-app reminders and notifications to prompt saving/printing                       |
| R5   | Privacy concerns with storing user location data        | Legal / Security  | Medium     | High   | High     | Initial Planning | Use encryption, anonymize data, and add clear privacy policy                       |
| R6   | Limited internet access in disaster areas               | Environmental     | High       | High   | High     | Deployment       | Include offline mode and integrate with low-bandwidth fallback systems             |
| R7   | App misunderstood as a substitute for official alerts   | Communication     | Low        | Medium | Medium   | Development     | Include disclaimers and redirect users to FEMA, local alerts, etc.                 |
| R8   | Third-party API dependency failures                     | Technical         | Medium     | Medium | Medium   | Development     | Build fallback logic and monitor API uptime proactively                            |
| R9   | Inadequate testing leading to bugs in critical functions| Quality Assurance | Medium     | High   | High     | Testing         | Conduct thorough unit and integration testing                                      |
| R10  | Insufficient user adoption or interest                  | Business          | Medium     | High   | High     | Post-Launch      | Launch targeted marketing and outreach campaigns                                   |
| R11  | Misinterpretation of AI chatbot responses               | Functional        | Medium     | Medium | Medium   | Development     | Add disclaimers and offer response feedback options                                |
| R12  | Device compatibility issues (older phones/tablets)      | Technical         | Medium     | Medium | Medium   | Testing         | Perform compatibility testing on various devices and OS versions                   |
| R13  | Inaccurate or outdated shelter data                     | Data Integrity    | High       | High   | High     | Maintenance      | Regularly verify and sync with authoritative shelter databases                     |
| R14  | Budget overruns during development                      | Financial         | Medium     | High   | High     | Development     | Track expenses closely and maintain a contingency fund                             |
| R15  | Team burnout due to tight deadlines                     | Team Management   | Medium     | Medium | Medium   | Development     | Set realistic timelines and encourage work-life balance                            |


## Collection-Relationship-Diagram

![Collection Relationship-Diagram](\\)

## Data Dictionary 

# Data Dictionary

## User

| Attribute Name | Key         | Data Type | Description                                |
|----------------|-------------|-----------|--------------------------------------------|
| UserID         | Primary Key | ObjectID  | Unique identifier for the user             |
| Alert          | Foreign Key | object    | Links to associated alert for the user     |
| Customer_Name  |             | ObjectID  | Name of the user                           |
| Location       |             | string    | Location of the user                       |
| Date           |             | string    | Date the user record was created/modified  |

---

## Alert

| Attribute Name | Key         | Data Type | Description                                             |
|----------------|-------------|-----------|---------------------------------------------------------|
| AlertID        | Primary Key | ObjectID  | Unique identifier for the alert                        |
| Disaster       | Foreign Key | object    | References the related disaster                        |
| Location       | Foreign Key | string    | Geographical location of the alert                     |
| Resource       | Foreign Key | object    | References the resource associated with alert          |
| Status         |             | string    | Current status of the alert (active/inactive)          |
| Priority       |             | string    | Priority level (e.g., High, Medium, Low)               |

---

## Disaster

| Attribute Name       | Key         | Data Type | Description                                              |
|----------------------|-------------|-----------|----------------------------------------------------------|
| DisasterID           | Primary Key | ObjectID  | Unique identifier for the disaster                       |
| Location             | Foreign Key | string    | Location where the disaster occurred                     |
| Resource             | Foreign Key | object    | Related resource needed for the disaster                 |
| Disaster_Type        |             | string    | Type of disaster (e.g., flood, earthquake)               |
| Danger_Level         |             | string    | Severity or threat level of the disaster                 |
| Disaster_Info        |             | string    | Description and details about the disaster               |
| Disaster_Time Period |             | string    | Time period when the disaster took place                 |

---

## Resources

| Attribute Name        | Key         | Data Type | Description                                               |
|-----------------------|-------------|-----------|-----------------------------------------------------------|
| ResourceID            | Primary Key | ObjectID  | Unique identifier for the resource                        |
| Resource_Name         |             | string    | Name of the resource                                      |
| Resource_Type         |             | string    | Type of resource (e.g., food, shelter, medical)           |
| Resource_Need         |             | string    | Indicates the need or purpose of the resource             |
| Resource_Importance   |             | string    | Importance level (e.g., Critical, Optional)               |
| Resource_Location     |             | string    | Location where the resource is available                  |

# Lesson Learned Report for MNat.ai

This report is to show what knowledge and skills we gathered through this process. We were able to help each other with many aspects of this project which led to the successful completion of it. Below is the Lessons Learned statement and also a reflection of our improvements over the duration of this project.

---

## Ronnie Burns

I learned a multitude of things during this project from skills to new ideas to new concepts I can now apply to my professional development. Transferring the project manager role between me and my group throughout each milestone gave me valuable experience from every level of a project.

Also learning about different planning techniques such as a style guide, and ways to formulate data like DFDs showed not only how much goes into a project, but also how important things like communication and delegation are when you have lots of moving parts in a project.

Designing the project was fun and it was satisfying bringing it to life. However, more importantly reflecting on the project, I realize that establishing dedicated work periods would have helped me better manage my time better with all my obligations.

I also recognized that strengthening our communication channels through regular check-ins could have enhanced team clarity and overall project flow.

Moving forward, I plan to integrate these strategies to create a more balanced and efficient approach to both my time management and collaborative efforts with any new projects.

---

## Jarrett Gilbert

(No input provided.)

---

## Calvin Mitchell

My takeaway so far from this project is how to delegate tasks to my fellow teammates and further improve upon my leadership skills.

The team has done a great job of completing the tasks I assigned them with little setback. They're very receptive to any kind of comment that is made by me or the professor, which I'm extremely grateful for especially due to the severity of this project.

This project has taught me the ins and outs of creating a start-up, along with other information pertaining to my major, to see out this vision of a future project. With each assignment we continue to hone our craft and better the quality of our work with each milestone.

---

## Jamal Person

This project helped me understand what creating a project for a professional business making a product is like. Everyone must fulfill their role when completing the project because it will not come together if one part is missing.

In the future, ensure that the people working together are coordinated well enough that there will be no setbacks when meeting each other.

The projects are being done according to the instructions and improved to meet the expectations.


##Poster

![CIS EXPO POSTER](https://github.com/cis-famu/semester-project-mnat-ai/blob/main/milestone%203/MNAT%20AI%20Style%20Guide.png)

## MNat.ai Poster presentation

[![Watch the video](https://img.youtube.com/vi/m6dXoNuk4Nk/0.jpg)](https://www.youtube.com/watch?v=m6dXoNuk4Nk)

## References
*None*
