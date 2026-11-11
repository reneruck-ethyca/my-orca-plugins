# My Orca Plugins

Personal [Orca](https://github.com/stablyai/orca) plugins and themes. Each plugin lives in its own
folder under `plugins/`, and `orca-catalog.json` lists them so Orca can install from this repo.

## Plugins

| Plugin | What it adds |
| --- | --- |
| [`ember-theme`](plugins/ember-theme) | Ember Light and Ember Dark app themes |

## Develop

```sh
orca plugin create plugins/<name> --template <theme|terminal-theme|icon-theme|components|...>
orca plugin dev watch plugins/<name>     # load into Orca and hot-reload on save
orca plugin validate plugins/<name> --json
```

## Publish a release

1. Bump `version` in the plugin's `orca-plugin.json`, commit, and push to `main`.
2. Run `orca plugin release-entry plugins/<name> --json` and add the printed release to that
   plugin's entry in `orca-catalog.json` (newest first, with `source.path` set to `plugins/<name>`).
3. Commit and push the catalog. In Orca, add this repo's Git URL as a catalog under Settings → Plugins.
