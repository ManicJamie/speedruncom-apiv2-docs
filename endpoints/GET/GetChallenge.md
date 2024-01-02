## Parameters
- id

# Response
```
challenge
    id
    name
    url
    gameId
    createDate
    updateDate
    startDate
    endDate
    state: enum
    description
    rules
    numPlayers
    exactPlayers
    playerMatchMode: enum?
    timeDirection
    enforceMs
    coverImagePath
    contest: bool
    contestRules: str
    runCommentsMode: enum
    prizeConfig
        prizepool: int, maybe float
        currency: str
        prizes[]
            place: int
            amount: int, maybe float
game
    #Game#
moderatorList[]
    challengeId
    userId
    level
standingList[]
    place
    registeredPlayerIds[str]
    
```