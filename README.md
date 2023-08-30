# MERN Full-Stack Development 2023 > Personal Project 💻

## Individual Project Completed By
* SMU Computer Science Year 3 – Kang Chin Shen (cskang.2020@scis.smu.edu.sg)

## Project Description
### Technologies 
This project is dedicated to constructing a full-fledged **CRUD** (Create, Read, Update, Delete) Blog Application, using the technologies as listed below:

#### MERN Stack
&nbsp;&nbsp;[`MongoDB`](https://www.mongodb.com)
&nbsp;&nbsp;[`Express.js`](https://expressjs.com) 
&nbsp;&nbsp;[`React.js`](https://react.dev/)
&nbsp;&nbsp;[`Node.js`](https://nodejs.org)

#### Frameworks & Tools
&nbsp;&nbsp;[`Mongoose`](https://mongoosejs.com/)
&nbsp;&nbsp;[`Insomnia`](https://insomnia.rest/download)
&nbsp;&nbsp;[`Vite.js`](https://vitejs.dev/)
&nbsp;&nbsp;[`Material UI`](https://mui.com/)
&nbsp;&nbsp;[`Redux`](https://react-redux.js.org)

#### Hosting Services
&nbsp;&nbsp;[`Heroku`](https://www.heroku.com/)
&nbsp;&nbsp;[`Netlify`](https://www.netlify.com/?attr=homepage-modal)

#### Main Concepts
1. Full-stack development with **MERN** 
2. Microservices enforce **REST** Principles
3. Authentication with **JWT** and **Google OAuth API**

## Repository High Level Architecture
```
| mern-full-stack-summer-project-2023                      # Root folder > ./
        | client                                           # Frontend code implemented using React.js
            | src
                | components                               # React components
                | images
        | server                                           # Backend code implemented using Express.js & Node.js
            | controllers
            | routes
            index.js
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
    * `npm install @mui/material @emotion/react @emotion/styled @fontsource/roboto` for styling React components.

#### Generate the template code in [`./server`]()
1. Run `cd server` to change directory into `./server` folder.
2. Create a file `index.js` in `./server` folder.
3. Run the command `npm init -y` to initialise `package.json` file for installation of the following dependencies:
   * `npm install body-parser` for parsing `POST` requests.
   * `npm install cors` for Cross-origin requests.
   * `npm install express` for Express backend framework.
     * Add `"type" : "module"` in `package.json` to use the syntax : `import x from 'x'`.
     * Old syntax : `const x = require('x')`.
   * `npm install mongoose` for ODM (Object Data Modelling) in MongoDB. 
   * `npm install nodemon` for automatic update for any backend changes.
      * Replace the `"scripts" > "test"` in `package.json` to `"scripts" > "start" : "nodemon index.js"`.

## Database Design
#### Connection To MongoDB Cluster
1. Register an account [here](https://www.mongodb.com/cloud/atlas/register).
2. Create a new cluster free of charge with the following configuration:
![Screenshot 2023-07-29 at 9 12 20 PM](https://github.com/cskang0121/mern-full-stack-summer-project-2023/assets/79074359/e9b4392a-467d-47a3-80ba-19c4a714fd69)
3. Create a database user under `Security > Quickstart`.
4. Add IP address of the local machine under `Security > Network Access`.
5. Connect to `MERN-Stack-DB` under `Deployment > Database > Connect to your application (Drivers)`.

#### Schema Design
1. The Schema `PostMessage` has the following definition:
```
const postSchema = mongoose.Schema({
    title: String,
    message: String,
    creator: String,
    tags: [String],
    selectedFile: String,   # An image is converted into string format using react-file-base64
    likeCount: {
        type: Number,
        default: 0
    },
    createdAt: {
        type: Date,
        default: new Date()
    }
})

const PostMessage = mongoose.model('PostMessage', postSchema)
```

   
## Running The Code

## Credits
> Special thanks to **JavaScript Mastery** for contributing to this project! 

## References
* [Full Stack MERN Project](https://www.youtube.com/watch?v=ngc9gnGgUdA&list=PL6QREj8te1P7VSwhrMf3D3Xt4V6_SRkhu&pp=iAQB)
* [Default Exports VS Named Exports](https://medium.com/@etherealm/named-export-vs-default-export-in-es6-affb483a0910)
* [HTTP Status Codes](https://www.restapitutorial.com/httpstatuscodes.html)
* [Material UI Templates](https://mui.com/material-ui/getting-started/templates/)
  
## More
