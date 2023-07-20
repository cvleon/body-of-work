# Composer UI: Push Content Proof Modal

## Description

Goal of this story was to create a way for business users of the Composer UI tool to send push content proof messages
to their individual phones to see how a push marketing message would look like to a guest. This story was part of the first
major epic I took part when joining the Guest Messaging Platform team. On top of acting as a refresher in frontend development
from my previous TLP rotation, it taught me some important lessons on creating components, testing and working with 
React hooks like `useEffect`. 

## Noteworthy Tasks

- A unique task in this story was creating a component for multi-selecting multiple tags from a drop-down select component. 
By default, the [Material UI](https://mui.com/material-ui/getting-started/overview/) did not have a pre-built component that had this feature so I had to use an existing component, 
the [MuiAutoComplete component](https://mui.com/material-ui/react-autocomplete/) and set some of its basic params so that we could get the behavior we wanted. You can find 
the source code for that component in the PR above. 
- Another key task of this story was being able to manage the state of the DOM to known when the modal was open, closed, when it
was making the HTTP post call to the backend, and how to handle a success or error message if the proof request was successful or not. 
ComposerUI already had a format for properly handling HTTP calls so in the PR above you can see me work around the current system
to implement the behavior I was looking for. 
## Learnings

- Main outcome was able to create a new interactive multi-select component built on top of MUI's AutoComplete component
- Learned how to properly make and test HTTP calls using axios library for the first time
- Able to use a common React hook like `UseEffect` to manage when the modal was open, closed, or sending an HTTP request

## Screenshots
*Due to the internal nature of this project, screenshots and some relevant links were redacted* 
