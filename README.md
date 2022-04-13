# REACT BASIC INTRODUCTION


## What is React?
   React is an open-source front-end JavaScript library that is used for building user interfaces, especially for single-page applications.
   
   It is used for handling the view layer for web and mobile apps. It follows a component-based architecture which helps in building reusable UI components. It was created by Jordan Walke, a software engineer working for Facebook. Due to its high demand, it also has a large community support. 


## Features of React
   Features of react are as follows:-
   
   1. It uses reusuable UI components to develop the view of our application.
   2. It has an easy learning curve because it requires the basic knowledge of HTML and Javascript.
   3. It uses Virtual DOM instead of Real DOM, which enhances the performance of our application.
   4. It supports JSX , which helps us to write html code inside javascript.
   5. It follows Unidirectional data flow or data binding.
   6. Using React native we can create mobile - application as well which supports both Android and iOS.
   7. It helps to create single page applications.
   
   

## What is SPA ?
   SPA stands for Single Page Application. It means whenever any event is occured in an application then that application not getting reloading , such type of appliactions is known as Single Page Application. When we create React application using CRA, it always create the application which will be Single page application.
   
   And if that appliaction is getting reloading then that type of application is known as Multipage Application. 
   
   #### For example 
   When we click on the button or select any option in navigation bar then our website is not getting reloading in browser it directly updates the content of our website such type of websites are the example of SPA.
   
   

## What is JSX ?
   JSX stands for JavaScript XML which is simply a syntax extension of JavaScript. It is a type of file used by React which allows developers to directly write HTML like template syntax in React and makes it really easy to understand. Basically it helps to avoid writing the React.createElement() function which is the feature of ECMA Script 5 where as JSX is the feature of ECMA Script 6.



## What is Virtual DOM ?
   DOM stands for Document Object Model. Whenever any HTML, CSS, javascript application gets loaded for the first time on the browser then the browser creates Document object model of that file, and whenever we changes anything in application then the complete DOM is rerendered again and again. 
   
   But in case of react, the DOM is created whenever our react components mounted on the screen for the first time. Now when we makes any changes on the screen like button click because of which the state variable gets updated so in this case the real DOM not directly changed the updates, for this in react we have a concept known as Virtual DOM. In react we use virtual DOM to update the real DOM. 
   
   In react we are having two virtual doms, one virtual dom gets created at the time of mounting of react component so it is a copy of our real DOM, and another virtual DOM contains all the new changes, updated values of state variables. Now both the virtual DOMs get compared with each other and will check for the new changes, this complete procedure is known as Diffing algorithm. Now the new changes will be updated in our Real DOM, this procedure is known as Recoinciliation.



## What is CRA ?
   The create-react-app is a tool/boilerplate that allow us to create quickly our react application and run our application quickly without any config.
   It is a easiest way for creating react application while creating CRA it provides a default setup which includes module bundler(webpack) and babel and other required module also. 



## What is .gitignore ?
   In .gitignore file we can list down all the folders or file which we do not want to push during pushing the changes in github like node_modules.


## Library Vs Framework
   Library is a collection of functions where the code calls the different libraries that means the inversion of control is present in the developer's control i.e the Execution of code will be decided by the developers. In library its developers duty to design the structure. The example of library is React.
   
   On the other hand, framework is a collection of multiple libraries. The inversion of control is not present in the developer's control that means the execution of code is already defined or decided. The example of framework is Angular.
   
   The framework follows the MVC structure(Model View Controller), whereas a library can only be the one for example React is View of MVC. 
   
   

## What is Babel ?
Babel is an inbuild transpiler that converts the ECMA Script 6 code to an ECMA Script 5 code because the browser cannot read JSX which is not a regular JavaScript object. So Babel helps to convert the JSX file to a regular JavaScript object and then pass it to the browser.



## Difference between Class Component and Functional Component
   #### Class Component :- 
   1. A class component requires you to extend from React. Component and create a render function which returns a React element.
   2. Class component can be used when you are doing data operations and server calls.
   3. It is also known as Stateful components because they implement logic and state.
   4. It must have the render() method returning JSX.
   5. It contains lifecycle methods.
   6. Constructor are used as it needs to store state.


   
   #### Function Component :-
   1. A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element.
   2. Functional components can be used mostly when we need to create dumb or stateless components.
   3. It is also known as Stateless components as they simply accept data and display them in some form, that they are mainly responsible for rendering UI.
   4. It does not have state variables, it uses hooks like useState, useParams, etc.
   5. It uses hooks like useEffect in place of react life cycle method.
   6. Complete constructor structure is not required in these components, so they are easy to handle.



## Difference between named export and default export 
   Export without a default tag are named-exports, it use the name of the function or class as their identifier. When we want to import a named component, we can use the same name it was exported with. Names must be imported inside curly brackets. Named exports allow multiple exports in a single file.
   
Whereas, Default exports are created by including a default tag in the export. Usually, we see default exports happen at the bottom of a file, but it's possible to define them when your component is declared. When importing a default export, we don't use curly brackets. When we import a default export, we can give it whatever name we want. A modules can only have one default export.


## Props Vs State
   #### Props :-
   In react all the components are connected to each other like  parent-child relation but if we want to pass data from one component to another then we use props. Props are used to pass data from parent component to child component.
   
   
   #### State :-
   React components has a built-in state object. The state object is where you store property values that belongs to the component. When the state object changes, the component re-renders.



## Phases & Methods of Life cycle of a component
