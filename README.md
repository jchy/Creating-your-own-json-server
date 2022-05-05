# Json-server
Creating json-server from scratch

### step.1 Initialize the project 
```
  npm init -y
```
### step.2 Install json-server using the following command 
```
  npm install json-server
```
### step.3 create a json file named db.json in the same directory of the project using  
```
  touch db.json
```
### step.4 Insert the data into the json file whatever you want like and save it
```
  {
  "data": [
    {
      "name": "anc",
      "branch": "cse"
    },
    {
      "name": "xyz",
      "branch": "cse"
    },
    {
      "name": "yyz",
      "branch": "cse"
    }
  ]
}
```
### step.5 Go into the package.json file and write the following line of the code in the scripts object :   
```
  "start" : "json-server --watch db.json"
```
NOTE : After adding above lne of code your package.json will look like this
```
   {
      "name": "test",
      "version": "1.0.0",
      "description": "",
      "main": "index.js",
      "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1",
        "start" : "json-server --watch db.json"
      },
      "keywords": [],
      "author": "",
      "license": "ISC",
      "dependencies": {
        "json-server": "^0.17.0"
      }
   }
```
### step.6. To get the data into your favourite browser run the following code into the terminal
```
  npm start
```
### step.7. This step above will output a localhost link in terminal open the same in the browser of your choice, It will look like this
```
  http://localhost:3000/data
```
### step.8. To post the data into db.json open the postman and use the POST method and write the data and post it like (Make sure you must provide the id)
```
  {
    "id":8,
    "name": "amit",
    "age":18,
    "branch": "cse"
  }
```

