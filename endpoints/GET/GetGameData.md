## Required Parameters
- gameId OR
- gameUrl

Also works as POST!

## Response
```
game
    id: str
    name: str
    url: str
    type: str
    loadtimes: bool
    milliseconds: bool
    igt: bool
    verification: bool
    autoVerify: bool
    requireVideo: bool
    emulator: int(enum)
    defaultTimer: int(enum)
    validTimers[int (enum)]
    releaseDate: int
categories[]
    #Category#
levels[]
    #Level#
moderators[]
    gameId
    userId
    level
platforms[]
    #Platform#
regions[]
    #Region#
runCounts[]
    gameId
    categoryId
    variableId
    valueId
    count
theme
    #Theme#
users[] (just those relevant to the game information)
    #User#
values[]
    #Value#
variables[]
    #Variable#
```