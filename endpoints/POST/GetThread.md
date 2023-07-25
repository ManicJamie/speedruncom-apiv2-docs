Gets a thread page

# Parameters
- id
- page

# Response
```
thread
    id
    name
    gameId
    forumId
    userId
    replies
    created
    lastCommentId
    lastCommentUserId
    lastCommentDate
    sticky
    locked
commentList[]
    id
    itemType
    itemId
    date
    userId
    text
    parentId
    deleted
```