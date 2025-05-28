# Digital Kudos Wall

A web application that lets colleagues publicly recognize each other's great work, fostering a culture of appreciation and visibility within teams.

## 1. Project Members

**Project Member(s):** Individual Subscription - Working individually on this project to demonstrate XP, CD, and lean product development practices.

## 2. Version Control

**Version Control System:** Git  
**Hosting Platform:** GitHub

## 3. System Name

**Digital Kudos Wall** - A recognition platform for team achievements and contributions.

## 4. System Repository

This is the main system repository for the Digital Kudos Wall project.

**Contributors:**

- Individual developer following XP and CD principles
- Inspired by the work of Kent Beck, Martin Fowler, Dave Farley, Robert C. Martin, Marty Cagan, Dan North, and other lean/agile thought leaders

## 5. System Use Cases

### Primary Use Cases:

- **Give Kudos** - Tech Leads can create and submit kudos for team members
- **View Kudos Wall** - All users can view publicly displayed kudos
- **User Authentication** - Users can register and login to access the platform
- **Analytics Dashboard** - Users can view recognition trends and insights

### Primary Actors:

- **Tech Lead** - Can create kudos and view the wall
- **Team Member** - Can view kudos wall and analytics

### User Story Map Reference:

See [USER_STORY_MAP.md](./USER_STORY_MAP.md) and [user-story-map.pdf](./docs/user-story-map.pdf) for detailed user journeys and MVP scope.

## 6. External Systems

**External I/O Systems:**

- Public REST APIs for potential integrations
- Email system for notifications (future consideration)

**External Non-deterministic Systems:**

- System Clock for timestamps
- User authentication services

## 7. System Architecture Style

**Architecture:** Frontend + Microservice Backend

The system follows a clean, simple architecture suitable for the MVP scope while allowing for future scalability.

## 8. Architecture Diagram

The system consists of:

**Components:**

- Frontend (Web Application)
- Backend (API Server)
- Database (Data Storage)

**Relationships:**

- Frontend communicates with Backend via REST API
- Backend manages data persistence through Database
- All components support the core user journeys defined in the User Story Map

_Architecture diagram to be added_

## 9. Tech Stack

**Programming Languages:**

- TypeScript/JavaScript
- HTML/CSS

**Frontend Framework:**

- React.js with modern tooling

**Backend Framework:**

- Node.js with Express.js

**Database:**

- PostgreSQL (for production)
- SQLite (for development/testing)

**Additional Tools:**

- Jest for testing
- ESLint for code quality
- Prettier for code formatting

## 10. Repository Strategy

**Multi-Repository Approach** - Separate repositories for different concerns:

- **digital-kudos-wall** (this repo) - Main project documentation and workspace configuration
- **digital-kudos-wall-frontend** - React frontend application
- **digital-kudos-wall-backend** - Node.js backend API
- **digital-kudos-wall-system-tests** - Acceptance and E2E tests using Dave Farley's Four-Layer Model

## 11. Branching Strategy

**Feature Branching** - Trunk Based Development

## 12. Deployment Model

**Local Development** - Initial focus on local development environment:

- Docker containers for consistent development environment
- Local database setup
- Hot reloading for rapid feedback cycles
- Future consideration for cloud deployment (AWS)

## 13. Component Repositories

**Links to Component Repositories:**

- [Frontend Repository](https://github.com/chirag1507/digital-kudos-wall-frontend) - React web application
- [Backend Repository](https://github.com/chirag1507/digital-kudos-wall-backend) - Node.js API server
- [System Tests Repository](https://github.com/chirag1507/digital-kudos-wall-system-tests) - Smoke, Acceptance and E2E tests

## 14. Project Management

**Project Board:** GitHub Projects for ticket management and user story tracking

**Approach:** Single project board for the entire system with:

- User Stories from the story map
- Bug tracking
- Task lists for frontend and backend work
- Multiple assignees per ticket when needed

## 15. Development Approach

This project follows:

- **Extreme Programming (XP)** practices
- **Continuous Delivery (CD)** principles
- **Lean Product Development** methodology
- **User Story Mapping** for feature prioritization
- **Test-Driven Development** where appropriate
- **Small batch sizes** and frequent integration

### MVP Focus

The current MVP includes:

- User registration and authentication
- Kudos creation (Tech Leads only)
- Basic kudos wall display
- Simple, clean user interface

Future iterations will add filtering, search, analytics, and enhanced user experience features.

## Getting Started

1. Clone this repository and the component repositories
2. Open the `digital-kudos-wall.code-workspace` file in your IDE for multi-repo development
3. Follow setup instructions in individual component repositories
4. Refer to the User Story Map for understanding user journeys and priorities

## Documentation

- [User Story Map](./USER_STORY_MAP.md) - Detailed user journeys and MVP definition
- [Visual Story Map](./docs/user-story-map.pdf) - Visual representation of the story mapping session

---

_This project demonstrates modern software development practices including lean product development, continuous delivery, and user-centered design._
