curl -L --progress-bar -o SAP.zip "https://github.com/ryansmatthew/SAP/releases/download/SAP8/SAP8.zip"

powershell -Command "Expand-Archive -Path 'SAP.zip' -DestinationPath 'SAP' -Force"

cd SAP\Win32\Setup\

NwSapSetup.exe /Silent /Install /Product="SAPGUI"
