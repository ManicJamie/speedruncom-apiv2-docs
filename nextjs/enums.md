Extremely useful - nextjs requests contain an `enums` namespace which contains what appears to be all frontend enums!

```json
{
    "DefaultViewType": {
        "0": "Full game",
        "1": "Levels"
    },
    "DefaultViewType_GameSettings": {
        "0": "Full game leaderboard",
        "1": "Level summary"
    },
    "EmulatorFilter": {
        "0": "Hidden",
        "1": "Shown",
        "2": "Exclusive"
    },
    "EmulatorType": {
        "0": "Hidden by default",
        "1": "Shown by default",
        "-1": "Banned"
    },
    "FitType": {
        "0": "Original size",
        "1": "Fit to screen"
    },
    "GameModeratorLevel": {
        "0": "Moderator",
        "1": "Super moderator",
        "-1": "Verifier"
    },
    "GameOrderType": {
        "1": "Name",
        "2": "Newest released",
        "3": "Oldest released",
        "4": "Most active players",
        "5": "Least active players",
        "6": "Most total players",
        "7": "Least total players",
        "8": "Most runs",
        "9": "Least runs",
        "10": "Newest added",
        "11": "Oldest added"
    },
    "GameTypeId": {
        "1": "ROM hack",
        "2": "Modification",
        "3": "Fan game",
        "4": "Web game",
        "5": "Pre-release game",
        "6": "Mobile game",
        "7": "Expansion / DLC",
        "8": "Category extensions",
        "9": "Multiple games",
        "10": "Mini game",
        "11": "Server map",
        "12": "Homebrew game"
    },
    "HomepageStreamType": {
        "0": "Show the stream (muted)",
        "1": "Show the stream (paused)",
        "2": "Hide the stream"
    },
    "NavbarColorType": {
        "0": "Primary color",
        "1": "Panel color"
    },
    "ObsoleteFilter": {
        "0": "Hidden",
        "1": "Shown",
        "2": "Exclusive"
    },
    "PermissionType": {
        "0": "All users",
        "1": "Disable for this game",
        "2": "Users with a verified run (in any game)",
        "3": "Users with a verified run (in this game)",
        "4": "Game moderators"
    },
    "PlayerMatchMode": {
        "0": "All players, exact order",
        "1": "All players, any order",
        "2": "Any players, exact order",
        "3": "Any players, any order"
    },
    "PositionType": {
        "0": "Top left",
        "1": "Top",
        "2": "Top right",
        "3": "Left",
        "4": "Center",
        "5": "Right",
        "6": "Bottom left",
        "7": "Bottom",
        "8": "Bottom right"
    },
    "RepeatType": {
        "0": "No repeat",
        "1": "Horizontal",
        "2": "Vertical",
        "3": "Both"
    },
    "ResourceType": {
        "1": "Tool",
        "2": "Save",
        "3": "Splits",
        "4": "Patch"
    },
    "RunVerificationState": {
        "0": "Pending",
        "1": "Verified",
        "2": "Rejected"
    },
    "ScrollType": {
        "0": "No scroll",
        "1": "Slow speed",
        "2": "Medium speed",
        "3": "Fast speed"
    },
    "SupporterCreditType": {
        "1": "Subscription payment",
        "2": "Admin grant",
        "3": "Code redemption"
    },
    "SupporterIconType": {
        "0": "None",
        "1": "Default",
        "2": "Custom"
    },
    "SupporterSubscriptionCancelReason": {
        "1": "Too expensive",
        "2": "Not enough value",
        "3": "Interest / Time is shifting to other hobbies",
        "4": "Other"
    },
    "SupporterSubscriptionStatus": {
        "0": "Incomplete",
        "1": "Active",
        "2": "Unpaid",
        "3": "Canceled"
    },
    "TicketQueue": {
        "1": "Game requests",
        "2": "Series requests",
        "3": "Moderator reports",
        "4": "Marathon requests",
        "5": "Content reports",
        "6": "User reports",
        "7": "Bug reports",
        "8": "Front page requests",
        "9": "Feedback",
        "10": "Staff applications",
        "11": "Support",
        "12": "Content requests",
        "13": "Supporter"
    },
    "TicketStatus": {
        "0": "Pending",
        "1": "Approved",
        "2": "Denied",
        "3": "Reviewing",
        "4": "Withdrawn"
    },
    "TicketType": {
        "1": "Game request",
        "2": "Series request",
        "3": "Moderator request",
        "4": "Marathon request",
        "5": "Content report",
        "6": "User report",
        "7": "Bug report",
        "8": "Front page request",
        "9": "Feedback",
        "10": "Staff application",
        "11": "Other support",
        "12": "Game type update",
        "13": "Add to series request",
        "14": "Add platform request",
        "15": "Other game request",
        "16": "Supporter help"
    },
    "UserIconPosition": {
        "0": "Before name",
        "1": "After name"
    },
    "UserIconType": {
        "0": "None",
        "1": "Default",
        "2": "Custom"
    },
    "UserOrderType": {
        "1": "Name",
        "2": "Newest",
        "3": "Oldest"
    },
    "UserPowerLevel": {
        "0": "Banned",
        "1": "User",
        "2": "Content Moderator",
        "3": "Site Moderator",
        "4": "Site Admin"
    },
    "VariableCategoryScope": {
        "1": "Single category...",
        "-1": "All categories"
    },
    "VariableDisplayMode": {
        "0": "Automatic",
        "1": "Dropdown",
        "2": "Button group"
    },
    "VariableLevelScope": {
        "0": "Full game",
        "1": "Single level...",
        "-1": "Levels",
        "-2": "Full game and levels"
    },
    "VideoFilter": {
        "0": "Optional",
        "1": "Required",
        "2": "Missing"
    }
}
```