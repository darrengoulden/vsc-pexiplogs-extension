# Pexip Log Syntax

VSCode extension for Pexip log syntax highlighting with the Dark+ VSC theme.

## Install

Update `settings.json`

1. Open the Settings editor from the Command Palette (⇧⌘P or Ctrl+Shift+P) with Preferences: Open Settings (JSON)
2. Add the below
3. Save

```
"files.associations": {
	"**/var/log/*.log*": "pexip"
}
```

Install the extension

1. Select View > Extensions
2. Select the three dots on top of the Extensions menu > Install from VSIX...

## Release Notes

* 0.0.2: Pattern match additions
* 0.0.1: Minor Release, Commit Message: Initial Commit and Build.
