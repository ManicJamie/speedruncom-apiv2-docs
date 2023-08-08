Gets most recent runs for a game or set of games. Apparent limit of 14 days.

seriesId and gameId act like filters a la v1 api, so we can use this to find the most recent runs on the site.

# Optional Parameters
- seriesId
- gameId
- limit = 10 `max: 999 WARN: limit over max defaults back to 10`

# Response
```
categories[]
    id
    name
    url
    pos
    gameId
    isMisc
    isPerLevel
    numPlayers
    exactPlayers
    playerMatchMode
    timeDirection
    enforceMs
    archived
    rules
games[]
    #GameInfo#
levels[]
    id
    gameId
    name
    url
    pos
    archived
platforms[]
    id
    name
    url
    year
players[]
    id
    name
    url
    powerLevel
    color1Id
    color2Id
    colorAnimate
    areaId
regions[]
runs[]
    id
    gameId
    categoryId
    time
    timeWithLoads
    platformId
    emulator
    video
    comment
    submittedById
    verified
    verifiedById
    date
    dateSubmitted
    dateVerified
    hasSplits
    issues
    playerIds[str]
    valueIds[str]
values[]
    id
    name
    url
    pos
    variableId
    isMisc
    archived
values[]
    id
    name
    url
    pos
    gameId
    categoryScope
    categoryId
    levelScope
    levelId
    isMandatory
    isSubcategory
    isUserDefined
    isObsoleting
    defaultValue
    archived
```