# TripMind – Requirements

This repository holds the requirements documentation for **TripMind**, a trip planning system.

## About TripMind

TripMind helps travelers plan trips from start to finish. A traveler creates a trip by entering a destination, dates and budget, sets personal preferences, and gets a day-by-day itinerary with recommended attractions. The itinerary can be changed by hand or adjusted automatically when conditions change (for example weather or availability), and the traveler always approves those changes. Business owners keep their attraction data up to date, and administrators moderate content.

**User roles**

- **Traveler / User** – plans and manages trips
- **Business owner** – adds and updates attractions
- **Administrator** – moderates content and oversees the system

## Requirements Engineering Process

The requirements were developed in these steps:

1. **Elicitation** – identifying the stakeholders (travelers, business owners, administrators) and their needs.
2. **Analysis and grouping** – organizing the needs into **Epics**, each covering one functional area or quality attribute.
3. **Specification** – writing each requirement as a **user story** in the form *"As a &lt;role&gt;, I want &lt;goal&gt;, so that &lt;benefit&gt;"*.
4. **Decomposition** – splitting each story into **subtasks** (UI, validation, business rules, persistence).
5. **Management** – tracking epics, stories and subtasks in a Jira backlog. The backlog was exported to CSV and converted into the documents in this repository.

The backlog covers both **functional requirements** (account, trips, itinerary, attractions, recommendations, moderation) and **non-functional requirements** (performance, availability, security, scalability, usability).

## Main Features

| Feature | Summary |
|---------|---------|
| **Trip creation** | Create a new trip with destination, dates and budget; save and edit trips over time. |
| **Itinerary adjustment** | View the itinerary by day and time; add, remove and reorder activities; automatic changes based on external factors, approved or rejected by the traveler. |
| **Attraction management** | Business owners add attractions and update details such as price, availability and opening hours. Administrators moderate the content. |
| **User preferences** | Travelers define trip style and interests so the system can personalize their plans. |
| **Recommendations** | Attractions are matched to the traveler's preferences, ranked and shown as personalized suggestions. |

**Non-functional goals:** itinerary updates within 3 seconds, at least 99.9% availability, encrypted personal data, support for many users at once, and a simple, intuitive interface.

## Documentation

- [User Stories](docs/user-stories.md) – all user stories with their ID and status
