# 🚨 Women Safety App — SOS Alert System

<div align="center">

**A smart Android Women Safety application that sends instant SOS alerts with live GPS location — triggered just by shaking your phone.**

</div>

---

## 📌 Project Overview

The **Women Safety App** is an Android-based emergency assistance application developed in **Java & XML** using **Android Studio**. It is designed to provide quick help during unsafe situations by detecting a phone shake and automatically sending an SOS SMS with the user's live location to a pre-registered emergency contact — no buttons needed.

> 🔐 *Your safety, one shake away.*

---

## ✨ Features

| Feature | Description |
|---|---|
| 📳 **Shake Detection** | Detects device shake using accelerometer sensor |
| 📍 **Live Location** | Fetches real-time GPS coordinates via Google Fused Location Provider |
| 📩 **SOS SMS Alert** | Sends emergency message with a Google Maps link automatically |
| 👤 **Contact Registration** | User saves one emergency contact number |
| 🔔 **Foreground Service** | Runs continuously in the background with notification support |
| ⚡ **Instant Activation** | Shake → SMS sent in seconds |
| 🛡️ **Permission Handling** | Runtime permissions for SMS, Location & Notifications |

---

## 🛠️ Tech Stack

### Language & UI
- **Java** — Application logic
- **XML** — UI layouts and design

### Android Components
- Activities
- Foreground Service
- SharedPreferences
- Notifications & Notification Channels
- Snackbar

### APIs & Libraries
- Google Fused Location Provider
- Shake Detector Library
- SMS Manager API

---

## 📂 Project Structure

```
wsafety/
├── app/
│   └── src/
│       ├── main/
│       │   ├── java/com/vinayak09/wsafety/
│       │   │   ├── MainActivity.java           # Home screen & service control
│       │   │   ├── RegisterNumberActivity.java # Emergency contact registration
│       │   │   ├── ServiceMine.java            # Foreground service & SOS logic
│       │   │   └── SplashScreen.java           # Splash screen activity
│       │   ├── res/
│       │   │   ├── layout/                     # XML UI layouts
│       │   │   ├── drawable/                   # Icons and images
│       │   │   ├── values/                     # Colors, strings, styles
│       │   │   └── menu/                       # Menu resources
│       │   └── AndroidManifest.xml
│       ├── androidTest/
│       └── test/
├── build.gradle
├── proguard-rules.pro
├── gradle/wrapper/
├── gradlew
├── gradlew.bat
└── settings.gradle
```

---

## 📌 How It Works

```
📱 App Opened
      ↓
🌟 Splash Screen
      ↓
👤 Register Emergency Contact Number
      ↓
▶️  Start Background Safety Service
      ↓
📳 Device Detects a Shake
      ↓
📍 GPS Location Fetched
      ↓
📩 SOS SMS Sent Automatically to Emergency Contact
```

---

## 📍 SOS Message Format

When the device is shaken, the following SMS is sent to the registered emergency number:

```
I'm in Trouble!
Sending My Location :
http://maps.google.com/maps?q=loc:<latitude>,<longitude>
```

---

## 🔑 Permissions Required

```xml
<uses-permission android:name="android.permission.SEND_SMS"/>
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>
<uses-permission android:name="android.permission.FOREGROUND_SERVICE"/>
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/SakshiOfficial27/Women-Safety-App.git
```

### 2️⃣ Open in Android Studio

- Open **Android Studio**
- Click **Open Existing Project**
- Select the cloned project folder

### 3️⃣ Sync Gradle

- Wait for Gradle build to finish
- Resolve any missing dependencies if prompted

### 4️⃣ Run the Application

- Connect an **Android device** or start an **emulator**
- Click ▶️ **Run**

---

## 📦 Dependencies

Add these to your `build.gradle (app)`:

```gradle
implementation 'com.google.android.gms:play-services-location:21.0.1'
implementation 'com.github.tbouron:shake-detector:1.0.0'
implementation 'com.google.android.material:material:1.11.0'
```

---

## 🔥 Key Concepts Used

### 📳 Shake Detection
Uses the mobile **accelerometer sensor** to detect sudden shake movements and trigger the SOS flow without any user interaction.

### 🔔 Foreground Service
A **foreground service** keeps the SOS detection active even when the app is minimized or the screen is off, ensuring the app is always ready.

### 💾 SharedPreferences
Used to **store the emergency contact number** locally on the device so it persists between sessions.

### 📍 Fused Location Provider
Google's **Fused Location Provider API** is used for accurate, battery-efficient real-time GPS tracking.

---

## 🚀 Future Enhancements

- [ ] 📞 Auto calling feature to emergency contacts
- [ ] 🎙️ Voice activation for SOS trigger
- [ ] 📸 Hidden camera capture during emergency
- [ ] ☁️ Firebase integration for cloud alerts
- [ ] 👮 Nearby police station detection
- [ ] 🌐 Real-time live tracking dashboard
- [ ] 👥 Multiple emergency contacts support
- [ ] 🔊 Siren/alarm alert system

---

## 🧠 Learning Outcomes

Through this project, the following Android development skills were practiced:

- ✅ Android App Development with Java
- ✅ Java & XML UI Design
- ✅ Foreground Services
- ✅ Runtime Permissions Handling
- ✅ SMS Sending via SmsManager
- ✅ GPS & Location Services
- ✅ Accelerometer Sensor Management
- ✅ Notification Channels

---

## 👩‍💻 Developed By

**Sakshi Chavhan**

Android & React Native Developer
Passionate about Mobile App Development | Interested in Safety-Based Applications

LinkedIn: https://www.linkedin.com/in/sakshi40765/ 
GitHub: https://github.com/SakshiOfficial27 
Email: chavhansakshi14@gmail.com


---

## 📄 License

This project is developed for **educational and learning purposes**.

---

<div align="center">
  <i>⭐ If this project helped you or inspired you, please give it a star on GitHub!</i><br><br>
  <b>🚨 Stay Safe. Stay Strong. 💪</b>
</div>
