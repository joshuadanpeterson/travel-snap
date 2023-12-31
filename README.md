# TravelSnap: Travel Photography Sharing Platform

## Overview

TravelSnap is a Node.js and Express-powered web platform for travel enthusiasts to share, explore, and discuss stunning travel photographs, leveraging MongoDB for data storage and Google Cloud Storage for photo management.

## Technical Stack

- **Backend**: Node.js with Express
- **Database**: MongoDB
- **File Storage**: Google Cloud Storage (for photo storage)
- **Frontend**: (To be decided, e.g., React)

## Getting Started

Follow these steps to get your development environment set up:

1. Clone the repo: `git clone [repository-url]`
2. Navigate to the project directory: `cd TravelSnap`
3. Install dependencies: `npm install`
4. Set up your environment variables for database connection and Google Cloud Storage.
5. Start the server: `npm start`

## Routers and Endpoints

### User Router (`/users`)

Handles user-related operations.

- **GET** `/users`: Retrieve all users.
- **POST** `/users`: Create a new user.
- **PUT** `/users/:userId`: Update a user's information.
- **DELETE** `/users/:userId`: Delete a user.

### Photo Router (`/photos`)

Manages photo uploads and information.

- **GET** `/photos`: Retrieve all photos.
- **GET** `/photos/:photoId`: Retrieve a specific photo.
- **POST** `/photos`: Upload a new photo.
- **PUT** `/photos/:photoId`: Update photo details.
- **DELETE** `/photos/:photoId`: Delete a photo.

### Comments Router (`/comments`)

Facilitates commenting on photos.

- **GET** `/photos/:photoId/comments`: Retrieve comments for a photo.
- **POST** `/photos/:photoId/comments`: Post a comment on a photo.
- **DELETE** `/photos/:photoId/comments/:commentId`: Delete a comment.

### Authentication Router (`/auth`)

Handles user authentication.

- **POST** `/auth/login`: User login.
- **GET** `/auth/logout`: User logout.

## Project Setup

- **Subfolder**: `TravelSnap` in `5-NodeJS-Express-MongoDB`.
- **Git Repository**: Initialized with `.gitignore` for `node_modules`.
- **Dependencies**: Express, body-parser, and morgan.
- **Routes**: Implemented in the `routes` subfolder.

## Data Storage

- **Photo Metadata**: Stored in MongoDB.
- **Photo Files**: Stored in Google Cloud Storage.

## Author

- **Joshua Peterson** - *Initial work* - [joshuadanpeterson](https://github.com/joshuadanpeterson)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details

## Acknowledgments

