# Pexip Log Syntax  

VSCode extension for Pexip log syntax highlighting.  
 
Made for the `Dark+` VSC theme, highlighting will work in other themes but it won't be as optimised.

## Install  

Update `settings.json` 

1. Open the Settings editor from the Command Palette (⇧⌘P or Ctrl+Shift+P) with Preferences: Open Settings (JSON)
2. Add the below
3. Save 

```
"files.associations": {
	"**/diagnostic_snapshot_*/log/*.log*": "pexip"
}
```
 
Install the extension 

Grab the latest VSIX from the [releases](https://github.com/darrengoulden/vsc-pexiplogs-extension/releases) section then in VSCode;
1. Using the Install from VSIX command in the Extensions view command dropdown
2. or the `Extensions: Install from VSIX` command in the Command Palette (⇧⌘P or Ctrl+Shift+P), point to the `.VSIX` file.  

## Release Notes  

* 0.0.2: Pattern match additions
* 0.0.1: Minor Release, Commit Message: Initial Commit and Build.