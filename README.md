# 🚗 BYD Unlocking Guide (Han / Seal / Seal U / DM-i)

> [!WARNING]
> Nie biorę odpowiedzialności za żadne działania podejmowane w pojeździe BYD; użytkownik działa na własną odpowiedzialność. Nie instaluj plików APK z niepewnych źródeł. Pamiętaj, że modyfikacje systemu mogą wpłynąć na gwarancję producenta w zakresie inforozrywki.

**🌍 Język / Language**
* **Polska Wersja** (bieżąca)
* [English Version (README_EN.md)](README_EN.md)

**✅ Kompatybilne modele:** Ta metoda działa wyłącznie na modelach (Han, Seal, Seal U oraz DM-i).

---

**📅 Stan na:** 28.03.2026  
**💡 Inspiracja:** Abdulkadir Kartal

---

## 🛠 SEKCJA A: Downgrade (Instalacja starszej wersji)

Aby odblokować system, musisz najpierw zainstalować wersję oprogramowania, która posiada lukę umożliwiającą dostęp przez protokół ADB.

> [!NOTE]
> Jeśli podczas tego procesu w pojeździe znajduje się karta SD, pojawi się komunikat o błędzie; dlatego należy wyjąć kartę SD i rozpocząć proces bez włożonej karty.

### 1. Przygotowanie
* **Weryfikacja wersji**: Upewnij się, że Twoja obecna wersja zaczyna się od `13.1.33.XXXX` (np. `13.1.33.2511`). Sprawdzisz to w: `Ustawienia` ➔ `System` ➔ `Wersja`.
* **Pobieranie**: Pobierz wersję [13.1.33.2404](https://drive.google.com/file/d/1awJk8OgAMT_z3DHve5cFFUzfH7viOVfT/view?usp=sharing), która umożliwia odblokowanie.
* **Pendrive**: Nośnik **8 GB / 16 GB / 32 GB** sformatowany jako **FAT32**. W przypadku większych nośników użyj formatu **exFAT**.
* **Struktura plików**: Utwórz na pendrive foldery: `BYDUpdatePackage` ➔ `msm8953_64` ➔ `UpdateFull.zip` (Ostatni to nasz pobrany plik).
* **Nazwa pliku**: Umieść pobrany plik w ostatnim folderze i zmień jego nazwę na **UpdateFull.zip**.

> [!CAUTION]
> Przed rozpoczęciem upewnij się, że poziom naładowania baterii trakcyjnej wynosi min. **30%**. Nie wyłączaj pojazdu podczas procesu aktualizacji!

### 2. Procedura instalacji
1. Włącz pojazd i włóż przygotowany pendrive (jeśli auto ma tylko porty USB-C, użyj przejściówki).
2. Gdy na ekranie pojawi się **Kod QR**, przytrzymaj przez **10 sekund** jednocześnie:
   * **Lewą strzałkę** na kierownicy (powrót).
   * **Przycisk głośności** (pokrętło/przycisk obok selektora biegów).
   <img width="1187" height="279" alt="image" src="https://github.com/user-attachments/assets/ec2b5cce-7caa-4fa8-bfb6-ef9648c7887c" />
3. Proces trwa zazwyczaj **10–20 minut**. Po zakończeniu i ponownym uruchomieniu ekranu wyjmij pendrive.

---

## 🔓 SEKCJA B: Dostęp ADB

### 1. Włączanie trybu DEBUG (ADB)
1. Połącz swój telefon z systemem multimedialnym auta przez **Bluetooth**.
2. Otwórz aplikację `Telefon` w aucie i wpisz kod: `*#91532547#*`.
3. Zapisz **6 ostatnich cyfr numeru IMEI**, który pojawi się na ekranie.
4. Wejdź na stronę [ahmada3mar.github.io/BYD/](https://ahmada3mar.github.io/BYD/) (na telefonie/komputerze) i wygeneruj hasło, wpisując te 6 cyfr.
5. Wpisz wygenerowane hasło na tablecie auta i zatwierdź prawym dolnym przyciskiem (z chińskimi znakami).
6. W menu `Test Tools` zjedź na dół i zaznacz:
   * ✅ `Wireless adb debug switch`
   * ✅ `Debug mode when USB is connected`
   <img width="748" height="291" alt="image" src="https://github.com/user-attachments/assets/44ff06ae-b885-4b87-9c77-40ccf7541614" />

   <img width="967" height="291" alt="image" src="https://github.com/user-attachments/assets/7bfefb51-9f4d-4612-a54a-bc9564f79ee1" />

---

## ⤵️ SEKCJA C: Instalacja aplikacji

### 1. Metoda bezprzewodowa (Aplikacja Bugjaeger)
1. Udostępnij **Hotspot WiFi** z telefonu i połącz z nim auto.
2. W ustawieniach WiFi auta kliknij ikonę `i` przy nazwie sieci i zanotuj **Adres IP** pojazdu.
<img width="893" height="306" alt="image" src="https://github.com/user-attachments/assets/62e98164-78c2-4d0c-ba52-881b3119a776" />

3. W aplikacji **Bugjaeger** (na telefonie) kliknij ikonę wtyczki (`+`), wpisz IP auta oraz port `5555`, a następnie kliknij `Connect`.
4. **Zaakceptuj połączenie** na ekranie auta (zaznacz `Always allow` i kliknij `Allow`).
5. Zainstaluj plik [PackageInstallerUnlocker.apk](https://drive.google.com/file/d/1aoWeo-XZFAiJkM3-cptNwGVxZuNtRbis/view?usp=drive_link). Od tego momentu system będzie pozwalał na instalację plików APK.

### 2. Metoda tradycyjna (Pendrive)
1. Skopiuj wybrane pliki APK bezpośrednio do głównego folderu na pendrive (FAT32/exFAT).
2. Włóż pendrive do portu USB w aucie.
3. Otwórz wbudowaną aplikację `Menedżer plików` (File Manager) i zainstaluj aplikacje bezpośrednio z nośnika.

---

## 📦 Polecane aplikacje
* ⚡ [Electro](https://electro.app.br/): Zaawansowane dane o pojeździe i statystyki baterii.
* 🌌 [AuroraStore](https://drive.google.com/file/d/1leQ-cinJ0gSUhrYMBQZQlGwhv2g1pXsM/view?usp=sharing): Bezpieczny zamiennik Sklepu Play.
* 🛠 [MicroG](https://drive.google.com/file/d/1tY5HX0U_q7cOxFQpiPefZWRIWTlG6NQi/view?usp=sharing): Niezbędne do działania usług Google. (W ustawieniach wyłącz rejestrację urządzenia, zaloguj się i wyłącz AutoStart w narzędziach systemowych).
* 📺 [Revanced Manager](https://drive.google.com/file/d/1zjbrAkGXbFAT36nsOZx98l_E_BD44Mvz/view?usp=sharing): YouTube bez reklam i z funkcją odtwarzania w tle.

---

## ⬆️ SEKCJA D: Aktualizacja Systemu (OTA)

Po udanym odblokowaniu i zainstalowaniu potrzebnych aplikacji, możesz bezpiecznie wrócić do nowszej wersji systemu. Twoje aplikacje pozostaną zainstalowane.

1. **Zalecane wersje**:
   * **[13.1.33.2511](https://drive.google.com/file/d/1TmPu7NKAuGVmCHNG6iFmebZRe3Pk1XRa/view?usp=sharing)** – Najbardziej stabilna wersja.
   * **[13.1.33.2602](https://drive.google.com/file/d/1E02Lzp_Gccb9rsEMeGqV3jNhllysXCH2/view?usp=sharing)** – Najnowsza wersja (zawiera polską nawigację, lecz nie zalecam ze względu na stabilność).
2. **Procedura**: Przygotuj pendrive analogicznie jak w Sekcji A i wybierz na ekranie opcję `Upgrade OTG`. Podczas aktualizacji (**ok. 15 minut**) nie dotykaj żadnych przycisków.
