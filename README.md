# auto-snap
CEP extension for Auto Snap
**Step 1: Unlock CEP (One-Time Setup)**
Open PowerShell and run this command so Illustrator allows your custom panel:

**PowerShell**
`Set-ItemProperty -Path "HKCU:\Software\Adobe\CSXS.11" -Name "PlayerDebugMode" -Value "1" -Type String; Set-ItemProperty -Path "HKCU:\Software\Adobe\CSXS.12" -Name "PlayerDebugMode" -Value "1" -Type String`

(If it says a path doesn't exist, just create it first with New-Item -Path "`HKCU:\Software\Adobe\CSXS.11`" -Force and CSXS.12, then re-run.)

**Step 2: Create the Plugin Folder**
Go to:
`C:\Users\<YourName>\AppData\Roaming\Adobe\CEP\extensions\`

Create a folder named LogoGridSnap with these 4 files inside:

**Plaintext**
LogoGridSnap/
├── CSXS/
│   └── manifest.xml
├── index.html
├── main.js
└── host.jsx
