# aosp-camper-navigator

Prebuilt CamperNavigator app for the AOSP build (`Android.bp` imports `CamperNavigator.apk`).

The APK is **not stored in git**. It is published as a GitHub release asset and pinned in
`APK_RELEASE` (tag and SHA-256). Fetch it before building:

```
packages/apps/CamperNavigator/fetch_apk.sh
```

## Publishing a new APK

1. Create a release with the new file, for example
   `gh release create apk-<yyyymmdd> CamperNavigator.apk --title "CamperNavigator <yyyymmdd>"`.
2. Update `TAG` and `SHA256` in `APK_RELEASE` (`sha256sum CamperNavigator.apk`) and commit.
