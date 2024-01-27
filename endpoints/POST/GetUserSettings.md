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
supporterCreditList[]
    id: str
    userId: str
    providerId: int enum
    createdAt: int
    updatedAt: int
    creditType: int
    amount: int (cents?)
    currency: str (eg "usd")
    receivedAt: int
    subscriptionId: str
    periodStartsAt: int
    periodEndsAt: int
    providerItemId: str
supportCodeList[]
    id: str
    code: str
    description: str
    duration: int
    userId: str
    createdAt: int
    updatedAt: int
?supporterSubscription
    id: str
    userId: str
    providerId: int enum
    createdAt: int
    updatedAt: int
    expiresAt: int,
    planId: int enum,
    nextPeriodPlanId: int enum,
    status: int enum,
    trialEndsAt: int date (0 otherwise),
    cancelAtPeriodEnd: bool,
    canceledAt: int date (0 otherwise),
    cardBrand: str ("visa" etc),
    cardLast4: str ("1234),
    providerItemId: str,
    isActive: bool,
    isExpired: bool,
    isOngoing: bool,
    isTrialing: bool
```