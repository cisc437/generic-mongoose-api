# generic-mongoose-api
A completely generic single-file mongo-backed API in Node using Mongoose.  This code can work out of the box on c9.io, for other servers adapt as needed.

## SETUP

 + git clone https://github.com/cisc437/generic-mongoose-api.git
 + cd generic-mongoose-api/
 + npm install
 + mongod --smallfiles --syslog --fork
 + npm start

## USAGE of the API:

 + GET /:collection returns a list of all documents in the requested collection
 + GET /:collection/:id returns the single document with the requested id
 + POST /:collection takes in JSON (Content-Type: application/json) and creates a new document in requested collection
 + PUT /:collection/:id merges the matching document with the JSON you pass in
 + DELETE /:collection/:id deletes the requested document
