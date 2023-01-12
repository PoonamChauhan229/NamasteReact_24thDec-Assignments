# Q1. What is `NPM`?
- npm is the package manager for Node.js. It was created in 2009 as an open source project to help JavaScript developers easily share packaged modules of code.
- The npm Registry is a public collection of packages of open-source code for Node.js, front-end web apps, mobile apps, robots, routers, and countless other needs of the JavaScript community.
- npm is the command line client that allows developers to install and publish those packages
- NPM is the default package manager for JavaScript's runtime Node.js.
- It's also known as "Ninja Pumpkin Mutants", "Nonprofit Pizza Makers", and a host of other random names that you can explore and probably contribute to over at npm-expansions(https://github.com/npm/npm-expansions)
-Npm alternative is Yarn and It can be initialized as follows
npm init => need to provide all the configuration details 
npm init -y can be used to skip the setup steps, npm takes care of it and creates the package.json json file automatically , but without configurations.
### NPM consists of two main parts:
1. a CLI (command-line interface) tool for publishing and downloading packages, and
2. an online repository that hosts JavaScript packages


# Q2. What is `Parcel/Webpack`? Why do we need it?
- Parcel and webpack are the bundlers used mostly for JavaScript or Typescript code that helps you to minify, clean, and make your code compact so that it becomes easier to send a request or receive the response from the server when it usually takes you to transfer multiple files without using any bundler for loading the page of your application.
- Both of these bundlers substantially reduce the time it takes for the transfer of data and files to the server from the application.
- Along with that both bundlers parcel and webpack remove the unnecessary comments, new lines, any kind of block delimiters, and white spaces while the functionality of the code remains unchanged.

Features:
https://parceljs.org/features/development/

Documentation:
https://parceljs.org/getting-started/webapp/

![parcel](https://user-images.githubusercontent.com/68181154/212066086-00847659-5cc7-4c6f-90fe-d9d25b34aad1.png)

# Q3.What is `.parcel-cache`
The .cache folder (or .parcel-cache in parcel v2) stores information about your project when parcel builds it, so that when it rebuilds, it doesn't have to re-parse and re-analyze everything from scratch. It's a key reason why parcel can be so fast in development mode. 

npx parcel build index.html

# Q4.What is `npx` ?

NPX is an NPM package executor.

Why npx has a 'x'? 🤔
Well, the x mostly likely is for eXecute

With NPX, we can run and execute packages without having to install them locally or globally.

if we run any executables with NPX means, first it will try to find the packages (locally or globally installed), and try to run those,

If the package was not previously installed means, NPX will create a temporary cache of that package and execute it, once the execution is over, it will remove the cache from the system.

The point to note here is, that NPX will never install any package, it just creates a temporary cache and executes it,

# Q4. What is difference between `dependencies` vs `devDependencies`

- In every web application project, we have a file called package.json. This file contains all the relevant data regarding the project i.e. metadata. Starting from all the dependencies used to all the version numbers are present in the file.
- In this way, there are three types of dependencies that are found in this file. They are dependencies, dev dependencies, and peer dependencies

### Dependencies	
- In package.json file, there is an object called as dev
- A dependency is a library that a project needs to function effectively.
- If a package doesn’t already exist in the node_modules directory, then it is automatically added. 
- These are the libraries you need when you run your code.
- Included in the final code bundle. 
- Dependencies can be added to your project by running :
- npm install <package_name>

### devDependencies	
- consists of all the packages that are used in the project in its development phase and not in the production or testing environment with its version number. So, whenever you want to install any library that is required only in your development phase then you can find it in the dev Dependencies object.
- DevDependencies are the packages a developer needs during development
- As you install a package, npm will automatically install the dev dependencies.
- These dependencies may be needed at some point during the development process, but not during execution.
- Included in the final code bundle .
- Dev dependencies can be added to your project by running :
- npm install <package_name> --save-dev

# Q5. What is Tree Shaking?
- Tree shaking is a term commonly used within a JavaScript context to describe the removal of dead code.
- Tree shaking or dead code elimination means that unused modules will not be included in the bundle during the build process.
- “Tree-shaking” is a must-have performance optimization when bundling JavaScript.

# Q6. What is Hot Module Replacement?
