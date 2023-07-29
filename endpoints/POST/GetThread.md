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
    id
    name
    url
    powerLevel
    pronouns[str]
    areaId
    color1Id
    color2Id
    iconType
    onlineDate
    signupDate
    touchDate
    staticAssets[]
        assetType
        path
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