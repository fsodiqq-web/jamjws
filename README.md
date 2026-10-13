# JWS Jam BT Android app

Project Android Studio untuk mengendalikan sketch `JWS_Jam_BT.ino` melalui Bluetooth serial klasik (SPP), misalnya modul HC-05/HC-06.

## Build APK
1. Buka folder `JWSJamBT` melalui Android Studio versi terbaru.
2. Izinkan Android Studio mengunduh Android Gradle Plugin/SDK bila diminta.
3. Pilih **Build > Build APK(s)**.
4. APK debug akan berada di `app/build/outputs/apk/debug/app-debug.apk`.

## Sebelum menghubungkan
- Pasangkan HC-05/HC-06 melalui Settings Bluetooth Android terlebih dahulu.
- Pastikan baud rate modul dan sketch sama-sama 9600.
- Aplikasi mengirim perintah berakhiran newline, sesuai sketch.
- Waktu menggunakan format `SDTddmmyyhhmmssH`; `H`: Minggu=1 sampai Sabtu=7.

Catatan: lingkungan pembuatan saat ini tidak memiliki Android SDK/Gradle terpasang, sehingga APK belum dapat dikompilasi di sini. Source project ini siap dibuka dan dibuild di Android Studio.
