# Nodejs-mysql

NodeJs for API api and AngularJs for CRUD with pagination and filters.
Project use Sequelize with supports for MySQL.
For testing, copy repository:
```
git clone https://github.com/raylight75/NodejsCRUD
```
Install dependecies:
```
npm install
```

Import products.sql.

Configure Sequelize database:
```
var sequelize = new Sequelize('api', 'name', 'password', {
    define: {
        timestamps: false//true for enable
    },
    host: 'localhost',
    dialect: 'mysql',
    pool: {
        max: 5,
        min: 0,
        idle: 10000
    },
});
```
Root project:
```
node bin/www
```
Starting App
```
START APP type: nodemon or nodemon app.js in App directory.
```
        - type: node app.js in App directory.
```
       or type: node server.js for basic http request.
```

Access of API:
[localhost:3000](http://localhost:3000)

Routes:
```
GET /articles -> get articles
POST /articles -> update articles

GET /articles/:id -> get articles by id
PUT /articles/:id -> update articles by id
DELETE /articles/:id ->delete articles
```
