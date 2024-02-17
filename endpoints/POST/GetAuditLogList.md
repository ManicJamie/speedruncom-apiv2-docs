# Parameters
- gameId OR seriesId OR userId OR actorId
- eventType = #eventType#
- page

# Response
```
auditLogList[]
    id
    date
    eventType
    actorId
    gameId
    context
```

# Use
actorId is admin only. But it should be a user's id.

It shows every change that the user has made to something else.
As opposed to userId, which shows every change that has happened to that user.