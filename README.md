# Pexip log syntax highlighting for VSCode

VSCode extension for Pexip log syntax highlighting.  
 
Made for the `Dark+` VSC theme, in other themes you may find that there is only partial highlighting.

## Install  

Update `settings.json` 

1. Open the Settings editor from the Command Palette (⇧⌘P or Ctrl+Shift+P) with `Preferences: Open Settings (JSON)`
2. Add the below (you can also customise it to suit your environment)
3. Save 

```
"files.associations": {
	"**/diagnostic_snapshot_*/var/log/**.log*": "pexip"
}
```
 
Install the extension 

Grab the latest VSIX from the [releases](https://github.com/darrengoulden/vsc-pexiplogs-extension/releases) section then in VSCode;
1. Using the Install from VSIX command in the Extensions view command dropdown
2. or the `Extensions: Install from VSIX` command in the Command Palette (⇧⌘P or Ctrl+Shift+P), point to the `.VSIX` file.  

## Release Notes  

* 0.0.9: Pattern match additions
* 0.0.8: Pattern match additions and add support for pexauth and pexidp
* 0.0.7: Pattern match additions
* 0.0.6: Pattern match additions
* 0.0.5: Pattern match additions
* 0.0.4: Update strings for Kebab-Case (per https://docs.pexip.com/admin/whats_new.htm#other or https://docs.pexip.com/v29/admin/whats_new.htm#other)
* 0.0.3: Pattern match additions
* 0.0.2: Pattern match additions
* 0.0.1: Minor Release
