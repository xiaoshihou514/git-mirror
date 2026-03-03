A small `fish` script that helps you setup read only git mirrors.

Requires `jq`.

```
Manage read-only git mirrors

Usage:
  git-mirror add <name> <url>
  git-mirror add_preset
  git-mirror push
```

Preset file format (default location is `$HOME/.config/git-mirror.json`):

```json
[
  {
    "name": "codeberg",
    "url": "ssh://git@codeberg.org/%s/%s.git",
    "type": "forgejo",
    "user": "xiaoshihou",
    "host": "codeberg.org"
  },
  {
    "name": "disroot",
    "url": "ssh://git@git.disroot.org/%s/%s.git",
    "type": "forgejo",
    "user": "xiaoshihou",
    "host": "git.disroot.org"
  },
  {
    "name": "sourcehut",
    "url": "git@git.sr.ht:~%s/%s",
    "type": "sourcehut",
    "user": "xiaoshihou",
    "host": "sr.ht"
  },
  {
    "name": "gitlab",
    "url": "git@gitlab.com:%s/%s.git",
    "type": "gitlab",
    "user": "xiaoshihou",
    "host": "gitlab.com"
  },
  {
    "name": "gitgud",
    "url": "git@gitgud.io:%s/%s.git",
    "type": "gitlab",
    "user": "xiaoshihou514",
    "host": "gitgud.io"
  },
  {
    "name": "frama",
    "url": "git@framagit.org:%s/%s.git",
    "type": "gitlab",
    "user": "xiaoshihou",
    "host": "framagit.org"
  }
]
```
