Gets this user's settings. NB that while userUrl is provided to allow selecting other users, presumably only site staff can use this.

# Required Parameters
- userUrl

# Response
```
settings
    id
    name
    url
    email
    bio
    powerLevel
    areaId
    theme
    color1id
    color2id
    colorAnimate
    defaultView
    timeReference
    timeUnits
    dateFormat
    timeFormat
    iconType
    disableThemes
    emailAuthentication
    latestMaxFollowed
    latestMinFollowed
    latestTimeFollowed
    showMiscByDefault
    showOnStreamsPage
    showUnofficialGameTypes
    homepageStream
    disableMessages
    showAds
    pronouns[str]
    nameChangeDate
    runCommentsDisabled
    followedGamesDisabled
    supporterEndDate
    boostEndDate
    supporterIconType
    supporterIconPosition
    staticAssets[]
        type
        path
    staticAssetUpdates
gameFollowerList[]
    gameId
    followerId // self
    pos
    accessCount
    lastAccessDate
gameModeratorList[]
    gameId
    userId
    level
notificationSettings[]
    type
    gameId <OPTIONAL>
    site
    email
userSocialConnectionList[]
    userId
    networkId
    value
    verified
gameList[]
    #GameInfo#
themeList[]
    #Theme#
supporterCreditList[] TODO
supportCodeList[] TODO
```