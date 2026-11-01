# BorderPatrol player list

The Ally/Enemy player list of clan BP, kept up to date automatically by the
CresSlayer9000 Discord bot. When a player is added, changed or removed,
`players.json` here is updated within about a minute.

## Using it

Download this file - no key or login needed:

```
https://raw.githubusercontent.com/agentyautja/borderpatrol-list/main/players.json
```

```json
{
  "version": 1,
  "updated": "2026-11-01T14:02:00Z",
  "count": 271,
  "players": [
    {"username": "SomePlayer", "roblox_id": 123456, "status": "Enemy", "clan": "SOMECLAN"}
  ]
}
```

| Field | Meaning |
|---|---|
| `username` | Roblox username (as it was when last added or edited) |
| `roblox_id` | Roblox user ID - match on this, it doesn't change when someone renames |
| `status` | `Ally` or `Enemy` |
| `clan` | Clan name, or `null` if none is known |

Players are sorted Enemies first, then by clan and name. Fetch the file at most
once a minute; GitHub may cache it for up to 5 minutes.
