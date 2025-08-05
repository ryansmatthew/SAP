curl -L --progress-bar -o SAP.zip "https://github.com/ryansmatthew/SAP/releases/download/SAP8/SAPGUI.exe"

Start-Process -FilePath "SAPGUI_20250805_1443.exe" -ArgumentList '/Silent /Package="SAPGUI"' -Wait
Write-Output "Cài đặt đã hoàn tất!"

