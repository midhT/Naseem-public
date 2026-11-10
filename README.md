# Naseem public content and releases

This folder is the seed for the separate public repository `midhT/Naseem-public`.

Copy its contents to the root of that repository. Keep the repository public so the app can read the JSON files without credentials.

## Files
- `release.json`: latest version metadata. After each GitHub Release, update `version`, `releaseUrl`, `downloadUrl`, `notesSummary`, and `publishedAt`.
- `content/duas.json`: remotely maintainable Dua Library source. The app still keeps its built-in content as an offline fallback until the remote loader is enabled and tested.
- `content/glance.json`: latest published Glance items. Set `published` to `true` only after content review.

Do not store private user data, signing keys, tokens, or credentials here. Do not publish religious content without verifying Arabic text and references against trusted sources.
