---
layout: post
title:      "What is this thing called dispatch?"
date:       2021-05-19 04:21:04 +0000
permalink:  what_is_this_thing_called_dispatch
---


The idea of a global state that is accessible to any component in an application is a powerful concept that Redux solves. It does this using a built in function called `dispatch` to communicate information from a component to the global state, or Redux store. `dispatch` is simply a function provided by the redux store that is responsible for carrying a payload of information to be stored in the Redux store. It is a plain JavaScript object that must include a "type" of action.

To give an application's component the ability to use the dispatch function, it must be connected to the Redux store with the `connect()` method. The connect method takes two arguments, the first, mapStateToProps, gives the component the desired information <em>from</em> the store, while the second argument, mapDispatchToProps, connects a component's function to the store, allowing it to send information <em>to</em> the store.

When a component is using the `connect()` method it is received as the `dispatch` function in props: `props.dispatch`.
Let's say I have an application for tracking recipes and all my recipe information is collected a form component and stored as an object called `recipe`. My new recipe form recipe would need to `import {connect} from 'react-redux'` to be connected to the Redux store and be able to call `props.dispatch`. I could then have a function to send the information in `recipe` to the store called `addRecipe`. I would connect that function to the redux store using `connect()` method's second argument, mapDispatchToProps. As I mentioned before, `dispatch` requires an action type, in this case, `type: ADD_RECIPE` makes the most sense. With this set up, I will be able to use the `dispatch` function to send the information in `recipe` to the store to be used by other components in the application that are also connected to the store.
