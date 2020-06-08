# python-wiki

### Basics

##### Start-Methode
```
if __name__ == '__main__':
    main()
```

##### Dateinamen auslesen
```
fileWithExt = os.path.basename(f)
fileWithoutExt = os.path.splitext(fileWithExt)[0]
fileExt = os.path.splitext(fileWithExt)[1]
```

##### Ordner-Elemente auslesen
```
os.listdir(folderPath)
```

##### Pfad auf Ordner prüfen
```
os.path.isdir(objectpath)
```

##### Pfade zusammenfügen
```
os.path.join(path1, fileWithExt)
```

##### Löscht überflüssige Leerzeilen
```
fileContent = "".join([s for s in fileContent.splitlines(True) if s.strip("\r\n")])
fileContent = os.linesep.join([s for s in fileContent.splitlines() if s])
```

##### Listeneinträge getrennt mit Zeilenumbruch in String speichern
```
mySting = '\n'.join(listOfFiles)
```

##### Datei zeilenweise auslesen und in Liste speichern
```
with open(donetaskspath, encoding='utf8') as f:
        listOfDoneTasks = f.read().splitlines()
```
##### Anzahl Elemente in Liste
```
countElements = len(listOfFiles)
```

##### Element einer Liste hinzufügen
```
result.append(objectpath)
```

##### Differenz aus zwei Listen auslesen
```
todo = list(set(listOfTasks) - set(listOfDoneTasks))
```

##### DateTime in String speichern
```
dateTime = datetime.datetime.now().strftime("%Y-%m-%d_%H.%M")
```

##### Funktion erstellen
```
def myFunction(para):
    ...
    return result
```

##### if / if not Beispiel
```
if var:
    ...
if not var:
    ...
```

##### For-Schleife mit vorgegebenen Range
```
for i in range(10):
    ...
```

##### Error-Handling
```
try:
    ...
except Exception as e:
    print("Error: " + e)
```

### Sonstiges

##### PIP mit Proxy
```
pip3 --proxy=http://163.241.128.141:80 install ...
```

##### All Deps from Package
```
download [package] -d /tmp --no-binary :all: -v
```
