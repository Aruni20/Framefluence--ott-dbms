# Framefluence: OTT Platform DBMS
**A Comprehensive Database Management System for Next-Generation Digital Streaming**

---

##  Project Overview
**Framefluence** is a high-performance, scalable, and mission-critical Database Management System designed to handle the complex ecosystem of an Over-the-Top (OTT) streaming platform. Engineered to mirror functionalities of industry giants like Netflix, Framefluence manages everything from high-concurrency user subscriptions to cross-border content licensing, granular viewing analytics, and multi-tenant billing.

---

## Architectural Highlights

### 1. Conceptual Modeling (ER Diagram)
The system is built upon a robust Entity-Relationship model that captures the intricate connections between:
*   **Users & Profiles**: Managing multi-device access and personalized viewing preferences.
*   **Hierarchical Content**: A specialized structure differentiating between standalone **Movies** and multi-season **Series** with shared metadata.
*   **Financial Ecosystem**: Linking Subscriptions, dynamically calculated Renewal Dates, and secure Payment transaction logs.
*   **Talent Database**: A sophisticated Artist mapping that categorizes talent into **Actors** and **Non-Actors** (Directors, Crew) across specific content credits.

### 2. Physical Design & Normalization
Framefluence is mathematically verified for data integrity. The project includes **Normalization Proofs** demonstrating that every one of the 20+ tables adheres to **Boyce-Codd Normal Form (BCNF)**.
*   **Redundancy Elimination**: Zero data duplication across relations.
*   **Anomaly Prevention**: Structured to prevent Insertion, Update, and Deletion anomalies.
*   **Integrity Enforcement**: Strict enforcement of Primary/Foreign Key constraints ensures a consistent state across the global schema.

---

## Schema Implementation (DDL)
The schema is implemented using highly optimized SQL scripts, categorized into three distinct layers:
*   **Core Entities**: `users`, `contents`, `subscriptions`, `payment`.
*   **Content Metadata**: `episodes`, `series`, `movies`, `content_genre`, `content_language`.
*   **Interaction Junctions**: `watch_history`, `ratings`, `user_device`, `playlist_content`.

---

## The Analytics Engine (Complex Queries)
Framefluence provides actionable insights through specialized query suites designed for different stakeholders:

###  User-Oriented Analytics
*   **Smart Recommendations**: SQL logic that suggests content based on >=4 star ratings while excluding already-watched titles.
*   **Personalized Metrics**: Tracking time spent on "Movies vs Series" to optimize user UI experience.

###  Administrator Control Suite
*   **Churn Management**: Predictive identification of subscriptions expiring within 7 days.
*   **Revenue Auditing**: Monthly extraction of revenue data aggregated by region and subscription tier.
*   **System Health**: Monitoring device-usage density per active user account.

###  Advertiser & Marketing Intelligence
*   **Viewer Diversity**: Content-level analysis of audience nationalities for targeted ad placement.
*   **Hidden Gems Identification**: A complex filter isolating high-rated content (Rating > 3.5) with low view counts (< 5000) for promotional boosting.
*   **Re-engagement Tracking**: Identifying content with the highest re-watch frequencies.

---

##  Sample Dataset
The project includes a comprehensive seeding script that populates the database with:
*   **Diverse User Base**: Global demographic data spanning USA, India, UK, Egypt, and more.
*   **Polymorphic Content**: A mix of genres (Sci-Fi, Action, Thriller) and languages (Spanish, Hindi, English).
*   **Transaction Logs**: Realistic subscription histories and rating patterns.

---

## Future Scope
Framefluence is designed with extensibility in mind. Future versions could incorporate:
*   **AI-Driven Hyper-Personalization**: Integrating machine learning models directly into the SQL layer to provide real-time, behavior-based content recommendations.
*   **Interactive Content Support**: Schema expansion to handle multi-branching storylines and user-driven choices (interactive episodes).
*   **Cloud CDN Integration**: Implementing geolocation-aware content delivery tracking to optimize video buffering based on server-to-user proximity.
*   **Ad-Tech Optimization**: Developing more granular advertiser tables to support dynamic ad-insertion based on real-time viewer trends.
*   **Social Connectivity**: Adding "Watch Together" features, social profiles, and collaborative playlists for a community-driven experience.

---

##  Contributors (Team 12)

| Name | Student ID |
| :--- | :--- |
| **Aruni Saxena** | 202418006 |
| **Paarth Patel** | 202418045 |
| **Rishi Barapatre** | 202418008 |
| **Chudasama Yashrajsinh** | 202418012 |

---
*Developed as a Harm Monitoring Ecosystem for Digital Safety.*
