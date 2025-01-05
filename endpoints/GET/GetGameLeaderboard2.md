Parameters are wrapped inside `params`, except `page`.

## Required parameters:
- gameId
- categoryId

## Optional parameters
- values[]
    - Consists of objects containing `variableId` and a list of `valueIds`.
- video (`0 = optional, 1 = required, 2 = missing`)
- verified (`0 = pending, 1 = verified, 2 = rejected`)
- timer
- obsolete (`0 = hidden, 1 = shown, 2 = exclusive`)
- platformIds[str]
- regionIds[str]
- dateFrom: str
- dateTo: str
- page: int

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
