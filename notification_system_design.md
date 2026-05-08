end point{
POST /api/v1/notifications
}
request header
{
  "Authorization": "Bearer <jwt_token>",
  "Content-Type": "application/json"
}
request body
{
  "userId": "USR_102",
  "title": "Assignment Deadline",
  "message": "Your assignment submission closes tomorrow.",
  "type": "academic",
  "priority": "high"
}
response{
{
  "success": true,
  "message": "Notification created successfully",
  "data": {
    "notificationId": "NTF_901",
    "createdAt": "2026-05-08T10:20:00Z"
  }
}
endpoint{
GET /api/v1/notifications
}
