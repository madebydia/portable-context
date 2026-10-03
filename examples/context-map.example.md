# Private context map template

Copy this outside the public repository, then replace the placeholders. These are configuration fields, not a required vault layout. Existing routing instructions can replace this map.

- **Store:** `<absolute path or authorized connector location>`
- **Routing and ownership instructions:** `<existing document or index>`
- **Capture scope:** `<for example: automatic durable capture across this host's conversations, or only when requested>`
- **Explicit exclusions:** `<excluded topics/locations, or none>`
- **Date convention:** `<timezone and preferred format>`

## Authoritative destinations

Point to existing locations where available. Use relative paths within a file store. Omit unused roles; do not create empty files merely to fill this list.

| Role | Existing destination / rule |
| --- | --- |
| Stable preferences | `<profile or preference note>` |
| Active projects and topic discovery | `<index or routing document>` |
| Decisions and current work | `<relevant project/domain note>` |
| Dated observations | `<evidence log or daily-note convention>` |
| Procedures | `<owning workflow location and editing rules>` |
| Tasks and other operational records | `<owning system; vault stores pointers>` |
| Exclusions preventing reimport | `<established exclusions location or affected topic note>` |

## Writing rules

- **New topic notes:** `<allowed within existing domains, or another chosen limit>`
- **Naming and section ownership:** `<existing conventions>`
- **Sensitive categories:** `<applicable restrictions>`
- **Conflict handling:** `<revision checks or storage conflict behavior, if known>`

Automatic capture within the chosen scope does not authorize new data access, external actions, historical backfills, or schedules. No-save requests and narrower task instructions take precedence.
