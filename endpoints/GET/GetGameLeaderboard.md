WARN: this is NOT used by the website, and as such may be removed at any time.

Parameters are wrapped inside `params`, except `page`.

## Required parameters:
- gameId
- categoryId

## Optional parameters:
not documented, assume same as GetGameLeaderboard2

# Response
```
leaderboard
    category
        #Category#
    game
        #Game#
    pagination
        count: int
        page: int
        pages: int
        per: int
    platforms[]
        #Platform#
    players[]
        id: str
        name: str
        url: str
        powerLevel: int (enum)
        color1Id: str
        color2Id: str
        colorAnimate: int (enum)
        areaId: str
    regions[]
        #Region#
    runs[]
        #Run#
    values[]
        #Value#
    variables[]
        #Variable#
```