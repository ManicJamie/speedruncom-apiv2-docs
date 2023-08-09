Gets most recent runs for a game or set of games. Apparent limit of 14 days.

seriesId and gameId act like filters a la v1 api, so we can use this to find the most recent runs on the site.

# Optional Parameters
- seriesId
- gameId
- limit = 10 `max: 999 WARN: limit over max defaults back to 10`

# Response
```
categories[]
    #Category#
games[]
    #GameInfo#
levels[]
    #Level#
platforms[]
    #Platform#
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
    #Region#
runs[]
    #Runs#
values[]
    #Value#
variables[]
    #Variable#
```