# microfrontends

This was a side project to help me learn how to build apps using microfrontends (microservice architecture for frontend). 

## Tech stack
React    
Vue    
Webpack    
React Router   
Material UI   
AWS   
Github Actions    

## Brief overview

packages > container    
Host app (React.js)

packages > auth     
Child app (React.js)

packages > marketing    
Child app (React.js)

packages > dashboard    
Child app (Vue.js)
- The reason this app was written in Vue was to see how to coordinate microfrontends that are using different FE frameworks.

Custom webpack configurations setting up module federation are in `config` folder in each app.
Apps are deployed to an S3 bucket in AWS. Each child app can also run in isolation.

## How to run locally

cd into each child app    
`npm i`     
`npm start`    

cd into container    
`npm i`    
`npm start`    

No env variables.
