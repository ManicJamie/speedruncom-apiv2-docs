Get moderation data

# Required Parameters
- gameId
- limit `max: 100`
- page

# Optional Parameters
- search
- verified
- verifiedById

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
    id
    name
    url
    type
    loadtimes
    milliseconds
    igt
    verification
    autoVerify
    requireVideo
    emulator
    defaultTimer
    validTimers[]
    releaseDate
    addedDate
    touchDate
    coverPath
    trophy1stPath
    trophy2ndPath
    trophy3rdPath
    runCommentsMode
    runCount
    activePlayerCount
    totalPlayerCount
    boostReceivedCount
    boostDistinctDonorsCount
    rules
    viewPowerLevel
    platformIds[str]
    regionIds[]
    gameTypeIds[]
    websiteUrl
    discordUrl
    defaultView
    guidePermissionType
    resourcePermissionType
    staticAssets[]
        assetType
        path
levels[]
    id
    gameId
    name
    url
    pos
    rules
    archived
pagination
    count
    page
    pages
    per
platforms[]
    id: str
    name: str
    url: str
    year: int
players[]
    id: str
    name: str
    url: str
    powerLevel: int
    color1Id: str
    colorAnimate: int
    areaId: str
regions[]
    # not documented
runs[]
    id: str
    gameId: str
    levelId: Optional[str]
    categoryId: str
    time: decimal
    timeWithLoads: decimal
    platformId: str
    emulator: bool
    video: str
    comment: str
    submittedById: str
    verified: int
    date: int
    dateSubmitted: int
    hasSplits: bool
    obsolete: bool
    place: int
    estimated: bool
    issues: ? (null?)
    playerids[str]
    valueIds[str]
```