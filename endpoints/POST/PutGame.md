Creates a game (available to series supermods for games within a series)

# Parameters
- name: str
- releaseDate: int
- gameTypeIds[] (usually empty)
- seriedId: str

# Response
```
game
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
    validTimers[int]
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
    regionIds[str]
    gameTypeIds[int]
    websiteUrl
    discordUrl
    defaultView
    guidePermissionType
    resourcePermissionType
    staticAssets[]
        assetType
        path
```