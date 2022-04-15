# multer-mern-image-uploader

# 🚀 Javascript full-stack 🚀

## MERN Stack

### React / Express / MongoDB / Redux

https://github.com/coding-to-music/multer-mern-image-uploader

https://multer-mern-image-uploader.herokuapp.com

by MrsKamran https://github.com/MrsKamran

https://github.com/MrsKamran/habit-tracker

<!-- Please update value in the {}  -->

<h1 align="center">Image Uploader</h1>

<div align="center">
   Solution for a challenge from  <a href="http://devchallenges.io" target="_blank">Devchallenges.io</a>.
</div>

<div align="center">
  <h3>
    <a href="https://https://image-uploader-67dc9.web.app/">
      Demo
    </a>
    <span> | </span>
    <a href="https://{your-url-to-the-solution}">
      Solution
    </a>
    <span> | </span>
    <a href="https://devchallenges.io/challenges/O2iGT9yBd6xZBrOcVirx">
      Challenge
    </a>
  </h3>
</div>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [Overview](#overview)
- [Built With](#built-with)
- [Features](#features)
- [How to use](#how-to-use)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

<!-- OVERVIEW -->

## Overview

![screenshot](https://i.ibb.co/X4YcSFd/imageupload-init.jpg)
![progress bar](https://i.ibb.co/nmWyxVG/progressbar.jpg)
![final result](https://i.ibb.co/F0y7vXV/imageuploader-result.jpg)

This is an Image Uploader application. User can :

-Drag and drop image an image to Upload it
-Choose to select an image from folder
-See a loader when image is uploading
-See the image and copy it when the image is uploaded
-Can choose to copy to the clipboard

### Built With

<!-- This section should list any major frameworks that you built your project using. Here are a few examples.-->

- [React](https://reactjs.org/)
- [Nodejs](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [Mongoose](https://mongoosejs.com/)
- [Sass](https://sass-lang.com/)

## Features

<!-- List the features of your application or follow the template. Don't share the figma file here :) -->

This application/site was created as a submission to a [DevChallenges](https://devchallenges.io/challenges) challenge. The [challenge](https://devchallenges.io/challenges/O2iGT9yBd6xZBrOcVirx) was to build an application to complete the given user stories.

## How To Use

<!-- Example: -->

To clone and run this application, you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
$ git clone https://github.com/your-user-name/your-project-name

# Install dependencies
$ npm install

# Run the app
$ npm start
```

## Acknowledgements

<!-- This section should list any articles or add-ons/plugins that helps you to complete the project. This is optional but it will help you in the future. For example -->

- [Steps to replicate a design with only HTML and CSS](https://devchallenges-blogs.web.app/how-to-replicate-design/)
- [Node.js](https://nodejs.org/)
- [Marked - a markdown parser](https://github.com/chjj/marked)
- [Multer](https://www.npmjs.com/package/multer)
- [react-dropzone](https://react-dropzone.js.org)
- [react-copy-to-clipboard](https://www.npmjs.com/package/react-copy-to-clipboard)
- [Axios](https://axios-http.com/)

## Contact

- Linkedin [@thomas-sentre](https://www.linkedin.com/in/thomas-sentre-20035b1b7)
- Email[@info3thomas](info3thomas@gmail.com)
- Quora [@Thomas-Sentre](https://fr.quora.com/profile/Thomas-Sentre)
- GitHub [@Thomas-Max99](https://github.com/Thomas-Max99)
- Twitter [@info3thomas](https://twitter.com/info3thomas)

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/multer-mern-image-uploader.git
git push -u origin main
```

## Heroku

```java
heroku create multer-mern-image-uploader
```

## Heroku MongoDB Environment Variables

```java
heroku config:set


heroku config:set MONGODB_URI="mongodb+srv://<userid>:<password>@cluster0.zadqe.mongodb.net/multer-mern-image-uploader?retryWrites=true&w=majority"
heroku config:set PASSWORD="something-secret"

heroku config:set PUBLIC_URL="https://multer-mern-image-uploader.herokuapp.com"
```

## Push to Heroku

```java
git push heroku

# or

npm run deploy
```

### Heroku Buildpack

See this repo for more info about setting up a node/react app on heroku:

https://github.com/mars/heroku-cra-node

```java
heroku buildpacks

heroku buildpacks --help

heroku buildpacks:clear

```

```java
heroku buildpacks
```

Output:

```java
=== multer-mern-image-uploader Buildpack URL
heroku/nodejs
```

### Notice we are doing a SET and then and ADD

```java
heroku buildpacks:set heroku/nodejs

heroku buildpacks:add mars/create-react-app
```

Output:

```java
Buildpack added. Next release on multer-mern-image-uploader will use:
  1. heroku/nodejs
  2. mars/create-react-app
Run git push heroku main to create a new release using these buildpacks.
```

### Lets try reversing the order

```java
heroku buildpacks:set mars/create-react-app

heroku buildpacks:add heroku/nodejs
```

```java
heroku buildpacks
```

Output:

```java
=== multer-mern-image-uploader Buildpack URL
heroku/nodejs
```

### Push to Heroku

```
git push heroku
```

## Error:

```java
2022-04-09T03:12:56.076028+00:00 app[web.1]: ls: cannot access '/app/build/static/js/*.js': No such file or directory
2022-04-09T03:12:56.076252+00:00 app[web.1]: Error injecting runtime env: bundle not found '/app/build/static/js/*.js'. See: https://github.com/mars/create-react-app-buildpack/blob/master/README.md#user-content-custom-bundle-location
2022-04-09T03:12:56.253505+00:00 app[web.1]: Starting log redirection...
2022-04-09T03:12:56.253698+00:00 app[web.1]: Starting nginx...
```

Attempted this:

```java
heroku config:set JS_RUNTIME_TARGET_BUNDLE=./client/build/static/js/*.js

heroku config:set JS_RUNTIME_TARGET_BUNDLE=/build/static/js/*.js

# and to remote it:

heroku config:unset JS_RUNTIME_TARGET_BUNDLE

```

## update npm packages

```java
npm install -g npm-check-updates
```

Output:

```java
removed 3 packages, changed 263 packages, and audited 264 packages in 10s

29 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
```

```java
ncu -u
```

Output:

```java
Upgrading /mnt/volume_nyc1_01/multer-mern-image-uploader/package.json
[====================] 15/15 100%

 axios                ^0.21.0  →  ^0.26.1
 bcrypt                ^5.0.0  →   ^5.0.1
 body-parser          ^1.19.0  →  ^1.20.0
 cookie-parser         ^1.4.5  →   ^1.4.6
 dotenv                ^8.2.0  →  ^16.0.0
 express              ^4.17.1  →  ^4.17.3
 express-fileupload    ^1.2.0  →   ^1.3.1
 js-cookie             ^2.2.1  →   ^3.0.1
 mongoose            ^5.10.13  →  ^6.2.10
 nodemon               ^2.0.6  →  ^2.0.15
 reactjs-popup         ^2.0.4  →   ^2.0.5
 validator           ^13.1.17  →  ^13.7.0

Run npm install to install new versions.
```

```java
npm install
```

Output:

```java
added 58 packages, removed 42 packages, changed 89 packages, and audited 299 packages in 7s

32 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
```

## Client directory

```java
cd client

ncu -u
```

```java
Upgrading /mnt/volume_nyc1_01/multer-mern-image-uploader/client/package.json
[====================] 18/18 100%

 @testing-library/jest-dom     ^5.11.4  →  ^5.16.4
 @testing-library/react        ^11.1.0  →  ^13.0.0
 @testing-library/user-event  ^12.1.10  →  ^14.0.4
 axios                         ^0.21.0  →  ^0.26.1
 dotenv                         ^8.2.0  →  ^16.0.0
 js-cookie                      ^2.2.1  →   ^3.0.1
 node-sass                     ^4.14.1  →   ^7.0.1
 react                         ^17.0.1  →  ^18.0.0
 react-dom                     ^17.0.1  →  ^18.0.0
 react-redux                    ^7.2.2  →   ^7.2.8
 react-router-dom               ^5.2.0  →   ^6.3.0
 react-scripts                   4.0.0  →    5.0.0
 reactjs-popup                  ^2.0.4  →   ^2.0.5
 redux                          ^4.0.5  →   ^4.1.2
 redux-thunk                    ^2.3.0  →   ^2.4.1
 web-vitals                     ^0.2.4  →   ^2.1.4

Run npm install to install new versions.
```
