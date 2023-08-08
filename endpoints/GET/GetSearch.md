## Required Parameters
- query

## Optional Parameters
- limit = 500 `max 500`
- includeGames = false
- includeNews = false
- includePages = false
- includeSeries = false
- includeUsers = false

# Response
```
gameList[]
    #GameInfo#
newsList[]
    id
    slug
    title
    summary
    body
    userId
    createDate
    updateDate
    publishDate
    publishTarget
    publishTags[str]
    coverImagePath
    commentsCount
pageList[]
    id
    slug
    title
    summary
    body
    userId
    createDate
    updateDate
    publishDate
    publishTarget
    publishTags[]
    commentsCount
seriesList[]
    id
    name
    url
    addedDate
    touchDate
    websiteUrl
    discordUrl
    runCount
    activePlayerCount
    totalPlayerCount
    officialGameCount
    staticAssets[]
        assetType
        path
userList[]
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
```