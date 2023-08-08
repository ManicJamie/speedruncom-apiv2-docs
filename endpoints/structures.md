# Data structures

Commonly seen data structures will be placed here for easier reference. Names are made up.

Attributes labeled with #Type# are documented here.

## GameInfo
GetSearch, GetLatestLeaderboard, GetForumList, GetGameSettings, GetModerationGames, GetModerationRuns, GetSeriesSettings, GetSession, GetUserSettings, PutGame
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
    assetType: str
    path: str
```