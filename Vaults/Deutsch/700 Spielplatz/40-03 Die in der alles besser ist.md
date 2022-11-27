# Plugins mit Better im Namen

[Better CodeBlock (Plugin)](app://obsidian.md/Better%20CodeBlock%20(Plugin))  
[Better Word Count (Plugin)](app://obsidian.md/Better%20Word%20Count%20(Plugin))  
[Better File Link (Plugin)](app://obsidian.md/Better%20File%20Link%20(Plugin))  
[Better Inline Fields (Plugin)](app://obsidian.md/Better%20Inline%20Fields%20(Plugin))


## Better Code Block

### Task

Check if there is an active file in the editor.

### Code
```javascript
const currentFile = app.workspace.getActiveFile()
if (!currentFile) {
	return new Notice("No active file");
	}
await app.plugins.plugins.metaedit.api.createYamlProperty("alias", currentFile.basename, currentFile)
```

### Better Code Block Advanced
```javascript TI: "Check for active file" HL:"2-4" "FOLD"
const currentFile = app.workspace.getActiveFile()
if (!currentFile) {
	return new Notice("No active file");
	}
await app.plugins.plugins.metaedit.api.createYamlProperty("alias", currentFile.basename, currentFile)
```

## Better Word Count

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

## Better File Link


## Better Inline Field

Sport:: true

Spielplatz:: [[40-02 Helfer beim Schreiben + Backup]]
