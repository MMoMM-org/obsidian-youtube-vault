# Buttons

## Beispiele

### Befehl
z.B. Öffene den Graph View
```button
name GraphView
type command
action Graph view: Open graph view
```
^button-10w1

und das gleiche nochmal in Blau

```button
name GraphView
type command
action Graph view: Open graph view
color blue
```

### Link

Notiz von [[@Tom]] öffnen

```button
name Tom
type link
action obsidian://open?vault=Deutsch&file=600%20Ressourcen%2F601%20Personen%2F%40Tom
```
^button-ln5i

### Rechnen

```button
name 2+2
type calculate
action 2+2
```
^button-2

Result: 4

5  
4

```button
name Wieviele Bananen habe ich noch?
type calculate
action $45-$46
color yellow
```
^button-banana

Result: 1


5 Hunde plus 2 Katzen divided by 2 Leute

```button
name Wieviel Tiere sind es?
type calculate
action $59
color red
```
^button-pet

Result: 6

### Swap

```button
name Verrückter Wechsel Knopf
swap [2,banana,pet]
```
^button-swap

`button-swap` 
 
> [!NOTE] Wenn's anders nicht geht
> `button-swap`

Hier ^^^^^^^ gibt es aber ein kleiner Problem bei diesem Beispiel.

```button
name Geht schon 😀
type link
action obsidian://open?vault=Deutsch&file=700%20Spielplatz%2F40-06%20Buttons-Dynbedded
```

#### Swap-Dynbedded

`button-swap` 

### Text & Template

Euch stehen die folgenden Möglichkeiten zur Verfügung:
- Prepend: Fügt vor dem Button den Text / das Template ein
- Append: Fügt nach dem Button den Text / das Template ein
- Add at Line: Fügt an einer bestimmten Stelle den Text / das Template ein
- New Note: Erstellt eine neue Notiz mit dem Inhalt des Textes / Templates.

#### Append
```button
name Log
type append text
action Text goes here
```
^button-log

```button
name Log2
type line(117) text
action Hallo
```
^button-qaxa
Hallo
Hallo
Hallo


#### Add at Line
```button
name Aktuelles Wetter
type line(69) template
action Weather Template
```

```button
name Wetter2
type append template
action Weather Template
```
^button-wk37

Draussen gibt es Wetter

Draussen gibt es Wetter

Draussen gibt es Wetter



#### New Note
```button
name Neues Meeting
type note(Meeting) template
action Meeting Template
```
^button-inherit

```button
name Neues Meeting in neuer Spalte
type note(Meeting-Split, split) template
action Meeting Template
```


## Erweiterte Beispiele

#### Remove

Result: 4

Result: 4

#### Replace


#### Inherit

```button
name Gurken?
type calculate
id banana
color green
```
^button-co1d

Result: 1

Wäre auch eine Möglichkeit Standard Buttons zu erzeugen 😀

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

### Buttons nebeneinander

```button
name Eins
type command
action New tab
```
^button-eins

```button
name Zwei
type command
action New tab
```
^button-zwei

```button
name Drei
type command
action New tab
```
^button-drei

#### EinsBisDrei

`button-eins` `button-zwei` `button-drei`

```button
name Geht schon 😀
type link
action obsidian://open?vault=Deutsch&file=700%20Spielplatz%2F40-06%20Buttons-Dynbedded
```
^button-dynbedded

### Buttons in Spalten

```button
name Lesemodus
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

