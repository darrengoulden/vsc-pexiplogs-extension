# Pexip Log Syntax  

VSCode extension for Pexip log syntax highlighting.  
Tested with the `Dark+` VSC theme.  

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

Grab the latest VSIX from the [releases](https://github.com/darrengoulden/vsc-pexiplogs-extension/releases) section then;
1. Using the Install from VSIX command in the Extensions view command dropdown
2. or the `Extensions: Install from VSIX` command in the Command Palette (⇧⌘P or Ctrl+Shift+P), point to the .vsix file.

## Config adjustments  

All configured patterns are enabled by default, if you want to add or remove one you can edit the `syntaxes/pexip.tmLanguage.json` file in the extension folder which is located in one of the below depending on your platform. 
 - Windows `%USERPROFILE%\.vscode\extensions`
 - macOS `~/.vscode/extensions`
 - Linux `~/.vscode/extensions` 

For example, to remove `#dbsummary` includes, simply remove it from the patterns array whilst retaining the structure. 

Before;  

```
 	"patterns": [
		{
			"include": "#dbsummary"
		},
		{
			"include": "#mjxsummary"
		},
		...
	],
```  

After;  

```
 	"patterns": [
		{
			"include": "#mjxsummary"
		},
		...
	],
```  

## Release Notes  

* 0.0.2: Pattern match additions
* 0.0.1: Minor Release, Commit Message: Initial Commit and Build.