## MAD-lab exp-5

# 📱 Android Notification Application

An Android application developed using **Kotlin** and **Android Studio** to demonstrate how to create and display notifications.

## 🎯 Aim

To develop an Android application that displays a notification when the user clicks a button.

## 📌 About the Project

This project demonstrates the basic implementation of **Android Notifications** using:

* `NotificationManager`
* `NotificationChannel`
* `NotificationCompat.Builder`
* `PendingIntent`
* `Intent`

When the user clicks the **Show Notification** button, the application creates and displays a notification in the device's notification panel.

## 🛠️ Technologies Used

| Technology     | Usage               |
| -------------- | ------------------- |
| Kotlin         | Application logic   |
| XML            | User Interface      |
| Android Studio | Development IDE     |
| Android SDK    | Android development |

## ✨ Features

* Simple and clean user interface
* One-click notification generation
* Notification title and message
* Notification channel support
* Auto-cancel notification
* Compatible with modern Android versions

## 📂 Project Structure

```text
NotificationApp/
│
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── MainActivity.kt
│           │
│           ├── res/
│           │   ├── layout/
│           │   │   └── activity_main.xml
│           │   └── values/
│           │
│           └── AndroidManifest.xml
│
├── build.gradle.kts
├── settings.gradle.kts
└── README.md
```

## ⚙️ How It Works

1. Launch the application.
2. The main screen displays a **Show Notification** button.
3. Click the button.
4. The application creates a notification channel.
5. A notification is generated using `NotificationCompat.Builder`.
6. `NotificationManager` displays the notification.
7. The notification appears in the Android notification panel.

## 🔔 Sample Notification

**Title:** Notification

**Message:** Hello! This is an Android notification.

## 💻 Basic Implementation

```kotlin
val notification = NotificationCompat.Builder(this, CHANNEL_ID)
    .setSmallIcon(android.R.drawable.ic_dialog_info)
    .setContentTitle("Notification")
    .setContentText("Hello! This is an Android notification.")
    .setPriority(NotificationCompat.PRIORITY_DEFAULT)
    .setAutoCancel(true)
    .build()

NotificationManagerCompat.from(this)
    .notify(1, notification)
```

## 🚀 How to Run

1. Clone this repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

2. Open the project in **Android Studio**.
3. Allow Gradle to sync.
4. Connect an Android device or start an emulator.
5. Click **Run ▶**.
6. Press **Show Notification** to test the application.

## 📸 Output

The application displays a notification in the Android notification panel after clicking the button.

## screenshots 

<img width="1906" height="985" alt="Screenshot 2026-08-27 014521" src="https://github.com/user-attachments/assets/7afa68cf-32b2-4dcb-ad12-0bbc391b59a7" />
<img width="1905" height="978" alt="Screenshot 2026-08-27 014603" src="https://github.com/user-attachments/assets/fd0a1955-302e-46a8-aa9a-e4f277cafd05" />

<img width="1882" height="961" alt="Screenshot 2026-08-27 014631" src="https://github.com/user-attachments/assets/d67da4dc-8f11-49e3-94f8-b4020c0c5fdc" />


## 📚 Learning Outcomes

After completing this project, you will understand:

* How Android notifications work
* How to create a Notification Channel
* How to use `NotificationCompat.Builder`
* How to use `NotificationManager`
* How to handle notification actions

## 👨‍💻 Author

**Sonu Jha**

## 📄 License

This project is created for **educational and academic purposes**.
