Gets the summary shown on the "Level" page, with the top 3 from each level in a category.

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
category
    #Category#
runList[]
    #Run#
playerList[]
    id: str
    name: str
    url: str
    powerLevel: int (enum)
    color1Id: str
    color2Id: str
    colorAnimate: int (enum)
    areaId: str
```