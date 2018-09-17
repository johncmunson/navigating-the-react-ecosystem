# Navivigating the React Ecosystem

_a quick note before getting started..._

If you _still_ haven't gotten up to speed with the syntax features added to Javascript through ES6, stop now and [read this](https://github.com/lukehoban/es6features) and test out your code [here](https://babeljs.io/en/repl). The most commonly used new features (at least in React development) are arrow functions, classes, template strings, destructuring, default + rest + spread, let + const, promises, and modules. ES6 is prevalent throughout React codebases and you should be familiar with it before you start digging in. At this point, even ES7/8 features are becoming more prevalent, such as async + await.

### Getting Started

There is a project maintained by Facebook called `create-react-app`. Some people might claim this project is for beginners and toy applications, but they are wrong. I highly recommend using this tool, as it will steer you in the right direction and let you focus on application architecture rather than application infrastructure. If the needs of the application one day outgrow what `create-react-app` provides out of the box then great! You can always eject at any time, but I recommend avoiding this for as long as possible. To eject your application is to expose the underlying config files and scripts that are powering everything, and it is a permanent action.

When you begin learning, start with the [main concepts](https://reactjs.org/docs/hello-world.html) section in the official docs. You should be able to get through all twelve concepts in a day.

From here, it's time to graduate to more in-depth tutorials and guides, preferably ones that walk you through the entire process of building a small to medium sized application that communicates with an API. There are a wealth of resources available. Choose one, or a couple, that are up to date and well maintained. If you are a small team all learning together, you should learn from the same resources so as to all be on the same page with each other. Allow yourself at least a full week to get up to speed with the basics, especially if you also intend to learn Redux.

Here are a couple of my recommendations...

- React
  - [Tutorial from official docs](https://reactjs.org/tutorial/tutorial.html)
  - [The Beginner's Guide to React](https://egghead.io/courses/the-beginner-s-guide-to-react)
  - [React for Beginners](https://reactforbeginners.com/)
  - [React Fundamentals](https://tylermcginnis.com/courses/react-fundamentals/)
  - [Fullstack React](https://www.fullstackreact.com/) (also covers Redux)
- Redux
  - [Official docs](https://redux.js.org/)
  - [Redux Fundamentals](https://tylermcginnis.com/courses/redux/)
  - [Getting Started With Redux](https://egghead.io/courses/getting-started-with-redux)
  - [Building React Applications with Idiomatic Redux](https://egghead.io/courses/building-react-applications-with-idiomatic-redux)
  - [Practical Redux](https://www.educative.io/collection/5687753853370368/5707702298738688)


_A note about Redux..._ Redux can really refer to two things. There is Redux the library and there is Redux the architectural pattern (which is itself a refinement of the Flux pattern pioneered at Facebook). There is a growing trend in the community to start transitioning away from dependence on Redux the library, while still maintaining the architectural patterns that it encouraged. My recommendation... for those who have never used it, you should. For those who have mastered it, start weening yourself off of it. Beginners will benefit from the wealth of Redux middleware the community has built over the past several years. Lastly, you may hear Redux described in terms of MVC. This is wrong. Redux is a new architectural pattern altogether, do not pollute it by bringing along MVC baggage. You may find Redux to be a steeper learning curve than React at first, but it is well worth the time investment.


### Recommended Libraries

React is an ecosystem just as much as it is a library. The same can be said for Redux. You do not have to utilize all of these libraries, and many of them can gradually be added to the codebase as needed. However, all of these libraries are first-class, grade A, battle tested projects that will without a doubt improve the the maintainablity and scalability of your application when implemented properly.

- redux (data management)
- xstate (state management / hierarchichal state machine)
- styled-components (styling)
- react-router (routing)
- reselect (memoized selectors)
- redux-thunk (async actions)
- redux-persist (persist and rehydrate a redux store)
- normalizr (normalize your redux store)
- redux-orm (interact with redux store like a database)
- lodash (functional utilities)
- recompose (like lodash for react components)
- immer (helps to simplify redux reducers)
- storybook (component prototyping)
- jest (unit testing)
- react-testing-library (component testing)
- cypress (E2E testing)
- flow (type system) or prop-types (prop checking)
- eslint (linting)
- prettier (auto-formatter)
- husky (git hooks)


### Common Patterns

These patterns are common enough that you should be somewhat familiar with them. Used correctly, they can make for very efficient composition and reuse and will enable proper separation of concerns as your applications grow.

- [Compound Components](https://www.youtube.com/watch?v=hEGg-3pIHlE)
- [Function as](https://www.youtube.com/watch?v=WE3XAt9P8Ek) [Child Components](https://cdb.reacttraining.com/use-a-render-prop-50de598f11ce)
- [Higher Order Components](https://www.youtube.com/watch?v=LTunyI2Oyzw&amp=&t=)
- [Smart + Dumb Components](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0)
- ... and [many](https://reactpatterns.github.io/) [more](https://egghead.io/courses/advanced-react-component-patterns)


### Influential React Developers

These guys have been instrumental in helping grow the React ecosystem. Most of them are active on twitter, maintain React blogs, produce course content, and/or speak at conferences.

- Dan Abramov
- Kent C. Dodds
- Tyler McGinnis
- Ryan Florence
- Michael Jackson
