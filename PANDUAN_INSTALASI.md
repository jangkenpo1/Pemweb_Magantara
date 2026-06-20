PANDUAN INSTALASI PROYEK MAGANTARA

1. Buka Terminal di Laragon, arahkan ke folder www:
cd C:\laragon\www

2. Tarik kode dari GitHub:
git clone <URL-GITHUB-REPO-INI>

3. Masuk ke folder proyek:
cd <nama-folder-repo>

4. Instal library pendukung:
composer install

5. Siapkan file .env:
- Jika Anda menerima file .env dari WhatsApp: Pindahkan file tersebut ke dalam folder proyek ini.

6. Buat Database Kosong:
Buka HeidiSQL di Laragon, buat database kosong bernama "pemweb".

7. Buat penghubung folder gambar: (jalanin di file )
php artisan storage:link

8. Bangun tabel dan isi data awal:
php artisan migrate:fresh --seed

Selesai. Buka browser dan jalankan melalui http://<nama-folder-repo>.test

AKUN UJI COBA:
- Admin: admin@magantara.com (Password: password)
- Perusahaan: rekrutmen@gojek.com (Password: password)
- Mahasiswa: mahasiswa@gmail.com (Password: password)
