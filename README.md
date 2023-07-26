# Speedrun.com's super secret v2 API

This API is pre-production, subject to change and, more importantly, not directly exposed to us. Endpoints documented here are all endpoints that have been found by inspecting XHR requests made by the new website.

Further, this documentation is Very Incomplete and Very Bad. I may make it better, but I assume if you're using this API you probably know enough about what you're doing that I don't need to document all potential errors and workflows.

## Authentication
Being preproduction, we can only auth using session authentication with this api - we must call `PutAuthLogin` & save the returned cookie for future calls. Note that if you want to use verifier/moderator endpoints, you must go through 2fa to login.
Certain endpoints require a `csrfToken`; this can be obtained from `GetSession` when logged in.

The `GET` endpoints do not require authentication. I have verified that `GetSession`, `PutAuthLogin` and `PutAuthSignup` all work unauthed (obviously).

## TODO
Remaining endpoints that are undocumented:
- PutUserSupporterNewSubscription

Various enums need to be documented:
- [ ] itemType (eg. GetCommentable)

More enums are definitely present, but this is not a personal priority of mine. Feel free to PR.

Additional endpoints may exist, or get added later. Feel free to raise an issue or PR if there is an endpoint missing.

Various attributes are likely missing, feel free to raise issue or PR on those too.