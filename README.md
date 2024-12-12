# 0x04. Files manager

This repository contains a file manager application built with Node.js. The application allows users to upload, manage, and share files efficiently. Below is an overview of the project structure and functionalities.

## Table of Contents

- [Project Overview](#project-overview)
- [File Structure](#file-structure)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Endpoints](#endpoints)
- [Testing](#testing)

## Project Overview

The file manager application provides various functionalities for users to manage their files:

- Upload files
- View file details
- Publish/unpublish files
- Generate thumbnails for images
- Send welcome emails to new users

The application utilizes Express.js for handling HTTP requests, MongoDB for database storage, and Redis for caching. Background processing for tasks such as thumbnail generation and sending emails is implemented using Bull queues.

## File Structure

```
project-root/
│
├── controllers/
│   ├── AppController.js
│   ├── AuthController.js
|   ├── UsersController.js
|   ├── FilesController.js     
│   └── ...
│
├── routes/
│   ├── index.js
│   └── ...
│
├── tests/ 
│   ├── dbClient.test.js
│   ├── redisClient.test.js
│   ├── status.test.js
│   ├── stats.test.js
│   ├── users.test.js
│   └── ...
│
├── utils/
│   ├── db.js
│   ├── redis.js
│   └── ...
│
├── package.json
├── server.js
├── worker.js
├── .env
└── README.md
```
