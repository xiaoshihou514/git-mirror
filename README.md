A small `fish` script that helps you setup read only git mirrors.

Requires `jq`.

```
Manage read-only git mirrors

Usage:
  git-mirror add <name> <url>
  git-mirror add_presets
  git-mirror push
```

Preset file format (default location is `$HOME/.config/git-mirror.json`):

```json
[
  {
    "name": "codeberg",
    "url": "ssh://git@codeberg.org/xiaoshihou/%s.git"
  },
  {
    "name": "sourcehut",
    "url": "git@git.sr.ht:~xiaoshihou/%s"
  },
  {
    "name": "gitlab",
    "url": "git@gitlab.com:xiaoshihou/%s.git"
  }
]
```
