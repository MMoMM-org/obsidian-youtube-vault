## Update Better Word Count

Has gained back it's full functionality.

There is more to come at which time I will do another video.

## Todoist App

https://todoist.com/

## Todoist Sync Plugin

### Todoist API Token

https://todoist.com/prefs/integrations

### Todoist Sync Examples

```todoist
{
"name": "All Tasks",
"filter": "today | overdue",
"group": true
}
```

```todoist
{
"name": "Privat Non Obsidian Tasks",
"filter": "(today | overdue) & #Privat & !@Obsidian"
}
```


## Todoist with Buttons

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

