Get support hub tickets.

# Parameters (select one?)
- queues = []
- requestorIds = [str] - appears to be necessary?
- statuses = []
- ticketIds = [str] - retrieve a specific (set of) ticket(s)
- types = []

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