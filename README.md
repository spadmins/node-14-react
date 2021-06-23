
<img width="100" src="https://cdn.springpeople.com/media/reactjs.png" />

# Node 14 + React Project

## Getting started

### Accessing terminal

 - Select Terminal from the menu > Open Terminal in specific container (Ctrl + `) > Select ``nodejs``

### Creating package.json

 - Create a package.json file using `npm init`
 - Then, once you have a package.json file, use
    - `npm install <pkg> --save`
    - `npm install <pkg> --save-dev`
 - [Refer here](https://docs.npmjs.com/creating-a-package-json-file) for more information on package.json

### To get the frontend running locally:

- `npm install` to install all req'd dependencies
- `npm start` to start the local server (this project uses create-react-app)

> Local web server will use port **4100** instead of standard React's port **3000** to prevent conflicts with some backends like Node or Rails. You can configure port in scripts section of `package.json`: we use [cross-env](https://github.com/kentcdodds/cross-env) to set environment variable PORT for React scripts, this is Windows-compatible way of setting environment variables.<br/><br/>
> Alternatively, you can add `.env` file in the root folder of project to set environment variables (use PORT to change webserver's port). This file will be ignored by git, so it is suitable for API keys and other sensitive stuff. Refer to [dotenv](https://github.com/motdotla/dotenv) and [React](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-development-environment-variables-in-env) documentation for more details. Also, please remove setting variable via script section of `package.json` - `dotenv` never override variables if they are already set.
