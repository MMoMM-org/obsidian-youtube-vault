## Update Better Word Count

Hat wieder seine volle Funktionalität.

Und soll noch mehr bekommen, es gibt dann eine neues Video.

## Todoist App

https://todoist.com/

## Todoist Sync Plugin

### Todoist API Token

https://todoist.com/prefs/integrations

### Todoist Sync Beispiele

```todoist
{
"name": "Alle Tasks",
"filter": "today | overdue",
"group": true
}
```

```todoist
{
"name": "Private Nicht Obsidian Tasks",
"filter": "(today | overdue) & #Privat & !@Obsidian"
}
```


## Todoist mit Buttons

```button
name Create New Todoist Task
type link
class obsidian-button
action todoist://addtask
```
```button
name Open Todoist Privat Project
type link
class obsidian-button
action todoist://project?id=123123123
```

