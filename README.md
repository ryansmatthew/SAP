curl -L --progress-bar -o SAP.zip "https://github.com/ryansmatthew/SAP/releases/download/SAP8/SAPGUI.exe"

Start-Process -FilePath "SAPGUI.exe" -ArgumentList '/Silent /Package="SAPGUI"' -Wait; Write-Output "Done!"


