# zqmlabs-gamification

Gamification service for [zqmlabs.com](https://zqmlabs.com) — missions, leaderboard, scoring, achievements.

## Domain: zqmlabs.com/gamification

| Feature | Description |
|---------|-------------|
| Missions | Track and complete gamification missions |
| Leaderboard | Community scoring and rankings |
| Achievements | Badge and milestone system |
| Scoring | Points calculation and aggregation |

## Architecture

This is the **gamification layer** of the ZQM modular architecture. It provides:
- Mission tracking and completion
- Leaderboard scoring
- Achievement/badge system
- Points calculation

## API Endpoints

| Endpoint | Function |
|----------|----------|
| `/health` | Health check |
| `/missions` | List all missions |
| `/leaderboard` | Community rankings |
| `/scoring` | Points calculation |

## Domain Mapping

```
zqmlabs.com/gamification → zqmlabs-gamification (separate service)
zqmlabs-backend ←→ zqmlabs-gamification (proxy)
zqmlabs-frontend ←→ zqmlabs-gamification (API calls)
```

## Repo Map

```
zqmlabs-frontend ←→ zqmlabs-gamification (gamification UI)
zqmlabs-backend ←→ zqmlabs-gamification (proxy route)
zqmlabs-gamification ←→ zqmlabs-shared (shared types)
```
