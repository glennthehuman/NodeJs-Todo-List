## Todo List.

Build a todo list with NodeJs, VueJs & MonogDB

**Run**

```
npm install

```

**Backend API**

Start mongodb. Usually, like this

```
mongod
```

**Build**

```
npm run build

```

**Running the App**

To start the application, navigate to project root where server.js file is located and run 
```
node server.js
```

Sample API requests:

create a new todo item
```
$ curl -H "Content-Type: application/json" -X POST -d "{\"name\":\"Going Shopping\"}" http://localhost:4000/api/add

{"__v":0,"name":"Going Shopping","done":false,"_id":"5a6365a39a2e56bc54000003"}
```

Get all todo items
```
$ curl  http://localhost:4000/api/all

[{"_id":"5a6365a39a2e56bc54000003","name":"Doing Laundry","done":false,"__v":0},{"_id":"5a6366039a2e56bc54000004","name":"Going Shopping","done":false,"__v":0}]
```

For the frontend, navigate to http://localhost:4000
