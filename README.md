# sober-time-backend

Static versioning endpoint for the Sober Time client.

The app `GET`s `version.json` to learn the latest and minimum supported
versions. Bump the numbers here when you ship a store build; set
`forceUpdate` to `true` (or raise `minSupportedVersion`) when older clients
must update.

## Client URL

After this repo is public (or GitHub Pages is enabled):

```
https://raw.githubusercontent.com/mahdiafshar/sober-time-backend/main/version.json
```

GitHub Pages (if enabled on `main` / root):

```
https://mahdiafshar.github.io/sober-time-backend/version.json
```

## Fields

| Field | Meaning |
| --- | --- |
| `latestVersion` / `latestBuild` | Newest store release (`pubspec` `version` + build) |
| `minSupportedVersion` / `minSupportedBuild` | Oldest client still allowed to run |
| `forceUpdate` | Soft prompt vs must-update, independent of min version |
| `store.android` / `store.ios` | Store / download links for the update CTA |
