# MongoDB Cheetsheet
## Commands
* mongod - start server
* mongo - repl for mongo
* help - help to get help
* show dbs - show database
* use - use database
* insert - insert into table
* find - find by search criteria
* update - update entry
* remove - remove entry

## start database
In terminal type below:

`mongod`
## database console
New terminal make sure you have two terminals 

`mongo`
## show databases
`show dbs`
## select database
`use databasename`
## show what database your in
`db`
## To see tables
`show collections`


# Example:
```js
// shows databases
show dbs
// select database
use databasename
// insert
db.database.insert({name: 'Richard'})
// find by object
db.databasename.find({name: 'Richard'})
// update with not perserving other properties
db.databasename.update({name: 'Richard'}, {name: 'Peter'})
// updating with preserving properties and adding new property
db.databasename.update({name: 'Peter'}, {$set: {name: 'Tater', newProperty: true}})
// delete by search criteria
db.databasename.remove({name: 'Richard'})
// limit for how many to remove
db.databasename.remove({type: 'category'}).limit(1)
```
