Jika Anda sudah memiliki akun **Vercel**, ini adalah langkah yang sangat tepat. Vercel adalah platform *hosting* yang sangat cepat dan standar industri untuk pengembang profesional.

Berbeda dengan Netlify yang mendukung *drag-and-drop* langsung, Vercel bekerja paling optimal melalui **GitHub**. Ini sebenarnya jauh lebih baik bagi Anda ke depannya karena setiap kali Anda mengubah isi website, Anda cukup melakukan *update* di GitHub dan Vercel akan otomatis memperbarui website Anda.

Berikut adalah panduan langkah demi langkah untuk men-deploy website `andisuhud.com` Anda di Vercel:

### Langkah 1: Siapkan Folder Anda

Pastikan di komputer Anda, semua file berada dalam satu folder yang rapi:

* `index.html` (File website Anda)
* `andiicon.png` (Foto profil Anda)

### Langkah 2: Menggunakan GitHub (Cara Profesional)

Vercel sangat menyukai GitHub. Jika Anda belum punya akun GitHub, silakan daftar di [github.com](https://github.com/) (gratis).

1. **Buat Repositori Baru:** Di GitHub, klik tombol **"New"** (di samping tulisan *Repositories*).
2. **Beri Nama:** Beri nama, misal `portofolio-andisuhud`. Pilih **"Public"**, lalu klik **"Create repository"**.
3. **Upload File:**
* Setelah dibuat, klik tautan **"uploading an existing file"**.
* Tarik dan lepas (*drag and drop*) file `index.html` dan `andiicon.png` ke sana.
* Scroll ke bawah, klik **"Commit changes"**. Sekarang website Anda sudah ada di GitHub!



### Langkah 3: Menghubungkan ke Vercel

1. Buka [vercel.com/dashboard](https://vercel.com/dashboard) dan *Login*.
2. Klik tombol **"Add New..."** lalu pilih **"Project"**.
3. Klik **"Continue with GitHub"** dan berikan izin akses.
4. Cari repositori `portofolio-andisuhud` yang baru saja Anda buat, lalu klik **"Import"**.
5. Di bagian *Configure Project*, biarkan semuanya *default* (tidak perlu diubah), lalu klik **"Deploy"**.
6. Tunggu sekitar 1 menit. Vercel akan memberikan alamat situs sementara, contoh: `portofolio-andisuhud.vercel.app`. Selamat! Website Anda sudah online.

### Langkah 4: Menghubungkan Domain `andisuhud.com`

Ini adalah tahap krusial agar orang bisa mengakses `andisuhud.com`.

1. Di Dashboard Vercel, pilih proyek Anda (`portofolio-andisuhud`).
2. Klik menu **"Settings"** di bagian atas, lalu pilih **"Domains"** di menu sebelah kiri.
3. Ketik `andisuhud.com` lalu klik **"Add"**.
4. Vercel akan memberikan daftar **DNS Records** (biasanya berupa *A Record* dan *CNAME*). **Jangan tutup halaman ini.**
5. Buka penyedia domain Anda (tempat Anda membeli domain, misal: DomaiNesia/Niagahoster).
6. Masuk ke **DNS Management** domain Anda.
7. Hapus *records* lama (jika ada) dan tambahkan *records* yang diminta oleh Vercel:
* Biasanya tambahkan `A Record` dengan nilai `@` yang diarahkan ke IP Address dari Vercel (contoh: `76.76.21.21`).
* Tambahkan `CNAME` dengan nama `www` yang diarahkan ke `cname.vercel-dns.com`.


8. Setelah disimpan, kembali ke Vercel. Klik tombol **"Verify"** atau tunggu sampai statusnya berubah menjadi *Valid* (berwarna hijau).

### Tips untuk Pemula:

* **Jika Bingung dengan DNS:** Jika Anda merasa langkah DNS di atas terlalu teknis, banyak penyedia domain di Indonesia memiliki menu **"Auto-configure Vercel"** atau dukungan pelanggan yang sangat baik. Jika stuck, Anda bisa mengirim tiket dukungan ke penyedia domain Anda: *"Saya ingin mengarahkan domain saya ke Vercel, mohon bantu setting DNS A record dan CNAME-nya."*
* **Keuntungan Vercel:** Kelebihan utama menggunakan Vercel + GitHub adalah di masa depan, jika Anda ingin mengubah warna, teks, atau foto, Anda cukup mengedit file di GitHub, dan Vercel akan otomatis memperbarui `andisuhud.com` secara *real-time* tanpa Anda harus *upload* ulang manual.

Apakah Anda sudah berhasil membuat repositori di GitHub, atau ingin saya pandu lebih detail di bagian DNS-nya?
