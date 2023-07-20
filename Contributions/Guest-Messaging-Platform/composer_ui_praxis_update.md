# Composer UI: Praxis 8 to 17 Update

## Description

As part of fixing various SCA vulnerabilities in our team's email and push marketing campaign management tool, ie
Composer UI, our team had to do a major praxis scripts update. Since Composer UI
had not seen any updates to its praxis script version since Praxis 8, this update from that version to the latest Praxis 17.2 version
would require a substantial refactor of major logic and components in the application source code. 

## Noteworthy Tasks

- Updating from Praxis 8 to 14 required an update to React 18 which introduced a substantial change to how routing and
rendering worked. After our Lead Engineer and UI expert left, I was the only one in my current team with the most 
recent work experience in the UI. This forced me to rely on only the documentation I could find and the information from
Target's #praxis-community slack channel to carry out this update.
- Another major task while migrating from Praxis 8 to 17 was in updating a large amount (over 50%) of the over 500 unit tests
that were written previously in Composer UI. Starting with React 18, an important React testing library, Enzyme, would 
no longer be supported so this broke several if not all tests that tried to mock axios HTTP calls in Composer's unit tests. 
Since our tests could no longer use Enzyme to mock our axios HTTP calls or assert our react component outputs, we had to rely heavily on 
only Jest to properly test our HTTP calls. 
- Since the main task of this story was remediating SCA vulnerabilities in Composer's dependency libraries, being able 
to use NPM commands to search though those dependencies or the child transitive dependencies was an important task. 
Early on I put together a detailed excel sheet of the SCA vulnerabilities in composer to keep track of which libraries
needed to be updated to fix the underlying security risks. To put together this doc, I made hefty use of Target's
Pi Superset Dashboard. 

## Learnings

- Broadened my understanding of react routing library and the way to properly organize an app around proper component
routing. 
- Cultivate proper unit testing techniques and introduced me to proper mocking patterns for axios HTTP calls. 
- Introduced me to common NPM commands to audit security vulnerabilities, locate transitive dependency vulnerabilities, 
and ways for fixing those discovered security risks. 
- Gain higher familiarity to Target's praxis community and the resources available to fix a myriad of common issues 
updating praxis versions or common used libraries. 

## Screenshots
N/A