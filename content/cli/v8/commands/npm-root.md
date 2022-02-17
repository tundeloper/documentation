---
title: npm-root
section: 1
description: Display npm root
redirect_from:
  - /cli/root
  - /cli/root.html
  - /cli/commands/root
  - /cli-commands/root
  - /cli-commands/root.html
  - /cli-commands/npm-root
github_repo: npm/cli
github_branch: latest
github_path: docs/content/commands/npm-root.md
---

### Synopsis

```bash
npm root [-g]
```

### Description

Print the effective `node_modules` folder to standard out.

Useful for using npm in shell scripts that do things with the
`node_modules` folder.  For example:

```bash
#!/bin/bash
global_node_modules="$(npm root --global)"
echo "Global packages installed in: ${global_node_modules}"
```

### Configuration

<!-- AUTOGENERATED CONFIG DESCRIPTIONS START -->
<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->
#### `global`

* Default: false
* Type: Boolean

Operates in "global" mode, so that packages are installed into the `prefix`
folder instead of the current working directory. See
[folders](/cli/v8/configuring-npm/folders) for more on the differences in behavior.

* packages are installed into the `{prefix}/lib/node_modules` folder, instead
  of the current working directory.
* bin files are linked to `{prefix}/bin`
* man pages are linked to `{prefix}/share/man`

<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->

<!-- AUTOGENERATED CONFIG DESCRIPTIONS END -->

### See Also

* [npm prefix](/cli/v8/commands/npm-prefix)
* [npm bin](/cli/v8/commands/npm-bin)
* [npm folders](/cli/v8/configuring-npm/folders)
* [npm config](/cli/v8/commands/npm-config)
* [npmrc](/cli/v8/configuring-npm/npmrc)