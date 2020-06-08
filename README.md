# python-wiki

### Basics

#### Löscht überflüssige Leerzeilen
```
fileContent = "".join([s for s in fileContent.splitlines(True) if s.strip("\r\n")])
fileContent = os.linesep.join([s for s in fileContent.splitlines() if s])
```

### Sonstiges

#### PIP mit Proxy
```
pip3 --proxy=http://163.241.128.141:80 install ...
```

#### All Deps from Package
```
download [package] -d /tmp --no-binary :all: -v
```
