# Milestone 2

**Table of Contents**
1. Task & Schedule Management
    - [Work Breakdown Structure](#work-breadown-structure)
    - [Gantt Chart  & Network Diagram](#gantt-chart--network-diagram)
1. [Requirements](#requirements)
1. [Use Cases](#use-cases)
1. [Use Case Diagram](#use-case-diagram)
1. [Research on other systems](#research-on-other-systems)
1. [API Descriptions](#api-descriptions)

## Work Breakdown Structure

| Task ID | Task Name | Duration (hours) | Start Date | Finish Date | Predecessors |
|---------|-----------|-----------------|------------|-------------|--------------|
| 1       | Project Management (PM) | 744 | 2/25/2025 | 4/1/2025 | - |
| 1.1     | Project Initiation and Planning | 240 | 2/25/2025 | 3/10/2025 | 1 |
| 1.2     | Risk Management | 192 | 3/10/2025 | 3/19/2025 | 1.1 |
| 1.3     | Stakeholder Communication | 192 | 3/20/2025 | 3/31/2025 | 1.2 |
| 1.4     | Project Tracking and Reporting | 120 | 4/1/2025 | 4/1/2025 | 1.3 |
| 2       | Requirement Analysis and Planning | 624 | 4/1/2025 | 5/6/2025 | 1.4 |
| 2.1     | Gather Requirements | 216 | 4/1/2025 | 4/11/2025 | 2 |
| 2.2     | Define System Functionalities | 192 | 4/14/2025 | 4/23/2025 | 2.1 |
| 2.3     | Document Data Storage Needs | 216 | 4/24/2025 | 5/6/2025 | 2.2 |
| 3       | System Design and Architecture | 816 | 5/14/2025 | 6/23/2025 | 2.3 |
| 3.1     | Database Design and Development | 264 | 5/14/2025 | 5/28/2025 | 3 |
| 3.2     | UI/UX Design and Testing | 288 | 5/22/2025 | 6/6/2025 | 3.1 |
| 3.3     | Secure Data Integration | 264 | 6/9/2025 | 6/23/2025 | 3.2 |
| 4       | Development and Implementation | 888 | 6/30/2025 | 8/11/2025 | 3.3 |
| 4.1     | Code Development and Prototyping | 384 | 6/30/2025 | 7/21/2025 | 4 |
| 4.2     | Testing and Feedback | 288 | 7/14/2025 | 7/29/2025 | 4.1 |
| 4.3     | Final Integration | 216 | 7/30/2025 | 8/11/2025 | 4.2 |

## Gantt Chart & Network Diagram
![gantt chart](https://github.com/CJdaRacc/MNat.ai/blob/main/Milestone%202/gnattchrt.png)

[Downloadable Project Management File](https://github.com/CJdaRacc/MNat.ai/blob/main/Milestone%202/Tasks-MNat.ai%20-%20Group%205%20-%203%20Mar%202025%20(2.36%20PM)(1).xlsx)

## Requirements

### Product Requirements Document

**Project Information**

**Details or description of the product that will improve the customer experience.**

The application provides individuals in high-risk natural disaster areas with personalized emergency escape plans and real-time resources to enhance their safety and preparedness. It offers customized evacuation routes, supply checklists, and local shelter information, along with a chatbot for real-time disaster-related assistance.

**Objectives/Goals**

**Define the product in an easy-to-understand, actionable, achievable, and measurable way.**

*   Provide real-time emergency preparedness assistance.
*   Enable personalized evacuation planning.
*   Enhance user safety with AI-driven recommendations.
*   Facilitate access to shelter and emergency services.
*   Deliver multilingual chatbot support for disaster-related queries.

**Assumptions & Constraints**

**Note what you expect to have but aren’t certain of (such as internet) and what implementation can’t require.**

*   The application assumes consistent access to GPS and internet connectivity but provides offline features where feasible.
*   Government and relief agency databases must be accessible for real-time shelter updates.
*   Security measures must comply with GDPR and CCPA regulations.

**Background & Strategic Fit**

**What is the problem you’re solving or niche you’re filling, and how does your organization have the capabilities to exploit this?**

With natural disasters becoming more frequent and severe, there is a critical need for a personalized emergency preparedness tool. This application leverages GIS mapping, AI-driven insights, and real-time weather data to enhance emergency readiness. The growing focus on disaster resilience creates market opportunities through premium subscriptions, affiliate partnerships, and collaborations with emergency retailers.

**Scope: User Stories & Requirements**

**Define features and functions of the product, including a general explanation of those requirements from a user’s perspective.**

*   As a user, I want to create an emergency profile with location and medical needs.
*   As a user, I want to receive real-time disaster alerts relevant to my area.
*   As a user, I want to generate evacuation routes that adapt dynamically.
*   As a user, I want access to a chatbot for immediate disaster-related queries.
*   As an emergency service provider, I want to update shelter capacities in real-time.

**Product Features**

**List all the product features, including a description, goal, and use case.**

*   **User Registration & Authentication:**
    *   **Description:** Secure login and profile management system to protect user data and personalize application experience.
    *   **Goal:** To ensure secure access to the application and personalize the user experience based on individual profiles.
    *   **Use Case:** A new user registers with their email and password, then completes their emergency profile with address and medical information.

*   **Personalized Emergency Planning:**
    *   **Description:** Generates customized evacuation routes and digital emergency plans based on user profiles and real-time disaster data.
    *   **Goal:** To provide users with tailored escape strategies, increasing their chances of safe evacuation during emergencies.
    *   **Use Case:** During a hurricane warning, a user receives a dynamically updated evacuation route based on their home location, traffic conditions, and open routes.

*   **Real-Time Disaster Alerts:**
    *   **Description:** Integrates with weather APIs and emergency broadcast systems to deliver timely and location-specific warnings about impending disasters.
    *   **Goal:** To provide early warnings enabling users to take proactive safety measures and prepare for evacuation.
    *   **Use Case:** A user receives a push notification on their smartphone about an approaching wildfire in their vicinity with safety guidelines.

*   **GIS Mapping & Navigation:**
    *   **Description:** Utilizes GIS technology to display dynamic evacuation routes, shelter locations, and real-time hazard zones on interactive maps, with offline access for use during connectivity disruptions.
    *   **Goal:** To offer reliable navigation and situational awareness even when internet access is limited during a disaster.
    *   **Use Case:** During a power outage and internet disruption caused by a flood, a user can still access pre-downloaded maps and evacuation routes to navigate to a safe zone.

*   **Supply Checklist & Recommendations:**
    *   **Description:** AI-driven recommendations for essential emergency kit supplies based on household size, location, and disaster type, with a digital checklist for preparation.
    *   **Goal:** To ensure users are well-prepared with necessary supplies, reducing risks associated with inadequate resources during emergencies.
    *   **Use Case:** Based on a user's family profile and location in a hurricane-prone area, the app suggests a customized emergency kit list including water, non-perishable food, batteries, and medications.

*   **Shelter Locator:**
    *   **Description:** Provides real-time updates on the location, capacity, and accessibility of nearby emergency shelters and medical services, sourced from government and relief agency databases.
    *   **Goal:** To quickly direct users to available safe shelters and medical assistance, especially when evacuation is necessary.
    *   **Use Case:** A user displaced by an earthquake uses the app to locate the nearest open shelter with available capacity and accessibility for individuals with disabilities.

*   **Chatbot Assistance:**
    *   **Description:** AI-powered multilingual chatbot to answer user queries related to disaster preparedness, safety procedures, evacuation routes, and available resources in real-time.
    *   **Goal:** To offer immediate support and information access, enhancing user understanding and reducing panic during emergencies.
    *   **Use Case:** A user asks the chatbot, "Where is the nearest flood shelter in my area?" and receives instant information and directions.

*   **Community Support:**
    *   **Description:** Platform for peer-to-peer information sharing, verified community reports on local conditions, and a forum for users to exchange experiences and preparedness tips.
    *   **Goal:** To foster a community of prepared individuals and provide crowdsourced real-time information on the ground, supplementing official alerts.
    *   **Use Case:** Users in a neighborhood affected by a storm share updates on road closures and local resource availability, helping others in the community navigate the situation.

**Release Criteria**

**Covers functionality, usability, reliability, performance, and supportability.**

*   The application must function on iOS and Android.
*   Minimum 99.99% uptime availability.
*   Scalable infrastructure supporting 1 million concurrent users.
*   Secure encryption for user data.
*   Offline access to critical features.

**Success Metrics**

**Define quantifiable measurements to track the product and see if it’s meeting objectives.**

*   80% of users complete emergency profile setup.
*   95% accuracy in AI-driven evacuation route suggestions.
*   Less than 5-second latency for real-time alerts.
*   1 million active users within the first year.
*   High user engagement and retention rates in premium subscriptions.

## Use Cases

### Full Dressed-Use Cases

**Case 1: Weather Alarm and Evacuation Notice**

**Primary Actor:** Administrators

**Stakeholders:**

*   Public users: People who want to know the danger and how to avoid it.
*   Local governments: To see which areas will be affected and issues emergency response for civilians.

**Preconditions:**

*   The AI system has access to real-time weather data from sensors and satellites.
*   The user has an active mobile app, social media, or communication tool to receive alerts.
*   Local authorities are prepared to issue evacuation orders if necessary.

**Main Flow:**

1.  The AI receives weather data from weather satellites, sensors, and meteorological systems.
2.  The AI processes this data to detect the impending weather disaster.
3.  The AI assesses the level of risk for the user's location based on real-time data.
4.  The AI sends weather alerts to users via emergency broadcast systems.
5.  The alert includes information about the disaster and what actions to take.
6.  If the risk level is high, the AI suggests evacuation routes based on real-time traffic conditions, the user's location, and the weather event's predicted path.
7.  The AI integrates with local authorities’ systems to ensure that evacuation centers are prepared and that roads are clear.
8.  The user receives the alert on their phone, informing them of the imminent weather disaster and providing evacuation instructions.
9.  Local government authorities issue official evacuation orders and guide users toward safe zones or shelters.
10. Emergency responders are alerted by the AI, and they use the AI system for situational awareness and to coordinate rescue or evacuation activities.
11. The user follows the evacuation instructions provided by the AI system and heads to the recommended shelter or safe zone.

**Postconditions:**

*   The user is safely on an evacuation route or within a shelter.
*   Local authorities and emergency responders have coordinated the evacuation effort with the AI system's guidance.


**Case 2: Resource Management and Distribution During a Weather Disaster**

**Primary Actor:** Administrators

**Stakeholders:**

*   Public users: People who need to know what supplies are needed to survive the weather disaster.
*   Supply/Resource Providers: To see what resources are needed to send to which area that needs it the most.
*   Local governments: Authorities responsible for managing resources, shelters, and aid distribution.

**Preconditions:**

*   The AI system is linked to a resource database that includes food, water, first aid supplies, and medical equipment.
*   Emergency responders are aware of the disaster's scope and have access to the AI system for coordination.
*   The local government has identified available shelters and is ready to manage resources.

**Main Flow:**

1.  A weather disaster (e.g., hurricane, flood, blizzard) strikes, and the AI system receives real-time data about the affected areas.
2.  The AI integrates with the resource database, which includes information about available resources like food, water, medical supplies, and shelters.
3.  AI analyzes data from user reports, sensors, and emergency responders to identify areas in critical need of resources.
4.  It determines the most efficient way to distribute resources, considering the severity of the disaster and the urgency of needs.
5.  The AI guides them to the most affected zones using real-time traffic data and weather conditions.
6.  Affected users may request assistance through the AI system (e.g., for food, medical supplies, or shelter).

**Postconditions:**

*   Critical resources (food, water, medical supplies) are delivered to users in need.
*   The AI has ensured the efficient allocation and distribution of resources during the disaster.
*   Emergency responders and users can continue the recovery process after immediate needs have been met.

## Use Cases Diagram

![Use Cases Diagram](https://github.com/CJdaRacc/MNat.ai/blob/main/Milestone%202/DFDChrt.png)

### Research on Other Systems

Several systems and methodologies share functionalities similar to MNat.AI, particularly in enterprise architecture, design capture rationale, and systems engineering. An overview of notable examples is provided below.

**Capella**

Capella is an open-source solution for model-based systems engineering (MSBE). Developed by Thales and later released as an Eclipse open-source project. Capella provides a process and tooling for graphical modeling of systems, hardware, or software architectures, aligning with the Arcadia method (A system and software architecture engineering model based on architecture-centric method and model-driven engineering activities). Primarily used for modeling complex and safety-critical systems in industries such as aerospace, transportation, and communications. Capella offers an intuitive interface, guiding engineers in their activities and allowing them to focus on defining architectures rather than learning complex modeling languages.

*   **Key Features/Purpose:**
    *   Provides a process and tooling for graphical modeling of systems, hardware, or software architectures.
    *   Aligns with the Arcadia method.
    *   Offers an intuitive interface, guiding engineers.
    *   Focuses on defining architectures rather than learning complex modeling languages.
*   **Applications:**
    *   Primarily used for modeling complex and safety-critical systems.
    *   Industries: aerospace, transportation, and communications.

**Enterprise Systems Engineering (ESE)**

Enterprise Systems Engineering (ESE) involves applying systems engineering principles to the enterprise as a whole, integrating both business and technology needs. It encompasses processes such as technology planning, capabilities-based engineering analysis, enterprise architecture, and enterprise analysis and assessment. ESE aims to improve decision-making, increase efficiency, and ensure that technological implementations align with organizational goals.

*   **Key Features/Purpose:**
    *   Applies systems engineering principles to the enterprise as a whole.
    *   Integrates both business and technology needs.
    *   Encompasses processes: technology planning, capabilities-based engineering analysis, enterprise architecture, and enterprise analysis and assessment.
    *   Aims to improve decision-making.
    *   Aims to increase efficiency.
    *   Aims to ensure technological implementations align with organizational goals.

**IDEF6**

IDEF6, or Integrated Definition for Design Rationale Capture, is a method aimed at facilitating the acquisition, representation, and manipulation of the design rationale used in developing enterprise systems. It focuses on capturing the reasons, justifications, and underlying motivations that drive the decision-making process during design. By explicitly documenting design rationale, IDEF6 helps avoid repeating past mistakes, provides a means for determining the impact of proposed design changes, forces the explicit statement of goals and assumptions, and aids in communicating final system specifications.

*   **Key Features/Purpose:**
    *   A method aimed at facilitating the acquisition, representation, and manipulation of design rationale.
    *   Focuses on capturing reasons, justifications, and motivations driving design decisions.
    *   Helps avoid repeating past mistakes.
    *   Provides means to determine impact of design changes.
    *   Forces explicit statement of goals and assumptions.
    *   Aids in communicating final system specifications.

## API Descriptions

### API Integrations for Disaster Response System

This section outlines the APIs to be integrated into the disaster response system, categorized by their purpose and key endpoints, using short bullet points.

**1. Google Maps API**
*   **Purpose:** Mapping, geolocation, routing for escape routes, shelters, resources.
*   **Endpoints:**
    *   Geocoding API: Address to coordinates.
    *   Directions API: Route calculations, real-time traffic.
    *   Places API: Essential services (hospitals, gas stations, shelters).
    *   Distance Matrix API: Travel time/distance calculation.
    *   Maps JavaScript API: Embed interactive maps.
    *   Roads API: Accurate path tracing.

**2. FEMA API (Federal Emergency Management Agency)**
*   **Purpose:** Disaster info, alerts, shelters, federal assistance.
*   **Endpoints:**
    *   Disaster Declarations Summary: Disaster details.
    *   Shelter Locator API: Shelter locations & availability.
    *   Weather Alerts API: FEMA disaster alerts.
    *   Financial Assistance API: Aid eligibility & status.

**3. NOAA API (National Oceanic and Atmospheric Administration)**
*   **Purpose:** Weather forecasts, storm tracking, disaster alerts.
*   **Endpoints:**
    *   Weather Alerts API: Warnings for hurricanes, tornadoes, floods.
    *   Forecast API: Hourly/daily weather forecasts.
    *   Storm Reports API: Storm tracking, wind speed, precipitation.
    *   Tsunami Alerts API: Tsunami warnings & safety zones.

**4. OpenWeather API**
*   **Purpose:** Real-time & forecasted weather conditions.
*   **Endpoints:**
    *   Current Weather Data: Live weather info.
    *   Weather Alerts: Location-based warnings.
    *   Historical Weather API: Past weather trends.
    *   Air Pollution API: Air quality reports.

**5. ArcGIS API (Esri Disaster Response Services)**
*   **Purpose:** GIS data & layers for disaster zones.
*   **Endpoints:**
    *   Disaster Response API: Maps, satellite imagery of affected areas.
    *   Shelter and Resource Finder: Evacuation shelters & relief centers.
    *   Road Conditions API: Blocked/damaged roads.

**6. Red Cross API**
*   **Purpose:** Disaster relief info, emergency contacts, first-aid.
*   **Endpoints:**
    *   Shelter Finder API: Red Cross shelter locations.
    *   Emergency Contacts API: Local emergency services.
    *   First Aid API: Medical emergency instructions.

**7. Firebase API (Google Cloud Messaging & Database Storage)**
*   **Purpose:** Real-time data sync, cloud storage, push notifications.
*   **Endpoints:**
    *   Firestore Database: User emergency plans storage.
    *   Cloud Messaging API: Push notifications for alerts/updates.
    *   Authentication API: Secure user login & profiles.

**8. GPT-4 API (AI Chatbot for Emergency Assistance)**
*   **Purpose:** AI chatbot for disaster preparedness questions.
*   **Endpoints:**
    *   Chat Completion API: AI chatbot interaction.
    *   Knowledge Base API: Disaster FAQs integration.

**9. SafeGraph API (Business & POI Data)**
*   **Purpose:** Locate open businesses during disasters.
*   **Endpoints:**
    *   Places API: Business locations & status.
    *   Mobility API: Human movement data for response.

**10. USPS Address API (United States Postal Service)**
*   **Purpose:** Verify user addresses.
*   **Endpoints:**
    *   Address Validation API: Address accuracy.
    *   ZIP Code Lookup API: Address to postal codes.

**11. Waze API (Crowdsourced Traffic & Road Hazard Data)**
*   **Purpose:** Real-time road conditions, hazards, accidents.
*   **Endpoints:**
    *   Traffic Alerts API: Congestion & blocked roads.
    *   Incident API: Road closures & accidents.

**12. SendGrid API (Email Notifications & Alerts)**
*   **Purpose:** Emergency preparedness emails & warnings.
*   **Endpoints:**
    *   Transactional Email API: Customized emergency emails.
    *   Marketing API: New safety feature notifications.

**13. Crowdsource Data API (Custom API for User-Submitted Reports)**
*   **Purpose:** User reports of disasters, road blocks, missing persons.
*   **Endpoints:**
    *   Incident Reporting API: Submit disaster reports.
    *   Verification API: Report verification.
