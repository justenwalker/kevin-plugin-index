# kevin-plugin-index

A [kevin](https://github.com/justenwalker/kevin) plugin index. Lists plugins and their signed release versions for `kevin plugin index add` to discover.

## Use this index

```sh
kevin plugin index add https://github.com/justenwalker/kevin-plugin-index
kevin plugin search
```

## Layout

```text
kevin-index.yaml
plugins/
  <name>/
    plugin.yaml
    versions/
      <version>.yaml
```

`kevin-index.yaml` holds `layout: 1`.

Each plugin has a `plugin.yaml` (name, summary, homepage, maintainer, signers) and one `versions/<version>.yaml` per release, never edited after it's published.

See kevin's [Plugin index format](https://justenwalker.github.io/kevin/docs/reference/plugin-index/) reference for every field, and [Publishing a plugin](https://justenwalker.github.io/kevin/docs/extending/publishing-a-plugin/) for how to add a plugin here.

## Plugins

| Plugin | Summary |
|:-------|:--------|
| [echo](plugins/echo/plugin.yaml) | Demonstrates the kevin plugin protocol. Echoes a message, no real resource. |
