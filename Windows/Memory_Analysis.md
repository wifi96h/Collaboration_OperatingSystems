# Installing Notepad++
```
PS C:\windows\system32> invoke-webrequest -uri "https://github.com/notepad-plus-plus/notepad-plus-plus/releases/download/v7.8.8/npp.7.8.8.Installer.x64.exe" -outfile "C:\npp.7.8.8.Installer.x64.exe" 
PS C:\windows\system32> cd C:\ 
PS C:\> start-process npp.7.8.8.Installer.x64.exe -ArgumentList '/S'
```

# Installing Volatility
Use Powershell for all steps

```
invoke-webrequest -uri "http://downloads.volatilityfoundation.org/releases/2.6/volatility_2.6.win.standalone.zip" -outfile "C:\Users\andy.dwyer\Desktop\Memory_Analysis\volatility_2.6_win64_standalone.zip"
```
Download standalone zip

```
Expand-Archive "C:\Users\andy.dwyer\Desktop\Memory_Analysis/volatility_2.6_win64_standalone.zip" "C:\Users\andy.dwyer\Desktop\Memory_Analysis\volatility_2.6_win64_standalone"
```
Unzip file

```
mv "C:\Users\andy.dwyer\Desktop\Memory_Analysis\volatility_2.6_win64_standalone\volatility_2.6_win64_standalone.exe" "C:\Users\andy.dwyer\Desktop\Memory_Analysis\volatility_2.6_win64_standalone.exe"
```
Moves executable to Memory Analysis folder