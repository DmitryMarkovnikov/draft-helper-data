# draft-helper-data

Static data packages for the draft-helper mobile app: aggregated League of Legends ranked
statistics per patch, rank bracket and region (champion win rates, lane matchups, rune pages,
summoner spells, item builds, champion tags). No player data is included.

Layout:

- `packages/index.json` — the latest package per `region/rank`, with size and sha256
- `packages/{region}/{rank}/{patch}-v{version}/package.zip` — immutable package archives
- `packages/{region}/{rank}/{patch}-v{version}/meta.json` — copy of the package metadata

Source: Riot Games API (Match-v5, League-v4) and Data Dragon.

draft-helper isn't endorsed by Riot Games and doesn't reflect the views or opinions of
Riot Games or anyone officially involved in producing or managing Riot Games properties.
Riot Games and League of Legends are trademarks or registered trademarks of Riot Games, Inc.
