# react-native-web-express-starter


## 1 | Getting Started


### 1.1 Installing

1. Clone project

2. Install dependencies in both `./frontend` and `./backend`

```
yarn || npm install
```

### 1.2 Running

Run the backend first, then the frontend.

In `./backend`:

```
npm run start || yarn start || exp start
```


In `./frontend`:

```
npm run start || yarn start || exp start
```

Runs the app on mobile.


```
npm run web || yarn web
```

Runs the app on browser.

```
npm run desktop || yarn desktop
```

Runs the app as a desktop app.


## 2 | Structure

### 2.1 Ports

The back-end will be running in localhost:3001, while the front-end runs in
localhost:3000 for web and desktop, and localhost:19000 for mobile.

### 2.2 Requesting Data

To run the app on Expo for mobile, no proxy is used. Instead, the port is
written in the `fetch` requests

```
fetch('http://localhost:3001/users')
```

### 2.3 Backend

Backend data is found in `.backend/routes/`. To add a new page, configure it
in `.backend/app.js`.


### 2.4 Desktop App functionality

Electron is set for development, but not for production. 
