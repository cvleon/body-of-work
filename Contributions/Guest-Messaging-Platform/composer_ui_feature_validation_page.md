# Composer UI: Feature Validation Page

## Description

As part of a goal last year to A/B test our team's personalize content messaging system, 
Morpheus introduced an epic to create a new A/B test UI landing page called simply Feature Validation.
The new UI would be added into our existing email and push marketing management tool, 
called Composer UI, as a new sub-page. This new landing page would interact with a new set of
REST-ful endpoints to browse existing Feature Validation A/B tests and create, edit, update, and delete
new tests. 

This was the first major UI epic that I undertook at Morpheus.

## Noteworthy Tasks

- Used [Material UI](https://mui.com/material-ui/getting-started/overview/) component library to create new Feature Validation landing page and A/B Test 
form. This was my first use of the MUI React library and it changed the way I think about
and create new UI components. Similar to Target's Canvas UI, MUI allowed me to easily create 
gorgeous and interactive forms. You can find screenshots of the final form below. 
- One of the key challenges of completing this task was making use of the built-in data store that kept 
track of the current state of components. I have never personally used the React Redux store before but this built in 
data store was a manual implementation of that feature. Our team's Composer UI used a custom built 
data store solution to disbatch actions and subscribe to data state updates. In the beginning, I found working
with the data store limiting because I could not use one of favorite react libraries, but after working with it for a bit,
I came to appreciate the simplicity and flexibility that it provided. 
- Another challenge was properly using complex javascript syntax to easily combine objects to create 
simple and easily updatable payloads that are sent downstream via HTTP calls. It was in this project that I was first
introduced to javascript `spread(...)` syntax for objects which changed the way I built and update javascript objects in react. 

## Learnings

- Creating beautiful react components with React Material UI
- Effectively utilize Composer UI's built-in data store to disbatch actions and subscribe to data state updates
- Introduced me to new javascript syntax rules like the spread method for creating and updating JS objects
- Pressured me to make use of new react libraries and tools instead of ones that I had previously been 
exposed to. For example, using MUI and data store instead of Canvas UI and react-hook-form
- Make efficient use of useEffect and dispatch actions from child component pages to send payloads to downstream APIs

## Screenshots
*Due to the internal nature of this project, screenshots and some relevant links were redacted* 