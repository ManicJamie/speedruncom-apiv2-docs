Gets a thread page. 20 comments per page.

WARNING: This endpoint's pagination 404s if you request a page that doesn't exist, rather than just going to maxpage like all other paginated objects!

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