# Onboarding new developers

A full-stack developer needs to get familiar with three systems used in the Zeeds ecosystem.

- Psychologist portal
- Cloud functions
- Mobile application



## Psychologist portal

The relevant [repository](https://github.com/ZeedsApp/zeeds-admin). 
Clone the repository and navigate to it. 

> Description of the project structure 

### Files at the root of the project
- *netlify.toml* - This file is used to configure your project for deployment to Netlify. It contains information about your project's name, build commands, and environment variables.
- *Dockerfile* - This file is used to build a Docker image for your project. It contains the instructions that Docker will use to create the image, such as the operating system, packages, and files that will be included in the image.
- *craco.config.js* - This file is used to configure CRACO, a tool that helps you customize the build process for your React project. It contains options for things like code splitting, bundling, and minification.
- *.firebaserc* - This file is used to configure your project for deployment to Firebase. It contains information about your Firebase project's name, region, and authentication credentials.
- *cypress.config.js* - This file is used to configure Cypress, a testing framework for React. It contains options for things like test suites, plugins, and reporters.
- *README.md* - This file is a Markdown file that contains a description of your project. It is often used to provide instructions on how to install, run, and test your project.
- *.dockerignore* - This file is used to specify files that should be excluded from the Docker image that is built for your project. This can be helpful for things like temporary files or files that are not needed for production.
- *.gitignore* - This file is used to specify files that should be ignored by Git. This can be helpful for things like binary files or files that are not part of your project's source code.
- *package-lock.json* - This file is a lock file that contains the exact versions of all of the packages that are installed in your project. This can be helpful for reproducibility and preventing conflicts when you share your project with others.
- *package.json* - This file is a manifest file that contains information about your project, such as its name, version, dependencies, and scripts.
- *global.d.ts* - This file is a declaration file that contains type information for global variables and functions. This can be helpful for things like using third-party libraries that export global variables or functions.
- *tsconfig.json* - This file is a configuration file that tells TypeScript how to compile your code. It contains options for things like the target version of TypeScript, the module format, and the file extensions that are used for TypeScript files.
- *docker-compose.yml* - This file is used to define a multi-container Docker application. It contains information about the containers that will be created, the ports that they will expose, and the volumes that they will share.
- *.eslintignore* - This file is used to specify files that should be ignored by ESLint. This can be helpful for things like binary files or files that are not part of your project's source code.
- *tsconfig.path.json* - This file is used to configure the path mappings for TypeScript. It can be helpful for things like resolving relative imports and locating declaration files.
- *.env.example* - This file is used to provide an example of the environment variables that are required by your project. It can be helpful for things like setting up your project's development environment.
 

> Setting up a local environment 

- Install [Node.js](https://nodejs.org/en/download/) if you don't have it already.
- Install [Docker](https://docs.docker.com/get-docker/) if you don't have it already.
- Install [VSCode](https://code.visualstudio.com/download) if you don't have it already.
- Install [Netlify CLI](https://docs.netlify.com/cli/get-started/) if you don't have it already.
- Install [Cypress](https://docs.cypress.io/guides/getting-started/installing-cypress.html#System-requirements) if you don't have it already.

> Setting up the environment variables

- Create a file named `.env` in the root directory of the project.
- Copy the contents of `.env.example` into `.env`.

> Running the project locally

- Run `npm install` to install the project dependencies.
- Run `npm start` to start the development server.

If everything goes well, the development server should start on `http://localhost:3000`.



## Cloud functions


The relevant [repository](https://github.com/ZeedsApp/zeeds-functions). Clone the repository and navigate to it.

> Description of the project structure

### Files at the root of the project
- *Dockerfile* - This file is used to build a Docker image for your project. It contains the instructions that Docker will use to create the image, such as the operating system, packages, and files that will be included in the image.
- *README.md* - This file is a Markdown file that contains a description of your project. It is often used to provide instructions on how to install, run, and test your project.
- *docker-compose-with-firebase-functions.yml* - This file is used to define a multi-container Docker application. It contains information about the containers that will be created, the ports that they will expose, and the volumes that they will share.
- *docker-compose.yml* - This file is used to define a multi-container Docker application. It contains information about the containers that will be created, the ports that they will expose, and the volumes that they will share.
- *firebase.json* - This file is used to configure your project for deployment to Firebase. It contains information about your Firebase project's name, region, and authentication credentials.
- *firebase_emulator_baseline* - This file is used to configure your project for deployment to Firebase. It contains information about your Firebase project's name, region, and authentication credentials.
- *package-lock.json* - This file is a lock file that contains the exact versions of all of the packages that are installed in your project. This can be helpful for reproducibility and preventing conflicts when you share your project with others.
- *package.json* - This file is a manifest file that contains information about your project, such as its name, version, dependencies, and scripts.
- *public* - This folder is used to store static assets, such as images and fonts.
- *functions* - This folder is used to store the source code for your Firebase functions. It contains files that are used to configure your Firebase functions, such as the name of your functions and the region that they will be deployed to.
- *hasura* - This folder is used to store the source code for your Hasura GraphQL engine. It contains files that are used to configure your Hasura GraphQL engine, such as the name of your Hasura GraphQL engine and the region that it will be deployed to.

### Files in the functions directory
- *README.md* - This file is a Markdown file that contains a description of your project. It is often used to provide instructions on how to install, run, and test your project.
- *\_\_tests__* - This folder is used to store the source code for your Firebase functions tests. It contains files that are used to configure your Firebase functions tests, such as the name of your functions tests and the region that they will be deployed to.
- *package-lock.json* - This file is a lock file that contains the exact versions of all of the packages that are installed in your project. This can be helpful for reproducibility and preventing conflicts when you share your project with others.
- *package.json* - This file is a manifest file that contains information about your project, such as its name, version, dependencies, and scripts.
- *src* - This folder is used to store the source code for your Firebase functions. It contains files that are used to configure your Firebase functions, such as the name of your functions and the region that they will be deployed to.
- *tsconfig.dev.json* - This file is a configuration file that tells TypeScript how to compile your code. It contains options for things like the target version of TypeScript, the module format, and the file extensions that are used for TypeScript files.
- *tsconfig.json* - This file is a configuration file that tells TypeScript how to compile your code. It contains options for things like the target version of TypeScript, the module format, and the file extensions that are used for TypeScript files.

> Setting up a local environment 

- Install [Node.js](https://nodejs.org/en/download/) if you don't have it already.
- Install [Docker](https://docs.docker.com/get-docker/) if you don't have it already.
- Install [VSCode](https://code.visualstudio.com/download) if you don't have it already.
- Install [Firebase CLI](https://firebase.google.com/docs/cli) if you don't have it already.

> Running the project locally

**It is important to note that this repository holds 3 parts to the project:**
- Hasura GraphQL engine
- Postgres database
- Firebase functions


**To run the project locally, you need to run the following commands:**
- `docker-compose up -d` to start the Hasura GraphQL engine and Postgres database.
- Navigate to the `functions` directory and run `npm install` to install the project dependencies for the Firebase cloud functions instance.
- `firebase login` to login to your Firebase account.
- `firebase use --add` to select the Firebase project that you want to use, we use the `staging` instance to select the staging environment as Firebase requires a project to deploy to but that is irrelevant in our case as all the deployment is handled via PRs and Github Actions.
- `npm run serve` to start the Firebase cloud functions instance.

If everything goes well, you should have Firebase function emulator running on your computer.

## Testing the functionality between the local instances of the cloud functions and the psychologist portal

With the local instances of the cloud functions and the psychologist portal running, you can test the functionality between them.
Open your browser and open the psychologist portal on `http://localhost:3000` and the Hasura GraphQL engine on `http://localhost:8080/console`.
The Hasura GraphQL engine will ask for an admin secret, you can find it in .env.example file in the root of the project. It is named `REACT_APP_X_HASURA_ADMIN_SECRET`.

With the portal open go ahead and register a new user. You can use the following credentials:
```
Name - Test
Your Email - testuser@zeeds.com
Organization - Zeeds
Phone Number - 123456789
Password - 123456
```

After you register a new user, you should be able to see it in the Hasura GraphQL engine. To do that, go to the `Data` tab and select the `admin_user` table. You should be able to see the admin user you just registered. In order to be able to login, you need to set the `is_active` field to `true`. You can do that by clicking on the `Edit` button next to the user you just registered. After you set the `is_active` field to `true`, you should be able to login to the portal with the credentials you just registered with. The portal will send a verification code to the number you set in when you registered, but since this is a simulated environment the verification code will be printed out in the terminal where you started the Firebase cloud functions instance. You can copy the verification code from the terminal and paste it in the portal to verify your phone number. A successful verification will redirect you to the dashboard.


## Mobile application


The relevant [repository](https://github.com/ZeedsApp/Zeeds). Clone the repository and navigate to it.

> Description of the project structure

### Files at the root of the project


- *App.tsx* - This file is the main entry point for your React application. It is responsible for rendering the application's UI and handling user interactions.
- *README.md* - This file is a Markdown file that contains a description of your project. It is often used to provide instructions on how to install, run, and test your project.
- *app.config*.js - This file is used to configure the application's environment. It contains options for things like the application's port, the database connection string, and the API endpoint.
- *babel.config.js* - This file is used to configure Babel, a tool that helps you convert JavaScript code into a format that can be understood by older browsers. It contains options for things like the target version of JavaScript, the plugins that are used, and the presets that are applied.
- *bitrise.yml* - This file is used to configure Bitrise, a platform that helps you automate the build, test, and deployment of your applications. It contains information about the steps that Bitrise should take to build and deploy your application.
- *codegen.ts* - This file is used to generate code from a template. It can be helpful for things like creating boilerplate code or scaffolding new features.
- *coverage* - This directory contains the coverage reports for your project's tests. These reports can be used to identify which parts of your code are not being tested.
- *defines.d*.ts - This file is a declaration file that contains type information for constants and variables that are defined in your project. This can be helpful for things like using third-party libraries that export constants or variables.
- *e2e* - This directory contains the files that are used for end-to-end testing. End-to-end tests are used to test the entire application from the user's perspective.
- *eas-hooks* - This directory contains the hooks that are used to interact with the Expo App Services API. The Expo App Services API provides a way to access features like push notifications, analytics, and crash reporting.
- *eas.json* - This file is used to configure the Expo App Services API for your project. It contains information about the project's name, the app's ID, and the app's secret.
- *graphql.config.yaml* - This file is used to configure the GraphQL client for your project. It contains information about the GraphQL endpoint, the authentication credentials, and the schema.
- *index.js* - This file is the entry point for the application's Node.js server. It is responsible for starting the server and loading the application's code.
- *metro.config.js* - This file is used to configure Metro, a tool that helps you build React Native applications. It contains options for things like the project's root directory, the packager's port, and the plugins that are used.
- *package-lock.json* - This file is a lock file that contains the exact versions of all of the packages that are installed in your project. This can be helpful for reproducibility and preventing conflicts when you share your project with others.
- *package.json* - This file is a manifest file that contains information about your project, such as its name, version, dependencies, and scripts.
- *src* - This directory contains the source code for your project. This code can be written in JavaScript, TypeScript, or React Native.
- *tsconfig.json* - This file is a configuration file that tells TypeScript how to compile your code. It contains options for things like the target version of TypeScript, the module format, and the file extensions that are used for TypeScript files.
- *unit_tests* - This directory contains the files that are used for unit testing. Unit tests are used to test small, isolated parts of your code.


> Setting up a local environment

- Install [Node.js](https://nodejs.org/en/download/) if you don't have it already.
- Install [VSCode](https://code.visualstudio.com/download) if you don't have it already (it is the best code editor by far).
- Install [Expo CLI](https://docs.expo.dev/get-started/installation/) if you don't have it already.

> Running the project locally

- Run `npm install` to install the project dependencies.
- Run `npm run ios` or `npm run android` to start the development server and open the application in the iOS or Android simulator.

If everything goes well, you should have the application running on your computer.

## Testing the functionality between the local instances of the cloud functions and the mobile application

With the local instances of the cloud functions and the mobile application running, you can test the functionality between them by clicking on the login button on the mobile application. This interacts with the cloud functions and if everything is set up correctly, you should navigate to the next screen in the application. As we are running in development mode, the sign in through BankID will not be necessary and you can just click on the button to continue to the next screen, which in the background will create an anonymous user. You can view the details of that user in Hasura.



## Publishing a new version of the app. 
To start with you need to update the version number of the mobile repository in the package-lock.json file and the package.json file. During this you should also update the version number as it exists in the frontend code to the in animatedsplashview.tsx and profile.tsx(previously this was possible to do using the config file but that has not worked since 2.7.9). These changes should be included in the merge request for your new project. once they have been merged you pull them to the repository you are working in using the terminal and the command git pull. after that you use the command eas build --platform ios to create a new build in expo dev and then you use the eas submit --platform ios. After that the app has been updated and is ready to be released for testflight.



## RevenueCat integration
Revenuecat is a third partyy softaware used to make it easier for us to handle purchases. To create a new purchase(like a course) you first create a non-consumable in app store connect add all the values and save it then in revenuecat import the purchase to revenuecat and attach it to the correct offering and then it is usable.



