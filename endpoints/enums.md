# Enums

This list attempts to document the canonical meanings of various int and string enums.

Further enums have been implemented in [speedruncompy/enums.py](https://github.com/ManicJamie/speedruncompy/blob/master/speedruncompy/enums.py).

## itemType
Displayed in various places, including thread comments, (continue)
```
Unknown = 0
Article = 30
Comment = 1
Run = 2
Game = 3
Guide = 4
Resource = 5
User = 6
Thread = 7
GameMod = 8
Category = 9
Level = 10
GameRequest = 11
News = 27
GameBoostToken = 28
GameBoost = 29
Ticket = 22
TicketNote = 23
UserFollower = 31
Challenge = 32
ChallengeRun = 33
```

## Verified
Run verification status
```
0 = Pending
1 = Verified
2 = Rejected
```

## ObsoleteFilter
Filter for obsolete status in grouped run requests
```
0 = Hidden
1 = Shown
2 = Exclusive
```

## VideoFilter
Filter for runs with a video link
```
0 = Optional
1 = Required
2 = Missing
```

## eventType
Displayed in audit log
```py
""
"category-created"
"category-removed"
"category-restored"
"category-updated"
"comment-created"
"comment-deleted"
"comment-updated"
"game-covers-updated"
"game-created"
"game-moderator-created"
"game-moderator-removed"
"game-moderator-updated"
"game-news-post-created"
"game-news-post-edited"
"game-news-post-removed"
"game-restored"
"game-updated"
"gamerequest-reviewed"
"level-created"
```

## type (in Game)
Not entirely sure. is this ever not "game"?
```py
"game"
```

## gameTypeIds (list in Game)
(taken from nextjs namespace)
```
1 = ROM hack,
2 = Modification,
3 = Fan game,
4 = Web game,
5 = Pre-release game,
6 = Mobile game,
7 = Expansion / DLC,
8 = Category extensions,
9 = Multiple games,
10 = Mini game,
11 = Server map,
12 = Homebrew game
```

## type (in Forum)
```
0 = front page
1 = supporter
2 = game
```

## type (in Resource)
```
1 = Tool
2 = Save
3 = Splits
4 = Patch
```

## runCommentsMode
```
1 = disabled
```

## validTimers
Part of game info
```discord
0 = RTA
1 = LRT? (TODO: check)
2 = IGT
```

## VariableCategoryScope
```
1 = Single Category
-1 = All Categories
```

## VariableLevelScope
```
0 = Full game
1 = Single Level
-1 = All Levels
-2 = Full game & All Levels
```

## Ticket Queue
NOT the same as ticket type!
```
1 = Game requests
2 = Series requests
3 = Moderator reports
4 = Marathon requests
5 = Content reports
6 = User reports
7 = Bug reports
8 = Front page requests
9 = Feedback
10 = Staff applications
11 = Support
12 = Content requests
13 = Supporter
```

## Ticket type
```
1 = Game Request
2 = Series Request
3 = Mod Request
4 = Marathon Request
5 = Content Report
6 = User Report
7 = Bug Report
8 = Front Page Request
9 = Feedback
10 = Staff Application
11 = Other Support
12 = Game Type Update
13 = Add To Series Request
14 = Add Platform Request
15 = Other Game Request
16 = Supporter Help
```

## Ticket Status
```
0 = Pending
1 = Approved
2 = Denied
3 = Reviewing
4 = Withdrawn
```

## level (of Game Moderator)
```
-1 = Verifier
0 = Moderator
1 = Super Moderator
```

# networkId (in userSocialConnectionList)
```
3 = Bilibili
5 = Discord
8 = Facebook
11 = Instagram
15 = Niconico
18 = Reddit
29 = Twitch
30 = Twitter
31 = Website
32 = Youtube
```

Deprecated values are not visible on the website or settable by users anymore
Deprecated values:
```
1 = Askfm
2 = Battlenet
4 = Deviantart
6 = Douyu
7 = Duolingo
9 = Googleplus
10 = Gpodcasts
12 = Itunes
13 = Mixer
14 = Mmrta
16 = Patreon
17 = Pinterest
19 = Smashcast
20 = Snapchat
21 = Soundcloud
22 = Splitsio
23 = Spotify
24 = Spotifyshow
25 = Srl
26 = Steam
27 = Stitcher
28 = Tumblr
33 = Zsr
```