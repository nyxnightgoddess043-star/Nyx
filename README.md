# Dewi Bulan Permata — Infinix Note 30 4G

Proyek Android (Kotlin) bertema anime bulan/kristal ungu. Ada wallpaper portrait, ikon kristal, pintasan aplikasi, tombol pasang wallpaper, dan pilihan aplikasi Home.

## Cara membuat APK hanya dengan HP Android (tanpa komputer)

APK dibangun di cloud menggunakan GitHub Actions. Kamu perlu akun GitHub dan koneksi internet.

1. Unduh ZIP proyek ini dan ekstrak menggunakan aplikasi pengelola file di HP.
2. Buka https://github.com di browser dan masuk/daftar.
3. Buat repository baru, misalnya `dewi-bulan-permata`, lalu pilih **Public** atau **Private**.
4. Di repository, pilih **Add file > Upload files**. Unggah semua isi folder proyek yang sudah diekstrak, termasuk folder tersembunyi `.github/workflows` dan file `android.yml`. Pastikan `settings.gradle`, `build.gradle`, dan folder `app` berada langsung di root repository.
   - Jika browser HP tidak menampilkan folder `.github`, gunakan tampilan **Desktop site** atau buat file workflow secara manual di GitHub: **Add file > Create new file**, nama `.github/workflows/android.yml`, lalu salin isi workflow dari ZIP.
5. Tekan **Commit changes**. Workflow akan mulai berjalan otomatis.
6. Buka tab **Actions**, pilih **Build Dewi Bulan Permata APK**, lalu buka proses build terbaru.
7. Tunggu sampai tanda centang hijau. Di bagian **Artifacts**, unduh `Dewi-Bulan-Permata-debug-apk`.
8. Ekstrak ZIP artifact tersebut di HP. Di dalamnya ada `app-debug.apk`. Ketuk file APK untuk memasang. Jika diminta, izinkan browser atau aplikasi File memasang aplikasi dari sumber tersebut.

## Catatan
- Build pertama dapat memerlukan beberapa menit.
- Jika build gagal, buka proses di tab Actions dan lihat log; pesan error bisa dikirim untuk dibantu.
- APK debug cocok untuk pemasangan pribadi, bukan rilis Play Store.
- Launcher ini versi awal. Android/XOS bisa meminta kamu memilih aplikasi Home secara manual. Aplikasi pihak ketiga tidak dapat otomatis mengganti seluruh ikon sistem, layar kunci, status bar, atau widget musik/cuaca.
- Wallpaper gambar ada di `app/src/main/res/drawable-nodpi/wallpaper_dewi_bulan.jpg`.
