## Required Parameters
- runId

## Response
```
game
    #Game#
category
    #Category#
?level
    #Level#
?platform
    #Platform#
players[]
    #Player#
region
    #Region#
run
    id: str
    gameId: str
    levelId: str
    categoryId: str
    ?time: int|float
    ?timeWithLoads: int|float
    ?(another for IGT?) : int
    ?enforceMs: bool
    platformId: str
    emulator: bool
    regionId: str
    video: str
    comment: ?str
    submittedById: str
    verified: int
    ?verifiedById: str
    ?reason: str
    date: int
    dateSubmitted: int
    dateVerified: int
    hasSplits: bool
    obsolete: bool
    place: int
    issues: ?
    playerIds[str]
    valueIds[str]
users[] (players and/or submitter and/or verifier)
    #User#
values[]
    #Value#
variables[]
    #Variable#
```