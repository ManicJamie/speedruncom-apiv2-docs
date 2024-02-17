Get support hub tickets.

# Parameters (select one?)
- queues = []
- requestorIds = [str] - with this empty, it returns all tickets. Only admins have access, since this is used on their admin console
- statuses = []
- ticketIds = [str] - retrieve a specific (set of) ticket(s)
- types = []
- page = int - pagination for the admin console
- limit = int - pagination for the admin console

- page

# Response
```
ticketList[]
    id
    queue
    type
    status
    requestorId
    dateSubmitted
    metadata = str (json structure may be per-type)
ticketNoteList[]
    id
    ticketId
    readerId
    dateSubmitted
    note
    isMessage
    isRead
pagination
    count
    page = 1
    pages
    per = 500
userList
    #User#
gameList[]
    #Game#
```