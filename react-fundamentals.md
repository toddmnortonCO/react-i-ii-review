### Remember

Answer these on your own, then compare answers as a group

1.  What is React?
    a JS library for building UIs, created by Facebook

2.  What is create-react-app?
    boilerplate tools and framework to start a React project, sets up development environment

3.  What is Component Based Architecture?
    the idea of splitting up various pieces of a React app into separate components

4.  What is JSX?
    syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like, allows you to write HTML in React, stands for Javascript XML

5.  What is the virtual DOM?
    The virtual DOM (VDOM) is a programming concept where an ideal, or “virtual”, representation of a UI is kept in memory and synced with the “real” DOM by a library such as ReactDOM. This process is called reconciliation.

6.  What is unidirectional (one-way) data flow?
    the flow of data that follows the structure down, way to get around this is to pass data up through events, parent > child, use props for this

### Understand

Discuss these questions in pairs if you have a 4-person group

7.  Summarize what happens when you run `create-react-app my-app`
      the best way to start building a new single-page application in React.  It sets up your development environment so that you can use the latest JavaScript features, provides a nice developer experience, and optimizes your app for production.

8.  Explain what this code does:
    checking to see if the title of the mentor is lead mentor or not, if it is then it displays Tim Biles w/ additinal information

```jsx
import React from "react";

const Mentor = props => (
  <div className="mentor-container">
    <h1 className={props.title === "Lead Mentor" ? "lead" : ""}>Tim Biles</h1>
    <ul>
      <li>Fort Worth, TX</li>
      <li>My email address is timbilestimbiles@gmail.com</li>
    </ul>
  </div>
);

export default Mentor;
```

9.  Explain how data is passed from a parent component to a child component.
    data is passed down via props (from parent component) along with the use of 'import' and 'export' components,

### Apply

Try these on your own, but work together if you start to get stuck.

10.  Use `create-react-app` to create a new React application called `student-directory`

11.  Use the code from `Mentor` above to create a new functional, stateless component called `User` with a list of friends. Hard code the list of friends, do not use state or props.

### Analyze, Evaluate, Create

Discuss these questions as a group

12. What are the benefits and drawbacks of using a tool like create-react-app?

13. Compare and contrast JSX with other templating options, such as those used in Angular or Vue

14. Compare and contrast one-way data flow with two-way data binding.
