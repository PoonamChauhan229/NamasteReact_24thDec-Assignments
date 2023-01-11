## Q1.What is Emmet?
- Emmet is a built-in feature in Visual Studio Code. 
- We don’t have to install any extensions for emmet support.
- Emmet prevents us from writing the entire code by yourself by providing Emmet abbreviation.
- Emmet is enabled by default in html, haml, pug, slim, jsx, xml, xsl, css, scss, sass, less and stylus files, and also in languages that inherits from any of the above like handlebars and PHP.

## Q2. Difference between a Library and Framework?
Library:
1. Libraries provide developers with predefined functions and classes to make their work easier and boost the development process.
2. By using a library, you can control the flow of the application and call the library.
3. Generally, libraries are a collection of helper modules, objects, classes, functions, message templates, pre-written code, etc.
4. Codes in libraries are geared toward a particular program or to solve a specific development problem. Therefore, developers must modify library code to meet their needs.
5. It is possible to call a library out of context. You may use the library wherever you see fit in your code.
6. In the program linking and binding process, they play an important role.
7. Having a library means understanding the functionality of each method, and it isn’t easy to create complex interactions since you need to call many methods to get the desired results
8. Generally, libraries aren’t designed for extensibility; they are designed to accomplish a specific purpose.
9. It is easy to replace a library with another library. For instance, if you do not like the jQuery date picker library, you can use another date picker like a bootstrap date picker or pick date.
10. Less code is required to build libraries, which leads to faster loading times and better performance.
11. The purpose of libraries is to perform a defined and specific task. Eg: Image manipulation, network protocols, math operations, etc.
12. You can integrate libraries seamlessly into existing projects to add functionality. 
13. Good code quality, reusability, and control, enhanced speed and performance of the program, etc.

Framework:
1. Framework, on the other hand, is like the foundation upon which developers build applications for specific platforms.
2. In contrast, when you use a framework, the control is inverted, i.e., the framework controls the flow and calls your code.
3. Frameworks consist of a lot of APIs, compilers, toolsets, support programs, libraries, etc.
4. Despite the fact that frameworks generate new codes for developers. These codes cannot be altered or modified later. Unlike libraries, frameworks do not allow users to modify their pre-written codes, so you don’t have to worry about deleting or changing them.
5. On the other hand, you can only call and use what belongs to a Framework within the same Framework. 
6. Using them, you can build and deploy applications in a standard way as the framework already provides code to perform common tasks and uses code provided by a developer for custom functionality.
7. Frameworks, on the other hand, embody the basic flow, and since plugins need to be added to code, it is easier to do the right modification.
8. Frameworks provide general functionality. Because of this, they are built to be extensible, which allows developers to incorporate app-specific features without modifying the framework’s source code.
9. Frameworks are difficult to replace. If, for instance, you were using AngularJS to build your product, you cannot simply swap it out for another framework. It requires rewriting the entire codebase.
10. Developing a framework requires a lot of coding, which increases loading times and decreases performance.
11. Frameworks can be used for performing a wide range of tasks. Among these are Web application systems, plug-in managers, GUI systems, and so on.
12. Incorporating frameworks seamlessly into an existing project is impossible. Instead, frameworks should be used when starting a new project.
13. Faster programming, support from the community, great support for MVC (Model View Controller) pattern, etc.


## Q3.What is CDN? Why do we use it?
A Content Delivery Network, or a CDN as it is commonly called, is an essential part of any modern website and application

The content that you view on your phones today, on any website or app, videos or images, or any other kind of content, is very likely to be delivered using a content delivery network.

A Content Delivery Network or a CDN is a globally-distributed network of servers that helps provide high-availability, faster performance, and security to websites distributing their content via it.

### Why do I need a CDN?
The number one reason for using a CDN is to improve your user’s experience in terms of speed, and as we know – speed matters!

Ensuring a consistent experience for all your users is important.

A website may be hosted in a particular region, but if the majority of its users are coming from an entirely different region – e.g., if your site is hosted in North America, GTmetrix might report fast speeds based on our default test location, but if a good chunk of your users come from Europe, their speed will not be as fast as you experience it to be.

CDNs not only ensure a faster experience to your users, but they also help to prevent site crashes in the event of traffic surges – CDNs help to distribute bandwidth across multiple servers, instead of allowing one server to handle all traffic

- Improve page load speed
- Handle high traffic loads
- Block spammers, scrapers
- Localize coverage without the cost
- Reduce bandwidth consumption
- Load balance between multiple servers
- Secure the application


## Q4.Why is React known as React?
React is called React because it was designed to be a declarative, efficient, and flexible JavaScript library for building user interfaces.

React is named React because of its ability to react to changes in data. When the data in a React component changes, React will automatically re-render the component so that it reflects the new data. This makes it easy to create performant user interfaces that always look up-to-date

React makes it painless to create interactive UIs.

Design simple views for each state in your application, and React will efficiently update and render just the right components when your data changes.

## Q5.What is crossorigin in script tag?
The crossorigin attribute on a <script> tag specifies that CORS is supported when loading an external script file from a third party server or domain.

The purpose of crossorigin attribute is used to share the resources from one domain to another domain.

Basically, it is used to handle the CORS request.

It is used to handle the CORS request that checks whether it is safe to allow for sharing the resources from other domains

CORS is a standard mechanism used to retrieve files from other domains.

### Using crossorigin
- The crossorigin attribute specifies that the script element supports CORS.
- CORS stands for Cross Origin Resource Sharing.
- CORS is a standard mechanism to retrieve files from a third party domain or server.
- If specified, the script file request will be sent with or without credentials.
- This attribute is only relevant when the script is retrieved from a third party server. Do not use this attribute when these files are on your own server.

<script type="text/javascript" src="my_script.js" crossorigin="anonymous"></script>

### Values: This attribute contains two values which are given below

1. anonymous: It has a default value. It defines a CORS request which will be sent without passing the credential information.
2. use-credentials: A cross-origin request will be sent with credentials, cookies, and certificate.

## Q6.What is diference between React and ReactDOM
React contains functionality utilised in web and mobile apps.

The reason React and ReactDOM were split into two libraries was due to the arrival of React Native. 

ReactDOM functionality is utilised only in web apps

When building web applications in React, we use two packages—react and react-dom

React is a JavaScript library for building User Interfaces and ReactDOM is the JavaScript library that allows React to interact with the DOM.

React library is responsible for creating views and ReactDOM library is responsible to actually render UI in the browser.

Including Scripts: Following are the CDN links for React and ReactDOM:

React: https://cdnjs.com/libraries/react
ReactDOM: https://cdnjs.com/libraries/react-dom

<script crossorigin src="https://unpkg.com/react@17/umd/react.development.js"></script>

<script crossorigin src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"></script>

## Q7.What is difference between react.development.js and react.production.js files via CDN?

### react.development.js
- Development mode includes useful warnings and gives you access to tools that make development and debugging easier.
- The development build is used - as the name suggests - for development reasons. You have Source Maps, debugging and often times hot reloading ability in those builds.
- The versions are only meant for development, and are not suitable for production. 
<script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>

<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>

### react.production.js
- Production mode minifies your code and better represents the performance your app will have on end users' devices.
- The production build runs in production mode which means this is the code running on your client's machine.
- Minified and optimized production versions of React are available at
- To deploy the application in the production environment, use below scripts.

<script crossorigin src="https://unpkg.com/react@18/umd/react.production.min.js"></script>

<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>

## Q8.What is async and defer?

When the web page is loaded, the web browser looks at the entire HTML document and looks for any CSS, JavaScript and images that are referenced by that page. This is what we refer as HTML Parsing
### async
- In case of async, the script is loaded parallelly and once loaded, parsing is halted, script is compiled and after that parsing is resumed.
- With async (asynchronous) attribute, the HTML parsing continues until the browser fetches the script file over the network so parsing and script fetching happens in parallel
- Once the scripts are available in the browser, HTML parsing is paused and scripts are executed. Once the execution is complete, HTML parsing continues
- So this is an asynchronous way of downloading scripts

Image 2 to be addded

### defer
- In case of defer, the script is loaded parallelly but compilation is only done when whole parsing is done
- The word ‘defer’ in English means to ‘hold back’. So with defer attribute mentioned in the script tag, the script files are downloaded in parallel while the HTML parsing continues
- But the execution is deferred until the HTML parsing is done.
- In simple words, the downloaded scripts are executed only when the browser finishes its HTML parsing.

Image 3 to be added

### When to use ‘async’ and when to use ‘defer’?
Well, you can use async attribute when your page does not depend on the script files (for example analytics). Why? Because async cannot guarantee the order in which your scripts files will be downloaded. So if there is any dependency amongst your script files, it may break your code. In such cases you can use defer attribute.

### Final Thoughts
Now that we have async and defer attributes, we can put our script references in head tag and as this allows your scripts to be downloaded asap without blocking your browser. If you are not using these keywords, make sure to put it at the bottom before closing your body tag. This will ensure that the HTML parser is not blocked by the scripts.