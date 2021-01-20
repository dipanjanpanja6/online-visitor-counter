# Live online visitor counter

server less real-time online visitors counter with firebase Realtime database

you can implement in any javascript based frontend/html/react js/angular js

just replace the config object with your own
 
 ### HTML
 
Real-time online visitors counter using firebase realtime database

1. create firebase project https://firebase.google.com/docs/web/setup
2. goto firebase realtime database and create a new one.
3. navigate to rules tab and add rules like this.
```javascript
{
  "rules": {
    ".read": false,
    ".write": false,
      "tempUser":{
        ".read":true,
         ".write":true,
         ".indexOn":"state"
      }
  }
}
```
3. now goto html/index.html
4. replace firebaseConfig with your own
```javascript
var firebaseConfig = {
  apiKey: "API_KEY",
  authDomain: "PROJECT_ID.firebaseapp.com",
  databaseURL: "https://PROJECT_ID.firebaseio.com",
  projectId: "PROJECT_ID",
  storageBucket: "PROJECT_ID.appspot.com",
  messagingSenderId: "SENDER_ID",
  appId: "APP_ID",
  measurementId: "G-MEASUREMENT_ID",
};
```
4. run index.html

### React JS

1. run ```npm i```
2. open config.js file
3. replace firebaseConfig with your own
```javascript
var firebaseConfig = {
  apiKey: "API_KEY",
  authDomain: "PROJECT_ID.firebaseapp.com",
  databaseURL: "https://PROJECT_ID.firebaseio.com",
  projectId: "PROJECT_ID",
  storageBucket: "PROJECT_ID.appspot.com",
  messagingSenderId: "SENDER_ID",
  appId: "APP_ID",
  measurementId: "G-MEASUREMENT_ID",
};
```
4. run ```npm start```
