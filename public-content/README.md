# Naseem public content seed

Copy this folder's contents to the root of the separate public repository `midhT/Naseem-public`. Keep the repository public: the app reads these JSON files without credentials.

## Files
- `release.json` — release version, public release URL, APK download URL and publication date. The CI release workflow writes this after publishing the APK.
- `content/glance.json` — daily reflections, lessons and quizzes. Keep `schemaVersion` supported by the app and increment `contentVersion` when content changes.
- `content/duas.json` — Dua Library entries. Keep Arabic, transliteration, meaning and references verified; increment `contentVersion` for changes.

The app validates feed structure, caches valid content locally and retains built-in fallback content. A public feed outage must not make the app unusable.

Never store private user data, signing keys, passwords, personal access tokens or other credentials here. Never publish religious content without checking the Arabic text and references against trusted sources. The public feed seed is not a signed application release.
