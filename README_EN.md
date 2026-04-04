# 🚗 BYD Unlocking Guide (Han / Seal / Seal U / DM-i)

> [!WARNING]
> **DISCLAIMER:** I take no responsibility for any actions taken on your BYD vehicle; you proceed at your own risk. Do not install APK files from untrusted sources. Modifying the system may void your manufacturer's warranty regarding the infotainment system.

**🌍 Language / Język**
* **English Version** (current)
* [Polska Wersja (README.md)](README.md)

**✅ Compatible Models:** This method works on models (Han, Atto 3, Seal, Seal U, and DM-i).

---

**📅 Status as of:** 28.03.2026  
**💡 Inspiration:** Abdulkadir Kartal

---

## 🛠 SECTION A: Downgrade (Installing an older version)

To unlock the system, you must first install a software version that contains a vulnerability allowing ADB protocol access.

> [!NOTE]
> If an SD card is in the vehicle during this procedure, an error message will appear; therefore, you should remove the SD card and start the procedure with the card removed.

### 1. Preparation
* **Version Verification**: Ensure your current version starts with `13.1.33.XXXX` (e.g., `13.1.33.2511`). Check this in: `Settings` ➔ `System` ➔ `Version`.
* **Download**: Download version [13.1.33.2404](https://drive.google.com/file/d/1awJk8OgAMT_z3DHve5cFFUzfH7viOVfT/view?usp=sharing), which enables the unlocking.
* **USB Drive**: Use an **8 GB / 16 GB / 32 GB** drive formatted as **FAT32**. For larger drives, use **exFAT**.
* **File Structure**: Create the following folders on the USB drive: `BYDUpdatePackage` ➔ `msm8953_64` ➔ `UpdateFull.zip` (The last one is the file we downloaded).
* **File Naming**: Place the downloaded file into the last folder and rename it to **UpdateFull.zip**.

> [!CAUTION]
> **IMPORTANT:** Before starting, ensure your traction battery charge is at least **30%**. Do not turn off the vehicle during the update process!

### 2. Installation Procedure
1. Turn on the vehicle and insert the prepared USB drive (use a USB-A to USB-C adapter if your car only has USB-C ports).
2. When the **QR Code** appears on the screen, press and hold for **10 seconds** simultaneously:
   * **Left Arrow** on the steering wheel (Back button).
   * **Volume Roller/Button** (located next to the gear selector).
   <img width="1187" height="279" alt="image" src="https://github.com/user-attachments/assets/ec2b5cce-7caa-4fa8-bfb6-ef9648c7887c" />
3. The process usually takes **10–20 minutes**. Once finished and the screen reboots, remove the USB drive.

---

## 🔓 SECTION B: ADB Access

### 1. Enabling DEBUG Mode (ADB)
1. Pair your phone with the car’s multimedia system via **Bluetooth**.
2. Open the `Phone` app in the car and dial the code: `*#91532547#*`.
3. Note down the **last 6 digits of the IMEI number** that appears on the screen.
4. Go to [ahmada3mar.github.io/BYD/](https://ahmada3mar.github.io/BYD/) (on your phone/PC) and generate a password using those 6 digits.
5. Enter the generated password on the car's tablet and confirm with the bottom-right button (labeled with Chinese characters `确定`).
6. In the `Test Tools` menu, scroll down and enable:
   * ✅ `Wireless adb debug switch`
   * ✅ `Debug mode when USB is connected`
   <img width="748" height="291" alt="image" src="https://github.com/user-attachments/assets/44ff06ae-b885-4b87-9c77-40ccf7541614" />
   <img width="967" height="291" alt="image" src="https://github.com/user-attachments/assets/7bfefb51-9f4d-4612-a54a-bc9564f79ee1" />

---

## ⤵️ SECTION C: App Installation

### 1. Wireless Method (Bugjaeger App)
1. Enable a **WiFi Hotspot** on your phone and connect the car to it.
2. In the car's WiFi settings, tap the `i` icon next to the network name and note the vehicle's **IP Address**.
   <img width="893" height="306" alt="image" src="https://github.com/user-attachments/assets/62e98164-78c2-4d0c-ba52-881b3119a776" />
3. In the **Bugjaeger** app (on your phone), tap the plug icon (`+`), enter the car's IP and port `5555`, then click `Connect`.
4. **Accept the connection** on the car's screen (check `Always allow` and click `Allow`).
5. Install the [PackageInstallerUnlocker.apk](https://drive.google.com/file/d/1aoWeo-XZFAiJkM3-cptNwGVxZuNtRbis/view?usp=drive_link). From now on, the system will allow native APK installations.

### 2. Traditional Method (USB Drive)
1. Copy your chosen APK files directly to the root folder of a USB drive (FAT32/exFAT).
2. Insert the USB drive into the car's USB port.
3. Open the built-in `File Manager` app and install your apps directly from the drive.

---

## 📦 Recommended Apps
* ⚡ [Electro](https://electro.app.br/): Advanced vehicle data and battery statistics.
* 🌌 [AuroraStore](https://drive.google.com/file/d/1leQ-cinJ0gSUhrYMBQZQlGwhv2g1pXsM/view?usp=sharing): A safe alternative to the Google Play Store.
* 🛠 [MicroG](https://drive.google.com/file/d/1tY5HX0U_q7cOxFQpiPefZWRIWTlG6NQi/view?usp=sharing): Required for Google services. (In settings: disable device registration, log in, and disable AutoStart in system tools).
* 📺 [Revanced Manager](https://drive.google.com/file/d/1zjbrAkGXbFAT36nsOZx98l_E_BD44Mvz/view?usp=sharing): YouTube without ads and with background playback.

---

## ⬆️ SECTION D: System Update (OTA)

After successfully unlocking and installing your apps, you can safely update back to a newer system version. Your installed apps will remain active.

1. **Recommended Versions**:
   * **[13.1.33.2511](https://drive.google.com/file/d/1TmPu7NKAuGVmCHNG6iFmebZRe3Pk1XRa/view?usp=sharing)** – Most stable version.
   * **[13.1.33.2602](https://drive.google.com/file/d/1E02Lzp_Gccb9rsEMeGqV3jNhllysXCH2/view?usp=sharing)** – Latest version (includes navigation improvements, though stability may vary).
2. **Procedure**: Prepare the USB drive exactly as in Section A and select the `Upgrade OTG` option on the screen. During the update (**approx. 15 minutes**), do not press any buttons.
