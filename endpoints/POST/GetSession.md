Unauthed requests return a reduced response with `signedIn = true`

# Response
```
session
    signedIn
    showAds
    user <OPT: if signedIn>
        #User#
    theme <Opt: if signedIn>
        #Theme#
    powerLevel
    dateFormat
    timeFormat
    timeReference
    timeUnits
    homepageStream
    disableThemes
    csrfToken
    networkToken <Opt: if signedIn>
    gameList[]
        #GameInfo#
    gameFollowerList[]
        gameId
        followerId
        pos
        accessCount
        lastAccessDate
    gameModeratorList[]
        gameId
        userId
        level
    gameRunnerList[]
        gameId
        userId
        runcount
    seriesList[] TODO
    seriesModeratorList[] TODO
    boostAvailableTokens <Opt: if signedIn>
    boostNextTokenDate
    boostNextTokenAmount
    userFollowerList[] TODO
```