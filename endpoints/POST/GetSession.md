# GetSession

Endpoint for getting the current session from https://speedrun.com

## Body

> You may need to send an empty (json object) body?

```json
{}
```

You do need to send a `PHPSESSID` in the Cookie header.

## Response

If you're authed, you get the full object as shown below. 
If not, you get an shortned object. The `signedIn` property is a hassle free way to tell if you're authed or not.

## Type (WIP)

```typescript
interface SessionData {
  session: {
    signedIn: boolean;
    showAds: boolean;
    user: {
      id: string;
      name: string;
      url: string;
      powerLevel: number;
      pronouns: string[];
      areaId: string;
      color1Id: string;
      color2Id: string;
      iconType: number;
      onlineDate: number;
      signupDate: number;
      touchDate: number;
      staticAssets: {
        assetType: string;
        path: string;
      }[];
    };
    theme: {
      id: string;
      name: string;
      url: string;
      primaryColor: string;
      panelColor: string;
      panelOpacity: number;
      navbarColor: number;
      backgroundColor: string;
      backgroundFit: number;
      backgroundPosition: number;
      backgroundRepeat: number;
      backgroundScrolling: number;
      foregroundFit: number;
      foregroundPosition: number;
      foregroundRepeat: number;
      foregroundScrolling: number;
      touchDate: number;
      staticAssets: any[];
    };
    powerLevel: number;
    dateFormat: number;
    timeFormat: number;
    timeReference: number;
    timeUnits: number;
    homepageStream: number;
    disableThemes: boolean;
    csrfToken: string;
    networkToken: string;
    gameList: any[];
    gameFollowerList: any[];
    gameModeratorList: any[];
    gameRunnerList: any[];
    seriesList: any[];
    seriesModeratorList: any[];
    boostAvailableTokens: number;
    boostNextTokenDate: number;
    boostNextTokenAmount: number;
    userFollowerList: any[];
  }
}
```