Note that information from this request is a subset of `GetCommentList`.

# Parameters
- itemId
- itemType

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
        canViewComments
        canPostComments
        canEditComments
        canDeleteComments
        cannotViewReasons[str]
        cannotPostReasns[str]
```