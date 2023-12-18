## Required Parameters
- userID: str

_Bruteforced, other parameters may exist_

# Response
```
categories[]
    #Category#
games[]
    #Game#
levels[]
    #Level#
platforms[]
    #Platform#
players[]
    #Player#
regions[]
    #Region#
runs[]
    #Run#
user
    #User#
userProfile
    userId: str
    signupDate: int
    defaultView: int
    showMiscByDefault: bool
    gameOrdering
        defaultGroups[]
            id: str
            name: str
            sortType: int
            gameIds[str]
        supporterGroups[]
            id: str
            name: str
            sortType: int
            gameIds[str]
    ?featuredFullRunId: str
    ?featuredLevelRunId: str
users[]  // always empty
    ???
values[]
    #Value#
variables[]
    #Variable#
followedGameIds: null
challengeList[]
    #Challenge#
challengeRunList[]
    #Run#
```