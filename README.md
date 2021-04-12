# InstallWindowsService
Who to Install Windows Service

sc create NameWs binPath="C:\xxxx\yyyyy\zzzzz.exe" displayname="display name"  start=auto
sc description NameWs "description text"
sc config NameWs obj="username" password="xxx"
sc failure NameWs reset=30 actions=restart/5000
