# Parameters
- conversationId
- markAsRead `Opt`

# Response
```
conversation
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
messages[]
    id
    conversationId
    userId
    text
    date
users[]
    #User#
userBlocks[]
```