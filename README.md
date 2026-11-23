# Exavera CBT — Rilis Resmi Windows (x64 Portable)

Repositori distribusi resmi aplikasi **Exavera CBT** untuk perangkat **Windows 10 / Windows 11 (64-bit)**.

---

## 1. Unduhan Resmi Terbaru

- **Berkas Instalasi:** [`Exavera-CBT-Windows-Universal.zip`](https://github.com/lutfiyblock-alt/exavera_winx64/releases/latest/download/Exavera-CBT-Windows-Universal.zip)
- **Checksum Integritas:** [`Exavera-CBT-Windows-Universal.zip.sha256`](https://github.com/lutfiyblock-alt/exavera_winx64/releases/latest/download/Exavera-CBT-Windows-Universal.zip.sha256)
- **Halaman Semua Rilis:** [Releases (`exavera_winx64`)](https://github.com/lutfiyblock-alt/exavera_winx64/releases)

---

## 2. Persyaratan Sistem

- **Sistem Operasi:** Windows 10 (versi 1903 atau lebih baru) / Windows 11 (arsitektur `x86_64`).
- **Perangkat Keras:** Laptop Windows dengan adaptor Bluetooth bawaan aktif (wajib menyala sebelum masuk sesi ujian).
- **Runtime Sistem:** DLL Microsoft Visual C++ Runtime (`vcruntime140.dll`, `vcruntime140_1.dll`, `msvcp140.dll`) sudah dibundel di dalam arsip rilis sehingga langsung berjalan di Windows 10/11 bersih tanpa instalasi terpisah.

---

## 3. Cara Memasang & Menjalankan

1. Unduh **`Exavera-CBT-Windows-Universal.zip`** dari halaman rilis terbaru.
2. Klik kanan file `.zip` $\to$ **Extract All...** ke folder permanen di komputer, misalnya `C:\ExaveraCBT\`.
   *(Jangan menjalankan aplikasi langsung dari dalam arsip ZIP karena seluruh berkas `.dll` dan `data/` harus berada di direktori yang sama).*
3. Buka folder hasil ekstrak lalu jalankan **`Exavera-CBT.exe`**.
4. Jika muncul peringatan *Windows protected your PC* (Microsoft Defender SmartScreen), klik **More info** $\to$ **Run anyway**.

---

## 4. Verifikasi Integritas Berkas (SHA-256)

Buka **PowerShell** pada folder tempat file `.zip` diunduh dan jalankan perintah berikut:

```powershell
Get-FileHash .\Exavera-CBT-Windows-Universal.zip -Algorithm SHA256
```

Cocokkan nilai **Hash** yang tampil dengan isi berkas **`Exavera-CBT-Windows-Universal.zip.sha256`** pada halaman rilis untuk memastikan file tidak rusak atau dimodifikasi selama proses unduh.

---

## 5. Catatan Operasional Ujian & Ekspor Dokumen

- **Mode Tenang (Offline):** Putuskan koneksi Wi-Fi/internet sesuai instruksi preflight sebelum membuka naskah ujian, dan biarkan **Bluetooth Windows tetap menyala** selama ujian berlangsung.
- **Autentikasi Login & Unfreeze:** Karena target Windows tidak memakai pemindai kamera langsung, gunakan tombol pilih gambar QR (`PNG`/`JPG`) atau tempel token (`Ctrl+V`), serta **PIN TOTP 6 digit** dari pengawas ruang untuk membuka kunci.
- **Unduh Kisi-Kisi (PDF & PNG):** Berkas kisi-kisi yang diekspor dari jendela pratinjau resmi otomatis tersimpan ke folder **`Downloads`** Windows pengguna.
