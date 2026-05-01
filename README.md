# Applied JS Projects

This repository contains multiple JavaScript projects ranging from small browser apps to React and full-stack applications.

## Projects

| Project | Type | Summary |
| --- | --- | --- |
| `alarm-clock` | Vanilla JavaScript | Browser-based alarm clock with time selectors and ringtone support. |
| `notes` | Vanilla JavaScript | Notes/task app that stores data in local storage with add, edit, and delete actions. |
| `textutils` | React | Text utility app with routing, alerts, and light/dark mode support. |
| `noteswift` | React + Node.js + MongoDB | Full-stack notes app with authentication and note management. Includes a `backend/` folder inside the project. |
| `noteswift-backend` | Node.js + Express + MongoDB | Standalone backend for the NoteSwift project. Exposes `/api/auth` and `/api/notes`. |

## Folder Structure

```text
applied-js-project/
├── alarm-clock/
├── notes/
├── noteswift/
│   ├── src/
│   ├── public/
│   └── backend/
├── noteswift-backend/
└── textutils/
```

## How To Run

### 1. `alarm-clock`

This is a static frontend project.

1. Open `alarm-clock/index.html` in a browser.

### 2. `notes`

This is a static frontend project that uses browser local storage.

1. Open `notes/index.html` in a browser.

### 3. `textutils`

This is a Create React App project.

1. Open a terminal in `textutils/`
2. Run `npm install`
3. Run `npm start`
4. Visit `http://localhost:3000`

Useful scripts:

- `npm start`
- `npm test`
- `npm run build`
- `npm run deploy`

### 4. `noteswift`

This project contains a React frontend and a backend folder.

Frontend:

1. Open a terminal in `noteswift/`
2. Run `npm install`
3. Run `npm start`

Backend inside `noteswift/backend`:

1. Open a second terminal in `noteswift/backend/`
2. Run `npm install`
3. Start the API with `node index.js`

There is also a root script in `noteswift/package.json`:

- `npm run both` to start the frontend and backend together if `nodemon` is available

Environment note:

- The frontend reads `REACT_APP_HOST`
- The backend connects to MongoDB, so a valid database connection is required

### 5. `noteswift-backend`

This is a standalone Express backend for NoteSwift.

1. Open a terminal in `noteswift-backend/`
2. Run `npm install`
3. Start the server with `node index.js`

Default API port:

- `http://localhost:5000`

## Tech Stack

- Vanilla JavaScript, HTML, CSS
- React
- React Router
- Node.js
- Express
- MongoDB with Mongoose

## Notes

- `noteswift` already contains its own backend under `noteswift/backend/`
- `noteswift-backend` appears to be a separate copy of the backend with `nodemon` listed in `devDependencies`
- `textutils` includes GitHub Pages deployment support through `gh-pages`
