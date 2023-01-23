# Netcat

### Netcat download: https://eternallybored.org/misc/netcat/

Into your CMD to listen:
1. ``cd C:\Users\De Lucca\Downloads\netcat-win32-1.12`` => Path where your extracted netcat file is
2. ``nc.exe -lvp [Port]`` => Listen, Verbose, Port

Into your CMD to listen while executing CMD:
1. ``nc.exe -lvp [Port] -e "cmd.exe"``

Into your CMD to connect:
1. ``cd C:\Users\De Lucca\Downloads\netcat-win32-1.12`` => Path where your extracted netcat file is
2. ``nc.exe [IP] [Port]``
