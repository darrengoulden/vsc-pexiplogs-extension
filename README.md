# Pexip Log Syntax  

VSCode extension for Pexip log syntax highlighting. 
Tested with the Dark+ VSC theme.  

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