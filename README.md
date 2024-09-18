Here’s an updated, more user-friendly guide to installing Flutter on macOS with icons for better readability!

---

### 🚀 Step-by-Step Guide to Install Flutter on macOS

---

#### 1. 🖥️ **Install Rosetta (For Apple Silicon Macs Only)**  
If you're on an Apple Silicon Mac (M1/M2 chip), install Rosetta for compatibility:

- Open **Terminal** and run:
  ```bash
  sudo softwareupdate --install-rosetta --agree-to-license
  ```

> **Note:** Intel-based Mac users can skip this step.

---

#### 2. 🛠️ **Install Android Studio**  
You need Android Studio for developing Android apps. Download it [here](https://redirector.gvt1.com/edgedl/android/studio/install/2024.1.2.12/android-studio-2024.1.2.12-mac.dmg).

##### 🔧 **Verify Required Android Components:**

1. Open **Android Studio**.
2. Navigate to **Tools** > **SDK Manager** (or from the **Welcome Screen**, click the **More Options** icon and select **SDK Manager**).
3. In the **SDK Platforms** tab, ensure the following are installed:
   - **Android SDK Command-line Tools**
   - **Android SDK Build-Tools**
   - **Android SDK Platform-Tools**
   - **Android Emulator**
4. If any components show as **Not installed**, select and install them by clicking **Apply** and **OK**.
5. When finished, click **Finish**.

##### 📱 **Set Up an Android Emulator:**
1. In Android Studio, go to **Virtual Device Manager**.
2. Click **Create Device**, then follow the instructions to set up your emulator.

---

#### 3.  **Install Xcode (For iOS Development)**  
To build iOS apps, download and install Xcode from the Mac App Store.  
Search for **Xcode** in the store and download it.

---

#### 4. 📦 **Download and Install the Flutter SDK**  
Get the latest Flutter SDK:

- For Intel-based Macs: [Download Flutter SDK](https://docs.flutter.dev/get-started/install/macos#install-flutter-sdk)
- For Apple Silicon Macs: [Download Flutter SDK](https://docs.flutter.dev/get-started/install/macos#install-flutter-sdk)

---

#### 5. 🛤️ **Add Flutter to Your PATH**

So that Flutter commands are accessible globally on your Mac, add Flutter to your system’s PATH:

1. Open **Finder**.
2. Go to your **Home** folder.
3. Press `Cmd + Shift + .` to show hidden files.
4. Open the `.zshrc` (or `.zshenv`) file with a text editor.
5. Add this line at the end of the file (replace `development` with your Flutter SDK path):
   ```bash
   export PATH="$HOME/development/flutter/bin:$PATH"
   ```
6. Save and close the file.

---

#### 6. ✅ **Verify Flutter Installation**

Check if Flutter is properly set up on your system. Open **Terminal** and run:

```bash
flutter doctor
```

This will identify any missing dependencies or issues in your setup.

---

#### 7. 📄 **Accept Android Licenses**

Run this command to accept the required Android licenses:

```bash
flutter doctor --android-licenses
```

Follow the on-screen instructions to accept all licenses.

---

🎉 **All Done!**  
You’re now ready to create Flutter apps on macOS. To start your first project, run:

```bash
flutter create my_app
```
