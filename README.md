# project

* make directory
* npm init and enter throught the prompts or npm init -y to skips through prompts
* make entrypoint file(index.js)
* run node project (node index.js)
* npm i //name of app
* import nodule by using require('name of nodule')
* created an instance of an app
* create a .gitignore //write node_modules in the .gitignore file
* home route
    * app.get('/', (req, res)=>{
        res.send()
    })
* import ejs using npm i ejs --> tells texpress that we will use ejs as the view engine
* html files
    * app.get('/', (req, res)=>{
        res.sendFile(__dirname+'where html file is located')
    })
* templates
    * app.get('/', (req, res)=>{
        res.render('filename.ejs', {key: value})
    })
* when using ejs make sure each line starts with <% and ends with %>
* partials
    * <%- include('../partials/filename.ejs') %>
* layouts
    * npm i express-ejs-layouts
    * require
    * app.set('view engine',)
    * app.use(ejslayouts)
    * make html boilerplate and insert <%- body %> in the body
* axios
* run node by typing nodemon in terminal

* sequelize
    * npm i pg sequelize
    * const db = require('./models')
    * db.user.create({}).then()
    * db.user.findAll().then()
    * db.user.findOne({where:{}}).then()
    * db.user.findOrCreate({where:{}, defaults}).then()
    * db.user.update({}).then(numRowsChanged=>{console.log(numRowsChanged)})
    * db.user.destroy({}).then(numRowsDeleted=>{console.log(numRowsDeleted)})