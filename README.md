# AIP-assignment2

> I OWE U

This is a favor tracker application from Advanced Internet Programming subject at UTS. It is a tracking system that intends to keep track of small favors amongst friends or groups.

## Technology Stack 

This is a PERN stack application. PERN stands for:

1. PostgreSQL
2. Express
3. React
4. Nodejs

## Developer Info

### Authors

1. Yoo Jin Chang
2. Mercedes Speroni
3. Saurabh Kumar
4. Renato Tranchesi

---

# Quick Start 🚀

## Installation ⚙️

### Install server dependencies

```bash
cd server
npm install
```

### Install client dependencies

```bash
cd client
npm install
```

## Database Setup 🛠

### Install Postgres
1. For Ubuntu or Window
```bash
apt install postgresql
```

2. For mac
```bash
brew install postgresql
```

### Prepare sample data

```bash
cd /server/sql
npm run initdb
npm run drop
npm run schema
npm run sample_data
```

## Run server 🏁

### Run Express

```bash
cd server
npm run server
```

### Run React

```bash
cd client
npm start
```

## Deployment 🌏

### Build for deployment

```bash
cd client
npm run build
```

### Deploy to AWS
After running the build from client, you need to uncomment codes for deployemnt in `/server/server.js` and `/server/config/db.js`

---

# Folder structure 📁

## Server-side (Back-end)
    server
    ├── api                   # Core application with API 
    ├── config                # Configuration file for database
    ├── middleware            # Middleware for authentication
    ├── sql                   # Storage and retrieval for sample data
    ├── utils                 # Utility for unicode validation
    ├── server.js             # Top-level module
    └── package.json

> Server-side consists of Persistence layer, Domain layer, and API layer

## Client-side (Front-end)
    client
    ├── public                  
    ├── src                
    │    ├── actions            # Communication with the API
    │    ├── components         # User interface
    │    ├── image              # Storage of images for landing page & profile
    │    ├── App.css        
    │    ├── App.js             # Top-level module
    │    └── index.js
    └── package.json

> Client-side consists of Presentation layer and API client layer

---

# Innovation and Inventiveness 💡

We have used [Nginx](https://docs.nginx.com/nginx/admin-guide/load-balancer/http-load-balancer/) and [pm2](https://pm2.io/docs/runtime/guide/load-balancing/) for load balancing.

The configuration file and steps to set them are documented in `/deployment/default.conf` and `/deployment/nginx_setup.sh`.



