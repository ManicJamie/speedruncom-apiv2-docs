Gets games moderated by this user

# Optional Parameters
- includeAll - boolean - when logged in as an Admin, this will return all of the site's games
- includeGameUrls[] - array of game URLs, unsure as to what this does

# Response
```
games[]
    #GameInfo#
gameModerationStats[]
    gameId
    state
    count
    minDate
    maxDate
```
