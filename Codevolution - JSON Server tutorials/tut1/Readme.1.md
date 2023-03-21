# step 0 -
[youtube](https://www.youtube.com/watch?v=_1kNqAybxW0&list=PLC3y8-rFHvwhc9YZIdqNL5sWeTCGxF4ya)
## create db.json file
## import json-server module
[doc](https://github.com/typicode/json-server)

```.sh
npm install -g json-server
```
-g for global install

## Start JSON Server to test

```.sh
json-server --watch db.json
```
not: db.json file in oldugu path e olmak gerek.


# step1 - create package.json file

```.sh
npm init -y
```

## be sure you have yarn

```.sh
npm install -g yarn
```
## add json-server to dependencies

```.sh
yarn add json-server
```

## add serve-json
```.sh
 "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "serve-json": "json-server -- watch db.json"
  },
```

## test the app

```.sh
yarn serve-json
```
