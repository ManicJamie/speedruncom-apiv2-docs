Unauthed requests return a reduced response with `signedIn = true`

# Response
```
session
    signedIn
    showAds
    user <OPT: if signedIn>
        id
        name
        url
        powerLevel
        pronouns[str]
        areaId
        color1Id
        color2Id
        iconType
        onlineDate
        signupDate
        touchDate
        staticAssets[]
            assetType
            path
    theme <Opt: if signedIn>
        id
        url
        primaryColor
        panelColor
        panelOpacity
        navbarColor
        backgroundColor
        backgroundFit
        backgroundPosition
        backgroundRepeat
        backgroundScrolling
        foregroundFit
        foregrountPosition
        foregroundRepeat
        foregroundScrolling
        touchDate
        staticAssets[]
            assetType
            path
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