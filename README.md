# Speedrun.com's super secret v2 API

This API is pre-production, subject to change and, more importantly, not directly exposed to us. Endpoints documented here are all endpoints that have been found by inspecting XHR requests made by the new website.

Further, this documentation is Very Incomplete and Very Bad. I may make it better, but I assume if you're using this API you probably know enough about what you're doing that I don't need to document all potential errors and workflows.

Note that dates returned from the API are typically UNIX timestamps, whereas date parameters (eg. dateFrom and dateTo) are typically strings (`yyyy-mm-dd`).

## Authentication
Being preproduction, we can only auth using session authentication with this api - we must call `PutAuthLogin` & save the returned cookie for future calls. Note that if you want to use verifier/moderator endpoints, you must go through 2fa to login.
Certain endpoints require a `csrfToken`; this can be obtained from `GetSession` when logged in.

The `GET` endpoints do not require authentication. I have verified that `GetSession`, `PutAuthLogin` and `PutAuthSignup` all work unauthed (obviously). Some (maybe all? untested) GET endpoints also work as POST, and some are requested with each method interchangeably by the website.

# Reading these docs
Nothing here is very consistent, but I have done my best to help where needed.

Where keys are only sometimes present, the key name is prefixed by a ?. 
Where fields may have a null value, the type is prefixed with a ?.

Note [enums](/endpoints/enums.md) and [structures](/endpoints/structures.md) are frequently referenced. 

Structures have had their fields replaced with #Struct_name# - if an apparent structure is not replaced, be careful! There may be additional (or missing) fields you haven't seen.

Enums are sparsely documented, listed in [enums](/endpoints/enums.md) by their key name, not a logical name. Wrappers may wish to edit these to more sensible names in places. Note they may be missing potential values - be careful when using!

## TODO
Remaining endpoints that are undocumented:
- PutUserSupporterNewSubscription

Various enums need to be documented:
- [ ] itemType (eg. GetCommentable)

More enums are definitely present, but this is not a personal priority of mine. Feel free to PR.

The following endpoints were found via brute force and not through use on the site, and as such may be missing parameters. Ticked endpoints have sufficient documentation for use.
- [x] GetArticleList
- [x] GetHomeSummary
- [x] GetGameList
- [x] GetSeriesList 
- [x] GetNews
- [x] GetNewsList
- [x] GetThreadList
- [x] GetGuideList
- [x] GetResourceList
- [x] GetGameSummary
- [x] GetForumList
- [x] GetArticle
- [x] GetChallenge
- [x] GetChallengeLeaderboard
- [ ] GetChallengeList (appears to require site mod?)
- [ ] GetChallengeRuns
- [x] GetChallengeRun

Additional endpoints may exist, or get added later. Feel free to raise an issue or PR if there is an endpoint missing.

Various attributes are likely missing, feel free to raise issue or PR on those too.