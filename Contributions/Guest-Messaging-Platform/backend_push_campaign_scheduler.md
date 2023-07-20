# Push Campaign Scheduler

## Description
The following contribution is broken up between two different stories that were completed at different
times, but supported the same general process. 

The first is the creation of a push campaign scheduler that calls an API endpoint in the backend to create a default 
push marketing campaign. The second is a new landing page in Composer UI to edit 
the template that is used to create the above default push campaign. Some additional requirements are that the push 
campaign scheduler must be configured to automatically run every day at a specific data/time following standard cron syntax
and that it must only create a default push campaign if no push campaign has already been created manually by the 
business team for that date. 
In addition, the landing page must enforce certain business rules as required by what is a valid default push campaign. 
The scheduler was built using Kotlin and Spring Framework and the new landing page in Composer UI was built using the 
standard JS, React and MUI tech stack. 


## Noteworthy Tasks

- Creating a new Github repo in my team's org and adding the necessary gradle and vela requirements. This was a 
first for this team and taught me a lot about the CI/CD pipeline used by the team. 
- Setting up a proper spring framework service that interacts with my team's RESTful composer-service API and runs everyday
at a specific date/time as configured by cron syntax.
- Making use of a Kotlin shuttleIO client to send an alert to slack if the scheduler is not able to create a default push 
campaign for that date. This was technically already created by a lead engineer, but it required copying major components
from a different repo and making the necessary adjustments to make it work for this application.
- For creating the UI landing page, a notable task was making sure the edit template page was user-friendly, provided helpful
and clear feedback when saving/editing the template, and create easy access to users via the main side navigation. Screenshots below 

## Learnings

- Constructed a configurable kotlin spring framework service that runs automatically at a given date/time
- Grew in my knowledge of ShuttleIO and how to use it to set up proper slack alerts for Restful APIs
- Strengthened my understanding of my team's CI/CD pipeline by creating a new gradle repo in team org
- Enforce my understanding of MUI components and responsive web design by creating a new Composer UI landing page

## Screenshots
*Due to the internal nature of this project, screenshots and some relevant links were redacted* 

