Parameters are wrapped inside `params`, except `page`.

## Required parameters:
- gameId
- categoryId

## Optional parameters
- values[] TODO: document value structure
- video `0 = any, 1 = present, 2 = missing`
- verified
- timer
- obsolete
- platformIds[]
- regionIds[]
- page

# Response
```
runList [
    #Run#
]
playerList [
    id: str
    name: str
    url: str
    powerLevel: int (appears to be site admin? default 1, Meta is 4)
    color1Id: str
    color2Id: str
    colorAnimate: int
    areaId: str
    ?isSupporter
]
pagination
    count: int
    page: int
    pages: int
    per: int
```