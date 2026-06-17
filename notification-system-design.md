# Stage 1: Notification System Design

## Core Actions
-Create notification
-Get notifications
-Mark as read
-Delete notifiction

## REST APIs
POST /notifications
GET/notifications/:userId
PUT/notifications/:id/read
DELETE/notifications/:id

## Sample Request
{
    "userId:"123",
    "title":"New Message",
    "message":"you have a new message"
}

## sample Response
{
    "id": "n1",
    "userId": "123",
    "title":"New message",
    "isRead":false
}

## Headers
content-Type: application/json
Authorization: Bearer token

## Real-time Notifications
Use WebSockets to send notifications instantly to users when they are online. 