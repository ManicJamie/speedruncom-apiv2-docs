Gets conversations belonging to authed user.

# Response
```
conversations[]
    id
    participantUserIds[]
    lastMessageId
    lastMessageUser
    lastMessageText
    lastMessageDate
    readDate
participants[]
    conversationId
    userId
    joinedDate
    leftDate
users[]
    #User#
```