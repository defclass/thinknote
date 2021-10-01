## Installation

Requirement:  macOS above 11.0

As I did't register the Apple developer account, the app is not signed. There might be some errors when you open the APP.

Try right click the APP -> Open ThinkNote.app

1. If encount this error：“ThinkNote.app is damaged and can’t be opened. You should move it to the Trash”

You may check the option   -> System Preference -> Security & Privacy -> Allow apps downloaded from:  Anywhere.

If there is no such option, try below command.

```
sudo spctl --master-disable
```

then check if the 'Anywhere' option exist.

2. If encount this error：“ThinkNote.app” is damaged and can’t be opened. You should move it to the Trash.　Try open Terminal, type below command 

```
cd /path/to/ThinkNote.app/
xattr -r -c ThinkNote.app
```

then right click the APP -> Open ThinkNote.app

If you failed still，please DM me on Twitter：https://twitter.com/michaelwong666


## Data backup

ThinkNote use SQLite to pesistent data. The db directory locate in: 

~/Library/Containers/org.huangqian.ThinkNote/Data/Applications/thinknote.sqlite3

You can simplely backup the thinknote.sqlite3 file. 
