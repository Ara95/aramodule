# Aramodule

## Install command:
npm install aramodule2 --save

connecting and using mongodb

### Setup
const dsn = "mongodb://localhost:27017/test";
const db  = require('aramodule').mongoInit(dsn, 'test');


### Get data

const data = await db.get();

### Insert data

var ob = {
    username: "ara",
    password: "password"
};

await db.insert(ob);


### Reset data

await db.reset();
