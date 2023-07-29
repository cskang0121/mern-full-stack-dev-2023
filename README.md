## Project Description

### Technologies 
This project is dedicated to constructing a full-fledged **CRUD** (Create, Read, Update, Delete) Social Media Application, using the **MERN** and other technologies as listed below:

#### MERN Stack
&nbsp;&nbsp;[`MongoDB`](https://www.mongodb.com)
&nbsp;&nbsp;[`Express.js`](https://expressjs.com) 
&nbsp;&nbsp;[`React.js`](https://react.dev/)
&nbsp;&nbsp;[`Node.js`](https://nodejs.org)

#### Frameworks & Tools
&nbsp;&nbsp;[`Vite`](https://vitejs.dev/)
&nbsp;&nbsp;[`Redux`](https://react-redux.js.org)

#### Hosting Services
&nbsp;&nbsp;[`Heroku`](https://www.heroku.com/)
&nbsp;&nbsp;[`Netlify`](https://www.netlify.com/?attr=homepage-modal)

#### Main Concepts
1. Full-stack development with **MERN** 
2. Microservices enforces **REST** Principles
3. Authentication with **JWT** and **Google OAuth API**

## Repository High Level Architecture
```
| mern-full-stack-summer-project-2023                      # Root folder > ./
    | client
    | server
    # Sub folder 3 ...
```

#### Generate the template code in [`./client`]()
1. Run `cd client` to change directory into `./client` folder.
2. Run `npm install -g vite` to install Vite globally using NPM.
3. Run `npm create vite ./ --template react` to generate the frontend code in `./client` folder.
    * Choose `Select a framework > React`.
    * Choose `Select a variant   > JavaScript`.
4. Install the following dependencies:
    * `npm install axios` for making API requests.
    * `npm install moment` for working with datetime in React.
    * `npm install react-file-base64` for working with images in React.
    * `npm install redux` for state management.
    * `npm install redux-thunk` for asynchronous actions used in Redux.

#### Generate the template code in [`./server`]()
1. Run `cd server` to change directory into `./server` folder.
2. Create a file `index.js` in `./server` folder.
3. Run the command `npm init -y` to initialise `package.json` file for installation of the following dependencies:
   * `npm install body-parser` for parsing `POST` requests.
   * `npm install cors` for Cross-origin requests.
   * `npm install express` for Express backend framework.
     * Add `"type" : "module"` in `package.json` to use the syntax : `import x from 'x';`.
     * Old syntax : `const x = require('x')`.
   * `npm install mongoose` for ODM (Object Data Modelling) in MongoDB.
   * `npm install nodemon` for automatic update for any backend changes.
      * Replace the `"scripts" > "test"` in `package.json` to `"scripts" > "start" : "nodemon index.js"`.

## Database Design

## Running The Code

## Credits
> Special thanks to **JavaScript Mastery** for contributing to this project! 

## References
- [Full Stack MERN Project](https://www.youtube.com/watch?v=ngc9gnGgUdA&list=PL6QREj8te1P7VSwhrMf3D3Xt4V6_SRkhu&pp=iAQB)

## More
