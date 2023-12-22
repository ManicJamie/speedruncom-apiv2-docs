# PutAuthLogin

Endpoint for attempting a login into https://speedrun.com (Note: this is the only endpoint that appears to be accessible without a PHPSESSID).

# Body

> ? = optional

```json
{
	"name": "{username}",
	"password": "{password}",
	"token?": "{2fa token}"
}
```

# Response

Successful login response includes a `Cookie`/`Set-Cookie` header with appropriate PHPSESSID;
`PHPSESSID=xxxx; Path=/; Domain=speedrun.com; Expires=Tue, 23 Jul 2024 22:52:09 GMT; HttpOnly`

## Type (WIP)


```typescript
interface PutAuthLogin {
  isLoggedIn: boolean;
  tokenChallengeSent?: boolean;
}
```