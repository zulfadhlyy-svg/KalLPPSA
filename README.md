KalLPPSA - Cordova project (Android)
==================================

Saya telah sediakan projek Cordova mudah untuk anda build APK secara lokal.

**Apa yang saya sediakan:**
- Folder `www/` yang mengandungi aplikasi web (offline).
- `config.xml` untuk Cordova (nama app: KalLPPSA, id: com.example.kallppsa).
- Folder `res/icons/` untuk ikon (placeholder).

**Langkah mudah untuk bina APK (pada komputer anda):**

1. Pasang Node.js & npm: https://nodejs.org/
2. Pasang Cordova CLI:
   ```
   npm install -g cordova
   ```
3. Pasang Java JDK & Android Studio. Tetapkan `ANDROID_HOME` atau `ANDROID_SDK_ROOT` mengikut arahan Android Studio.
4. Ekstrak folder projek ini.
5. Buka terminal di dalam folder projek (yang mengandungi `config.xml` dan `www/`), kemudian jalankan:
   ```
   cordova platform add android
   cordova build android --release
   ```
   Untuk bina debug (cepat) gunakan:
   ```
   cordova build android
   ```
6. Selepas berjaya, APK debug biasanya terletak di:
   `platforms/android/app/build/outputs/apk/debug/app-debug.apk`
   Anda boleh salin APK itu ke telefon dan install (aktifkan 'Unknown sources' / sideload).

**Nota penting:**
- Jika mahu APK ditandatangani untuk pengedaran rasmi (play store), perlu sediakan keystore dan tandatangan (saya boleh bantu langkah itu juga).
- Untuk ikon sebenar, gantikan `res/icons/icon-192.png` dengan ikon bersaiz sesuai sebelum bina.
- Jika anda mahu saya hasilkan APK siap menggunakan perkhidmatan cloud (seperti EAS atau GitHub Actions), saya boleh terangkan langkahnya — tetapi saya tidak boleh membina APK secara langsung di sini.

Jika anda mahu saya terus sediakan APK, beri tahu dan saya akan pandu anda melalui pilihan cloud build atau bantu hasilkan langkah tanda tangan & bina di komputer anda.
