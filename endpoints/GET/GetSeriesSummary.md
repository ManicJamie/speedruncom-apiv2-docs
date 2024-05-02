Gets a summary for a series

# Required Parameters:
- seriesId OR
- seriesUrl

# Response:
```
series: Series
forum: Forum
gameList[]:
    #Game#
moderatorList[]:
    seriesId
    userId
    level
theme:
    #Theme#
threadList[]
    #Thread#
userList[]:
    #User#
gameCount: int
streamCount: int
threadCount: int
```