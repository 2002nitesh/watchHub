# watchHub Backend 

## Introduction

This is a ``YOUTUBE + TWITTER`` backend project that covers allmost the functionalities of youtube 
and also combines the tweet functionality from twitter into it.A video streaming platform using MERN stack involves leveraging MongoDB’s aggregation pipeline for advanced data processing and user engagement features. User authentication with JWT. Find more about his project in the documentaion below.

## Features

### User Management:

- Registration, login, logout, password reset
- Profile management (avatar, cover image, details)
- Watch history tracking

### Video Management:

- Video upload and publishing
- Video search, sorting, and pagination
- Video editing and deletion
- Visibility control (publish/unpublish)

### Tweet Management:

- Tweet creation and publishing
- Viewing user tweets
- Updating and deleting tweets

### Subscription Management:

- Subscribing to channels
- Viewing subscriber and subscribed channel lists

### Playlist Management:

- Creating, updating, and deleting playlists
- Adding and removing videos from playlists
- Viewing user playlists

### Like Management:

- Liking and unliking videos, comments, and tweets
- Viewing liked videos

### Comment Management:

- Adding, updating, and deleting comments on videos

### Dashboard:

- Viewing channel statistics (views, subscribers, videos, likes)
- Accessing uploaded videos

### Health Check:

- Endpoint to verify the backend's health

## Technologies Used

- Node.js 
- Express.js
- MongoDB
- Cloudinary (must have an account)

## Api Endpoints

1. **users**
   ```bash
   /api/v1/users/logout
   ```
   ```bash
   /api/v1/users/refresh-token
   ```
   ```bash
   /api/v1/users/change-password
   ```
   ```bash
   /api/v1/users/current-user
   ```
   ```bash
   /api/v1/users/update-user
   ```
   ```bash
   /api/v1/users/update-avatar
   ```
   ```bash
   /api/v1/users/update-coverImg
   ```
   ```bash
   /api/v1/users/c/:username
   ```
   ```bash
   /api/v1/users/watch-history
   ```
   
2. **comment**
   ```bash
   /api/v1/comment/:videoId
   ```
   ```bash
   /api/v1/comment/c/:commentId
   ```
3. **likes**
   ```bash
   /api/v1/likes/toggle/v/:videoId
   ```
   ```bash
   /api/v1/likes/toggle/c/:commentId
   ```
   ```bash
   /api/v1/likes/toggle/t/:tweetId
   ```
   ```bash
   /api/v1/likes/videos
   ```
4. **subscriptions**
   ```bash
   /api/v1/subscriptions/c/:channelId
   ```
   ```bash
   /api/v1/subscriptions/u/:subscriberId
   ```
5. **tweet**
   ```bash
   /api/v1/tweet/
   ```
   ```bash
   /api/v1/tweet/user/:userId
   ```
   ```bash
   /api/v1/tweet/:tweetId
   ```
6. **video**
   ```bash
   /api/v1/video
   ```
   ```bash
   /api/v1/video/v/:videoId
   ```
   ```bash
   /api/v1/video/toggle/publish/:videoId
   ```
7. **healthcheck**
   ```bash
   /api/v1/healthcheck/
   ```
8. **playlist**
   ```bash
   /api/v1/playlist/
   ```
   ```bash
   /api/v1/playlist/:playlistId
   ```
   ```bash
   /api/v1/playlist/add/:videoId/:playlistId
   ```
   ```bash
   /api/v1/playlist/remove/:videoId/:playlistId
   ```
   ```bash
   /api/v1/playlist/user/:userId
   ```
9. **dashboard**
   ```bash
   /api/v1/dashboard/stats
   ```
   ```bash
   /api/v1/dashboard/videos
   ```

## Installation and Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/2002nitesh/watchHub.git
    ```

2. **Install dependencies:**

    ```bash
    cd server
    npm install
    ```

3. **Start the server:**

    ```bash
    npm run dev
    ```
