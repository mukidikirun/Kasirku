KASIRKU - BUILD APK ONLINE

Project ini disiapkan agar APK dapat dibuat melalui GitHub Actions tanpa Android Studio.
Laptop Windows 7 32-bit tidak perlu menjalankan Android Studio.

LANGKAH SINGKAT:
1. Buat akun/login GitHub di https://github.com
2. Buat repository baru. Agar gratis dan sederhana, pilih Public.
3. Buka repository tersebut.
4. Upload ISI FOLDER KasirKu ini, bukan file ZIP-nya.
   Struktur paling atas harus berisi:
      .github/workflows/build-apk.yml
      app/
      build.gradle
      settings.gradle
5. Setelah semua file ter-upload, buka tab Actions.
6. Pilih "Build KasirKu APK".
7. Klik "Run workflow" (atau lakukan push ke branch main).
8. Tunggu sampai proses selesai dengan tanda centang hijau.
9. Buka hasil workflow tersebut.
10. Di bagian Artifacts, download "KasirKu-debug-apk".
11. Di dalam ZIP hasil download ada app-debug.apk.
12. Pindahkan APK ke HP Android lalu instal.

CATATAN:
- Jangan upload file ZIP sebagai satu-satunya file repository, karena GitHub tidak otomatis mengekstraknya.
- Project menggunakan Android Gradle Plugin 8.6.1, Gradle 8.7, dan Java 17.
- Proses build membutuhkan internet di server GitHub untuk mengambil dependency Android/ML Kit.
