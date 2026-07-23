# 📱 Experiment 1: Hello World Android Application

## 🎯 Objective

To develop a basic Android application using Android Studio that displays the following information on the screen:

- Hello World
- USN: 25MCAR120
- This is my first program.

---

# 📖 Introduction

Android is an open-source mobile operating system developed by Google for smartphones, tablets, wearables, televisions, and other smart devices. Android applications are primarily developed using Android Studio, the official Integrated Development Environment (IDE), with Java or Kotlin as the programming language.

The **Hello World** application is traditionally the first program created while learning any new programming language or development framework. This experiment helps students understand the basic structure of an Android project, XML-based user interface design, and application execution on an Android Emulator.

---

# 🛠️ Technology Used

- **Android Studio**
- **Kotlin** *(Replace with Java if your project uses Java)*
- **XML**
- **Android SDK**
- **Gradle (Kotlin DSL)**

---

# 💡 Concept

Android applications separate the user interface from the application logic.

- The **XML layout file (`activity_main.xml`)** defines the user interface.
- The **MainActivity** acts as the entry point of the application.
- A **TextView** widget is used to display static text.
- When the application starts, Android launches the `MainActivity`, inflates the XML layout, and displays the predefined text on the screen.

---

# 🌍 Scenario

A beginner developing their first Android application wants to verify that the Android development environment is correctly configured.

This application simply displays:

- Hello World
- Student USN
- A message indicating that it is the first Android program

Running the application successfully confirms that Android Studio, the Android SDK, and the Emulator are properly configured.

---

# 📂 Project Structure

```text
prg1/
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── com/example/prg1/
│           │       └── MainActivity.kt
│           ├── res/
│           │   └── layout/
│           │       └── activity_main.xml
│           └── AndroidManifest.xml
├── images/
├── README.md
├── build.gradle.kts
└── settings.gradle.kts
```

> **Note:** If your project uses Java, replace `MainActivity.kt` with `MainActivity.java`.

---

# 📸 Screenshots

## Final Output

![Screenshot 1](images/Screenshot%202026-07-23%20110004.png)

![Screenshot 2](images/Screenshot%202026-07-23%20110441.png)

![Screenshot 3](images/Screenshot%202026-07-23%20110721.png)

---

# 📄 Source Code

## activity_main.xml

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:gravity="center"
    android:orientation="vertical">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World"
        android:textSize="24sp"/>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="USN: 22MCAR120"
        android:textSize="20sp"/>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="This is my first program."
        android:textSize="18sp"/>

</LinearLayout>
```

---

## MainActivity.kt

```kotlin
package com.example.prg1

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity

class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
    }
}
```

> **If your project is written in Java, replace this section with `MainActivity.java`.**

---

# ▶️ Steps to Run the Application

1. Open the project in **Android Studio**.
2. Allow Gradle to synchronize.
3. Connect an Android device or start an Android Emulator.
4. Click the **Run** ▶️ button.
5. Wait for the application to build and install.
6. Observe the output displayed on the emulator.

---

# ✅ Output

When the application is executed successfully, the following text is displayed:

```text
Hello World

USN: 25MCAR120

This is my first program.
```

---

# 🎓 Learning Outcomes

After completing this experiment, the following concepts were understood:

- Android project structure
- Android Studio development environment
- XML-based user interface design
- Working with the TextView widget
- Android Activity lifecycle
- Running applications on an Android Emulator
- Building and executing Android applications using Gradle

---

# 📌 Conclusion

The experiment was successfully completed by developing and executing a basic Android application using Android Studio. The application displayed the required text on the Android Emulator, confirming that the Android development environment was properly configured. This experiment provided a strong foundation for understanding Android project structure, XML layouts, and Activity-based application development.

---

# 👨‍💻 Author

**Name:** Shubham Pandey

**USN:** 25MCAR120

**Course:** Master of Computer Applications (MCA)

**Subject:** Mobile Application Development

**Experiment No.:** 1

**Experiment Title:** Hello World Android Application

---

## ⭐ Repository

If you found this project helpful, consider giving it a ⭐ on GitHub.