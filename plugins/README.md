# Plugins

Community-distributed iappyxOS Launcher plugins live here. Each plugin is its own folder under `plugins/<slug>/` and ships at minimum:

```
plugins/<slug>/
  manifest.json     # plugin manifest — id, capabilities, exposed methods
  plugin.html       # plugin runtime (hidden WebView)
  meta.json         # showcase metadata (title, description, author, added)
  settings.html     # OPTIONAL — per-plugin configure page
  icon.png          # OPTIONAL — 256x256
  README.md         # OPTIONAL — shown in the plugin's showcase entry
```

Plugins are JavaScript modules that extend the launcher with new capabilities — remote photo libraries, calendar mirrors, push routing, integrations with self-hosted services. They run in a hidden, sandboxed WebView and talk to other apps through bridges declared in their `manifest.capabilities` (the user grants those at install time via a consent dialog).

## Submitting

The launcher's editor (Remote Edit → Showcase tab → Plugins) has a "Submit" button on user-installed plugins; alternatively, open a pull request against this repo with a new `plugins/<slug>/` folder and the corresponding `plugins[]` entry in `showcase.json`.

## meta.json shape (for the showcase entry)

```json
{
  "title": "Immich",
  "description": "Photos from a self-hosted Immich server.",
  "author": "you",
  "added": "2026-05-01"
}
```

## manifest.json shape (for the plugin runtime)

See the launcher's `plugins/README.md` and the bundled `assets/plugins/immich/manifest.json` for the full schema.

## Bundled plugins

Plugins listed in [`launcher's BUNDLED_PLUGINS`](https://github.com/iappyx/iappyxOS-Launcher) ship in the launcher APK and don't need to be installed from the showcase. They appear in the browse list with a "Built-in" badge.
