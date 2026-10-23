HOME WITH HER

Game visual novel horor psikologis dan dark romance untuk Android, menggunakan HTML, CSS, JavaScript, Kotlin, dan Android WebView.

Fitur

- Cerita visual novel dengan dialog dan pilihan.
- Horor psikologis, efek visual, dan ekspresi karakter.
- Menu utama dan pengaturan game.
- Sistem simpan dan muat permainan sesuai implementasi kode.
- Dapat dimainkan secara offline.
- Build APK otomatis melalui GitHub Actions.

Cara Membuat APK

1. Siapkan proyek

Ekstrak ZIP proyek dan pastikan file "settings.gradle.kts", "build.gradle.kts", "gradle.properties", folder "app", serta folder ".github" tersedia.

2. Unggah ke GitHub

Buat repository baru bernama "HOME-WITH-HER". Unggah seluruh isi folder proyek ke root repository. Jangan mengunggah ZIP sebagai pengganti file proyek.

Pastikan workflow berada di:
".github/workflows/build-apk.yml"

3. Jalankan build

Buka tab Actions di GitHub. Pilih workflow Build APK, kemudian tekan Run workflow apabila build tidak berjalan otomatis.

Tunggu sampai proses build selesai. Jika gagal, buka log langkah yang berwarna merah untuk melihat penyebabnya.

4. Unduh APK

Pada halaman build yang berhasil, cari Artifacts. Unduh "HOME-WITH-HER-debug-apk", ekstrak file ZIP, lalu temukan "app-debug.apk".

5. Instal di Android

Buka "app-debug.apk" melalui pengelola berkas HP. Izinkan pemasangan dari sumber tersebut jika Android memintanya, lalu tekan Install.

Struktur Proyek

- "app/src/main/java/com/homewithher/game/MainActivity.kt" — pembungkus Android WebView.
- "app/src/main/assets/index.html" — halaman utama game.
- "app/src/main/assets/css/" — tampilan dan efek visual.
- "app/src/main/assets/js/" — mesin game, cerita, audio, pengaturan, dan penyimpanan.
- ".github/workflows/build-apk.yml" — workflow build APK otomatis.

Catatan

APK yang dibuat oleh workflow ini merupakan debug build untuk pengujian. Keberhasilan build dan fungsi game harus diperiksa langsung melalui GitHub Actions dan diuji di perangkat Android.

Jangan mengunggah keystore, kata sandi, token, atau informasi rahasia ke repository publik.
