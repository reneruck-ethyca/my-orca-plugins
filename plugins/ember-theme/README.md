# Ember

Warm light and dark Orca app themes, ported from T3 Code's Ember palette. Edit `themes/light.json` and `themes/dark.json`; omitted tokens are derived from `--background` and `--foreground`.

## Develop

```sh
orca plugin validate .
orca plugin dev watch .    # loads this folder into Orca and prints its logs and reloads; Ctrl-C unloads it
```

Orca names the publisher after where the plugin is installed from: the GitHub or GitLab owner of
its repository, or `local` for a folder. See
https://github.com/stablyai/orca/blob/main/docs/reference/plugin-authoring.md.
