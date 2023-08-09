Get moderation data

# Required Parameters
- gameId
- limit `max: 100`
- page

# Optional Parameters
- search
- verified
- verifiedById

# Response
```
categories[]
    #Category#
games[]
    #GameInfo#
levels[]
    #Level
pagination
    count
    page
    pages
    per
platforms[]
    #Platform#
players[]
    id: str
    name: str
    url: str
    powerLevel: int
    color1Id: str
    colorAnimate: int
    areaId: str
regions[]
    # not documented
runs[]
    #Run#
```