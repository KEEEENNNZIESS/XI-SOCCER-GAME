# ERA XI — Android Project v0.1 (Landscape)

Ini adalah **kerangka aplikasi Android yang membungkus prototype 3D ERA XI**. Orientasi dikunci landscape, layar penuh, dan antarmuka dimuat dari aset lokal aplikasi.

## Status saat ini
- APK belum dikompilasi di lingkungan ini karena Android SDK/Gradle belum tersedia.
- Prototype 3D masih berupa demonstrasi visual: 22 pemain placeholder, bola, pergantian kamera, dan tiga profil gerakan contoh.
- Three.js saat ini dimuat dari CDN, jadi koneksi internet diperlukan saat membuka layar pertandingan.
- Belum ada pertandingan sepak bola penuh, kontrol pemain sungguhan, mode kompetisi, database pemain historis terverifikasi, atau sistem penyimpanan koleksi.
- Angka atribut demo bukan statistik historis resmi.

## Cara mendapatkan APK melalui GitHub Actions (bisa dari browser HP)
1. Buat repository GitHub baru dan upload seluruh isi folder project ini.
2. Buka tab **Actions** pada repository.
3. Pilih workflow **Build ERA XI APK** lalu tekan **Run workflow** (atau tunggu build otomatis setelah push ke branch `main`).
4. Setelah selesai, buka hasil run dan unduh artifact **ERA-XI-debug-apk**.
5. Ekstrak ZIP artifact, lalu install `app-debug.apk` di Android. Android mungkin meminta izin untuk memasang aplikasi dari sumber tersebut.

## Build lokal
Gunakan Android Studio/Android SDK dengan JDK 17, lalu jalankan `gradle assembleDebug` dari root project.

## Identitas aplikasi
- Application ID: `com.eraxi.game`
- Version: `0.1.0`
- Minimum Android: API 23 (Android 6.0)
- Orientation: Landscape

Ini debug APK untuk pengujian, bukan rilis Play Store yang ditandatangani dengan release key.
