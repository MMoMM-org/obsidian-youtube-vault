# Buttons

## Examples

### Command
e.g. Open the graph view
```button
name Graph
type command
action Graph view: Open graph view
```
^button-unng

And the same in blue

```button
name Graph
type command
action Graph view: Open graph view
color blue
```

### Link

Open [[@Tom]] note

```button
name Tom
type link
action obsidian://open?vault=English&file=600%20Resources%2F601%20People%2F%40Tom
```
^button-lri8

### Caluclate

```button
name 2+2
type calculate
action 2+2
```
^button-2

Result: 4

I had how many bananas: 5  
Bananas I have lost: 4

```button
name How many bananas do I have?
type calculate
action $45-$46
color yellow
```
^button-banana

Result: 1


5 dogs  plus 2 cats divided by 2 people

```button
name How many pets do we have?
type calculate
action $59
color red
```
^button-pet

Result: 6

### Swap

```button
name Crazy Swap Button
swap [2,banana,pet]
```
^button-swap

`button-swap` 
 
> [!NOTE] Wenn's anders nicht geht
> `button-swap`

There ^^^^^^^ is a small problem with this example though

```button
name Just works 😀
type link
action obsidian://open?vault=English&file=700%20Playground%2F40-06%20Buttons-Dynbedded
```

#### Swap-Dynbedded

`button-swap` 

### Text & Template

You can do the following things:
- Prepend: Prepend text / template in front of the button
- Append: Append text / template behind the button
- Add at Line: Adds text / template at a certain line
- New Note: Create a new note with text / template

#### Append
```button
name Log
type append text
action Text goes here
```

```button
name Log2
type append template
action Log Template
```
Ein Log Template

There is weather outside

#### Add at Line
```button
name The Weather
type line(118) template
action Weather Template
```

#### New Note
```button
name New Meeting
type note(Meeting) template
action Meeting Template
```

```button
name New Meeting in new column
type note(Meeting-Split, split) template
action Meeting Template
```


## Advanced Examples

#### Remove


Ein Log Template



#### Replace



#### Inherit

```button
name Cucumbers?
id banana
color green
```
^button-co1d

Result: 1

Another way to create a standard button 😀

#### Class

```button
name Who Get The Pets?
type calculate
action $1
class button-red
```

### Templater

```button
name Make an Hourly Note
type note(<% tp.date.now("HH[_]mm") %>,split) template
action Log Template
templater true
```


## Tips & Tricks

### Buttons next to each other

```button
name One
type command
action New tab
```
^button-one

```button
name Two
type command
action New tab
```
^button-two

```button
name Three
type command
action New tab
```
^button-three

#### OnetoThree

`button-one` `button-two` `button-three`

```button
name Just Works 😀
type link
action obsidian://open?vault=English&file=700%20Playground%2F40-06%20Buttons-Dynbedded
```
^button-dynbedded

### Buttons in columns

```button
name Read Modus
type command
action Toggle reading view
```
^button-p9zw

```start-multi-column  
ID: DashboardRegion1  
number of columns: 2  
Largest Column: standard
```
#### Get Going

```button
name Open Todays Note
type command
action Daily notes opener: Open today's daily note in new pane
color grey
```

```button
name Open 5 Year Journal
type link
action obsidian://vault/Deutsch/5J-2023-01-31
templater true
color grey
```

```button
name Open Dayplanner
type link
action obsidian://vault/Deutsch/DP-2023-01-31
templater true
color grey
```

```button
name Open a Zettelkasten Note
type command
action Spaced Repetition: Notiz zur Wiederholung öffnen
```


--- end-column ---
#### Todoist


```button
name Create New Todoist Task
type link
class obsidian-button
action todoist://addtask
class button-red
```
```button
name Open Todoist Privat Project
type link
class obsidian-button
action todoist://project?id=1234123
class button-red
```
```button
name Open Todoist Work Project
type link
class obsidian-button
action todoist://project?id=12341234
class button-red
```

=== end-multi-column

### Standard Buttons

```button
name Standard Button
type link
id dynbedded
```
^button-17wh

