#### Most used DOS Commands
```
systeminfo
winver
```
#### DOS command to delete bin & obj Folders
```
@echo off
@echo Deleting all BIN and OBJ folders...
for /d /r . %%d in (bin,obj) do @if exist "%%d" rd /s/q "%%d"
@echo folders have been deleted. Press any key to exit
pause > nul
```

#### DOS command Number of Lines in Txt File in folders, subfolders
```
for /r %f in (*.txt) do find /v /c "" "%f" >>externalref.txt
```

#### DOS Command to clear Event Logger
```
for /F "tokens=*" %1 in ('wevtutil.exe el') DO wevtutil.exe cl "%1
```

#### DOS Command to kill node process
```
taskkill /F /IM node.exe
```
