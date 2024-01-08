# Parameters
- runId

# Response
```
settings
    runId: str
    gameId: str
    categoryId: str
    playerNames[str]
    ?time
        hour: int
        minute: int
        second: int
        millisecond: int
    ?timeWithloads
        hour: int
        minute: int
        second: int
        millisecond: int
    ?igt
        hour: int
        minute: int
        second: int
        millisecond: int
    platformId: str
    emulator: bool
    video: str
    comment: str
    date: int
    values[]
        variableId: str
        valueId: str
users[]
    #User#
```