# React Microfrontends

This project is a collection of React microfrontends that can be combined to create a larger application. Each microfrontend is built and deployed independently, allowing for greater flexibility and faster iteration.

## Technologies & Libraries

This project was built using the following technologies and libraries:

#### React

JavaScript library for building user interfaces

#### React Router

routing library for React

#### Redux

predictable state container for JavaScript apps

#### Axios 

promise-based HTTP client for the browser and Node.js

#### Jest

JavaScript testing framework

#### React Testing Library

lightweight testing library for React

#### ESLint 

pluggable and configurable linter tool for identifying and reporting on patterns in JavaScript

#### Prettier 

code formatter that supports various programming languages


## Getting Started

### Prerequisites

Node.js version 16.15.1 or higher \
npm version 8.11.0 or higher

### Setting up environment variables

Before you can start or build the app, you'll need to set up the environment variables by creating a ```.env.local``` file in the root directory of the project. The ```.env.local``` file should contain all the necessary environment variables that the app requires to function.

Here's an example ```.env.local``` file with the required environment variables:

```
REACT_APP_API_URL=
REACT_APP_CLIENT_ID=
REACT_APP_AUTHORITY=
REACT_APP_DOMAIN=
```

To fill in the values for each environment variable, you'll need to obtain the necessary information from the respective services. In the example above, ```REACT_APP_API_URL``` should be replaced with the API URL for your application, and ```REACT_APP_CLIENT_ID``` and ```REACT_APP_AUTHORITY``` should be replaced with the client ID and client secret for the OAuth service you're using.

```REACT_APP_DOMAIN``` should be replaced with the URL of the deployed microfrontend application. 

Once you've added the necessary environment variables to the .env file, you can start or build the app as normal. The environment variables will be loaded into the app at runtime and will be accessible through the process.env object.

## Available Scripts

To install the project dependencies, run:

### `npm install`

This will install all of the necessary packages for the microfrontends.

### `npm start`

This will start a development server for each microfrontend, which can be accessed at http://localhost:3000, http://localhost:3001, http://localhost:3002, and so on.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm run test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the ```dist``` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!


### `npm run lint`

Lints the code using ESLint.

### `Environment Variables`

The microfrontends use different environmental files for different deployment environments. The .env file in the root directory contains the default values, which can be overridden by environment-specific files such as ```.env.development```, ```.env.production``` and ```.env.staging.```

To build the microfrontends for a specific environment, run:

```npm run build:<environment>```

Replace <environment> with the name of the environment you want to build for (e.g. production or staging). This will create a build directory for each microfrontend with the appropriate environmental variables.


