# Enums

This list attempts to document the canonical meanings of various int and string enums.

## itemType
Displayed in various places, including thread comments, (continue)
```
1 = Like? Appears in GetThread.likeList[]
2 = Run
7 = Thread comment? Thread?
27 = Game news post
30 = Site news post
```

## Verified
Run verification status
```
0 = Pending
1 = Verified
2 = Rejected
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
```
"game"

```

## gameTypeIds (list in Game)
At a guess, to do with subgames
```
2 = modded?
8 = category extensions
11 (strawberry jam collab)
```

## type (in Forum)
```
0 = front page
1 = supporter
2 = game
```

## runCommentsMode
```
1 = disabled
```

## validTimers
Part of game info
```
0 = RTA
1 = LRT? (TODO: check)
2 = IGT
```

## Ticket type
```
5 = Content Report
```

## level (of Game Moderator)
```
-1 = Verifier
0 = Moderator
1 = Super Moderator
```

# networkId (in userSocialConnectionList)
```
5 = Discord
29 = Twitch
32 = Youtube
```