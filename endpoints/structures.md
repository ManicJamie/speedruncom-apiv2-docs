# Data structures

Commonly seen data structures will be placed here for easier reference. Names are made up.

Attributes labeled with #Type# are documented here.

# Asset
Seen in most structures, as it contains image refs for basically everything.
```
assetType: str
path: str
```

## GameInfo
GetSearch, GetLatestLeaderboard, GetForumList, GetGameSettings, GetModerationGames, GetModerationRuns, GetSeriesSettings, GetSession, GetUserSettings, PutGame, GetTickets
```
id: str
name: str
url: str
type: str (enum)
loadtimes: bool
milliseconds: bool
igt: bool
verification: bool
autoVerify: bool
requireVideo: bool
emulator: int (enum)
defaultTimer: int (enum)
validTimers[int (enum)]
releaseDate: int
addedDate: int
touchDate: int
coverPath: str
trophy1stPath: str
trophy2ndPath: str
trophy3rdPath: str
runCommentsMode: int (enum?)
runCount: int
activePlayerCount: int
totalPlayerCount: int
boostReceivedCount: int
boostDistinctDonorsCount: int
rules: str
viewPowerLevel: int (enum)
platformIds[str]
regionIds[str]
gameTypeIds[int]
websiteUrl: str
discordUrl: str
defaultView: int (enum)
guidePermissionType: int (enum)
resourcePermissionType: int (enum)
staticAssets[]
    #Asset#
```

# Category
GetGameData, GetLatestLeaderboard, GetModerationRuns
```
id: str
name: str
url: str
pos: int
gameId: str
isMisc: bool
isPerLevel: bool
numPlayers: int
exactPlayers: bool
playerMatchMode: int (enum)
timeDirection: int (0 = fastest)
enforceMs: bool
archived: bool
rules: str
```

# Level
GetGameData, GetLatestLeaderboard, GetModerationRuns
```
id: str
gameId: str
name: str
url: str
pos: int
rules: str
archived: bool
```

# Platform
GetGameData, GetLatestLeaderboard, GetModerationRuns
```
id: str
name: str
url: str
year: int
```

# Region
GetGameData, GetLatestLeaderboard
```
id: str
name: str
url: str
flag: str
```

# Run
GetGameLeaderboard2, GetGameRecordHistory, GetLatestLeaderboard, GetModerationRuns
```
id: str
gameId: str
categoryId: str
?time: int
?timeWithLoads: int
?(another for IGT?) : int
?enforceMs: bool
platformId: str
emulator: bool
video: str
comment: str
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
```

# Theme
GetGameSettings, GetSeriesSettings, GetSession, GetThemeSettings, GetUserSettings
```
id: str
url: str
primaryColor: str
panelColor: str
panelOpacity: int
navbarColor: int
backgroundColor: str (hex)
backgroundFit: int
backgroundPosition: int
backgroundRepeat: int
backgroundScrolling: int
foregroundFit: 0
foregroundPosition: int
foregroundRepeat: int
foregroundScrolling: int
touchDate: int
staticAssets[]
    #Asset#
```

# Variable
GetLatestLeaderboard
```
    id: str
    name: str
    url: str
    pos: int
    gameId: str
    categoryScope: int (enum?)
    categoryId: str
    levelScope: int (enum?)
    ?levelId: str
    isMandatory: bool
    isSubcategory: bool
    isUserDefined: bool
    isObsoleting: bool
    defaultValue: str
    archived: bool
    ?displayMode: int (enum?)
```

# Value
GetLatestLeaderboard
```
id: str
name: str
url: str
pos: int
variableId: str
isMisc: bool
?rules: str
archived: bool
```

# User
GetGameData, GetSearch, GetCommentList, GetConversationMessages, GetConversations, GetForumList, GetGameSettings, GetRunSettings, GetSeriesSettings, GetSession, GetThread, GetTickets
```
id: str
name: str
url: str
powerLevel: int
pronouns[str]
areaId: str
color1Id: str
color2Id: str
?isSupporter
?colorAnimate: int # No clue when this shows up
?iconType # Where specific user details are desired (user profile?)
?onlineDate: int
?signupDate: int
?touchDate: int
?staticAssets[]
    #Asset#
```