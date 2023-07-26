# Enums

This list attempts to document the canonical meanings of various int and string enums.

## itemType
Displayed in various places, including thread comments, (continue)
```
2 = Run
7 = Thread
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