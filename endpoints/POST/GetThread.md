Gets a thread page. 20 comments per page.

# Parameters
- id
- page `Optional`

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
userList[]
    #User#
likeList[]
    itemType
    itemId
    userId
    date
pagination
    count
    page
    pages
    per
```