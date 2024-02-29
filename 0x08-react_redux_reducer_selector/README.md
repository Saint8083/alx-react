# 0x08. React Redux reducer+selector

## Selectors
Explanations of how and why to use selector functions to read values from state

- Idiomatic Redux: Using Reselect Selectors for Encapsulation and Performance
https://blog.isquaredsoftware.com/2017/12/idiomatic-redux-using-reselect-selectors/
A complete guide to why you should use selector functions with Redux, how to use the Reselect library to write optimized selectors, and advanced tips for improving performance.

- ReactCasts #8: Selectors in Redux
https://www.youtube.com/watch?v=frT3to2ACCw
A great overview of why and how to use selector functions to retrieve data from the store, and derive additional data from store values

- Optimizing React Redux Application Development with Reselect
https://codebrahma.com/reselect-tutorial-optimizing-react-redux-application-development-with-reselect/
A good tutorial on Reselect. Covers the concept of "selector functions", how to use Reselect's API, and how to use memoized selectors to improve performance.

- Usage of Reselect in a React-Redux Application
https://dashbouquet.com/blog/frontend-development/usage-of-reselect-in-a-react-redux-application
Discusses the importance of memoized selectors for performance, and good practices for using Reselect.

- React, Reselect, and Redux
https://medium.com/@parkerdan/react-reselect-and-redux-b34017f8194c
An explanation of how Reselect's memoized selector functions are useful in Redux apps, and how to create unique selector instances for each component instance.

## Normalization
How to structure the Redux store like a database for best performance

- Querying a Redux Store
https://medium.com/@adamrackis/querying-a-redux-store-37db8c7f3b0f
A look at best practices for organizing and storing data in Redux, including normalizing data and use of selector functions.

- Normalizing Redux Stores for Maximum Code Reuse
https://medium.com/@adamrackis/normalizing-redux-stores-for-maximum-code-reuse-ae6e3844ae95
Thoughts on how normalized Redux stores enable some useful data handling approaches, with examples of using selector functions to denormalize hierarchical data.

- Advanced Redux Entity Normalization
https://medium.com/@dcousineau/advanced-redux-entity-normalization-f5f1fe2aefc5
Describes a "keyWindow" concept for tracking subsets of entities in state, similar to an SQL "view". A useful extension to the idea of normalized data.

## Middleware
Explanations and examples of how middleware work and how to write them

- Exploring Redux Middlewares
https://blog.krawaller.se/posts/exploring-redux-middleware/
Understanding middlewares through a series of small experiments

- Redux Middleware Tutorial
https://github.com/pshrmn/notes/blob/master/redux/redux-middleware.md
An overview of what middleware is, how applyMiddleware works, and how to write middleware.

- ReactCasts #6: Redux Middleware
https://www.youtube.com/watch?v=T-qtHI1qHIg
A screencast that describes how middleware fit into Redux, their uses, and how to implement a custom middleware

- A Beginner's Guide to Redux Middleware
https://www.codementor.io/reactjs/tutorial/beginner-s-guide-to-redux-middleware
A useful explanation of middleware use cases, with numerous examples

- Functional Composition in Javascript
https://joecortopassi.com/articles/functional-composition-in-javascript/
Breaking down how the compose function works
