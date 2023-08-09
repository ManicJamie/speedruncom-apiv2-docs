# Parameters
- itemId
- itemType
- page = 1

# Response
```
commentable
    itemType
    itemId
    properties
        disabled
        locked
    permissions
        canManage
        canViewcomments
        canPostComments
        canEditComments
        canDeleteComments
        cannotViewReasons[str]
        cannotPostReasons[str]
commentList[]
    id
    itemType
    itemId
    date
    userId
    text
    parentId
    deleted
likeList[]
    itemType
    itemId
    userId
    date
userList[]
    #User#
pagination
    count
    page
    pages
    per
```