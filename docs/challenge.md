
<img src="https://play-lh.googleusercontent.com/ESPEFSHC_T6NGI54ljG9YsYZv5MmH5jAQhonikjtgkzvzEaXGTOY85ePieT7V5BPL2E=w480-h960-rw"
     alt="Zeeds logo"
     style="float: left; margin-right: 10px; width: 48px; border: 1px solid black" />

Zeeds Exercise #1

---

We at Zeeds use the following technologies (ordered by importance).
*Items marked with an asterix (\*) can change in the future*.

- Typescript
- React Native
- React
- GraphQL
- PostgreSQL
- Hasura
- Firebase*
- Docker

You will need to be somewhat familiar with all of these items in order to complete this task.

---

## The Challenge

### Description

This exercise has three major parts, the app, backend and portal. The app has to be able to compile and run on both iOS and Android.
You are expected to produce an app for both iOS and Android via Expo. You can read more about it [here](https://docs.expo.dev/build/introduction/). The app should be able to run on both iOS and Android and the code should be written in Typescript. The output package should be provided to us in a zip file so that we can test it on our own simulators.

The second part involves creating a backend with the help of Firebase and Hasura in order to handle requests and store data that gets transmitted between the app and the portal. Since Hasura is an intermediary service you will have to use some kind of database for the actual data storage, for this you will use PostgreSQL.
In order to showcase your knowledge with Docker containers, we recommend that you use Docker to run the Hasura and Postgres services. You can read more about Docker [here](https://docs.docker.com/get-started/overview/). Both Hasura nad Postgres have official Docker images that you can use. For the cloud functions, you can use Firebase's own cloud functions. You can read more about them [here](https://firebase.google.com/docs/functions). The easiest way to setup Firebase is to use the Firebase CLI. You can read more about it [here](https://firebase.google.com/docs/cli).

The portal is the last part of the exercise, and it involves creating a web page by using React. API communication to Hasura happens via GraphQL and not REST. REST communication is allowed when communicating with Firebase as Firebase will only be used for authentication purposes. **Remember that all the code is typed in Typescript**.

### Expectations

You are expected to create an app that requires a user to log in. Once the user has logged in, the user arrives at a screen that has three bottom tabs. The default tab should be the middle one. In the middle tab there should be centered text called "My favorite number" and the user's favorite number. Initially there will not be one, so the app will prompt the user to enter one. The middle tab should also have a button called "Update" where when clicked, the user can update their favorite number. The tab to the left displays the user's favorite number but does not have the functionality to update it. The same for the tab to the right. 

It is expected from you to have at least three seperate repositories, one for the app, one for the portal and one for the backend. When submitting your solution, please provide us with the links to the repositories as well as instructions on how to run the app and the portal.

The final app should be published on Expo and it should be runnable on both iOS and Android.

Any updates the user makes have to be stored on the Postgres database. You are expected to interact with the Postgres database via Hasura as a middle-man and perform these updates via only GraphQL requests (hint: use mutations).

You are expected to build a website that also has a login screen where the user logs in and can view their favorite number.

--- 

## Grading

The factors that will be taken in consideration when evaluation your final result are:

- the usage of Typescript (code quality, reusability and simplicity)
- the usage of Hasura (integration with aforementioned systems as well as correct integration with Postgres database)
- proper usage of React hooks by not creating unnecessary re-renders
- usage of Expo (proper building and compiling on both platforms)
- clear instructions on how to run the app and the portal. If we cannot reproduce the environment that you've described, we unfortunately cannot grade your solution.







