# Obsidian Source Sync

Obsidian Source Sync is an Obsidian desktop plugin for syncing RedNote/Xiaohongshu bookmarks, likes, posts, albums, media, and comments into a local Obsidian vault.

Created by `坦丁|场景化AI知识库`.

## Install With BRAT

BRAT is recommended because it can install the plugin and follow GitHub Releases for updates.

1. In Obsidian, install and enable `BRAT` from Community plugins.
2. Open BRAT and choose `Add Beta plugin`.
3. Enter this repository URL:

```text
https://github.com/sundayding/obsidian-source-sync
```

4. After installation, open `Settings -> Community plugins` and enable `Obsidian Source Sync`.
5. BRAT will install the plugin into `.obsidian/plugins/multi-source-sync/`, based on the plugin ID in `manifest.json`.

## Trial And License

- Trial users can sync up to 100 notes.
- Permanent-license users unlock unlimited sync, richer comment sync, comment replies, local video transcription, AI classification, and AI comment insights.
- Paid features are unlocked with an authorization code from the Xiaohongshu order flow.
- The plugin verifies licenses through `https://multi-source-sync.pages.dev/v1/license/verify`.

## Manual Fallback

If BRAT or GitHub is temporarily unavailable, use the cloud-drive package provided through the Xiaohongshu order auto-reply or private message. For an existing manual install, replace only these program files inside `.obsidian/plugins/multi-source-sync/`:

- `main.js`
- `manifest.json`
- `styles.css`

Do not delete or replace `data.json`, synced Markdown, media folders, account folders, or other vault content.

## Privacy Boundary

Markdown, media, comments, RedNote account data, license data, device ID, and AI API keys are stored locally in your Obsidian vault/plugin data. The license service only validates license and device binding. AI calls happen only after you enable AI and configure an API key.
