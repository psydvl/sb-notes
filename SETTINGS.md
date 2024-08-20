#meta [[PLUGS]]

This page contains some configuration overrides for SilverBullet. A list of configs and their documentation [[!silverbullet.md/SETTINGS|can be found here]].

To update the [[!silverbullet.md/Libraries|libraries]] specified below, run {[Libraries: Update]}

```space-config
indexPage: index
libraries:
- import: "[[!silverbullet.md/Library/Core/*]]"

git: # github:silverbulletmd/silverbullet-git/git.plug.js
  autoCommitMinutes: 5
  autoSync: false # or true

katex: # github:silverbulletmd/silverbullet-katex/katex.plug.js
  # To change the default rendering mode to displaystyle, alternatively use `\displaystyle` in the block
  displayMode: false
  # To enable some special features KaTeX offers to e.g. allow DOM manipulation
  # Alternatively specifiy a list of features. For reference: https://katex.org/docs/options
  allowedFeatures: all
  # Macros can be globally specified likes this. Make sure to escape the backslash
  macros:
    - macro: "\\coolR"
      expansion: "\\mathbb{R}"
```

---
# Check
## KaTeX

```latex
e=mc^2
```
```latex  
c = \pm\sqrt{a^2 + b^2}  
```

