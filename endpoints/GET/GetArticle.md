## Required Parameters
- id OR
- slug

_Bruteforced, other parameters may exist_

# Response
```
article
    id
    slug
    title
    summary
    body
    createDate
    updateDate
    publishDate
    publishTarget
    publishTags
    commentsCount
relatedArticleList[] // Undocumented, assume as above
gameList[]
    #Game#
userList[]
    #User#
```