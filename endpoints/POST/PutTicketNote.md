# Parameters
- ticketId: str
- note: str
- isMessage: Boolean

# Response
When isMessage is true:
```
ok: true
```

But when isMessage is false, it's a generic 401 unauthorized.

# Use
When isMessage is true, the admin and user can add messages to communicate in the ticket's conversation.

But when it is set to false, only admins can see their messages in the Admin Console.