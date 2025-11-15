# speed.xobe-panel.my.id

Ini adalah proyek Speed Test sederhana yang berjalan penuh di sisi klien tanpa backend tambahan. Seluruh fungsi berada di satu file `index.html` dan digunakan untuk mengukur kecepatan download pengguna dengan mengunduh file dummy dari Cloudflare berukuran 5MB. Proyek ini bisa dijalankan di hosting statis seperti Vercel tanpa konfigurasi tambahan.

Proyek hanya terdiri dari satu file utama yaitu `index.html` yang berisi struktur halaman, gaya dasar, tombol untuk memulai pengukuran, dan script untuk melakukan proses speed test. Ketika tombol ditekan, browser akan mulai mengunduh file 5MB menggunakan `fetch()` dengan cache dimatikan. Waktu unduhan dihitung menggunakan `performance.now()`, kemudian hasilnya dikonversi menjadi Mbps dan ditampilkan pada halaman.

Untuk melakukan deployment, cukup unggah file `index.html` ke platform seperti Vercel. Jika ingin menggunakan domain khusus `speed.xobe-panel.my.id`, tambahkan domain tersebut ke pengaturan domain project di Vercel. Kemudian buka Cloudflare dan buat record CNAME baru dengan name `speed` dan target `cname.vercel-dns.com` dengan DNS Only. Setelah propagasi selesai, subdomain akan langsung mengarah ke halaman speed test.

Proyek ini bebas dimodifikasi, dikembangkan ulang, atau dipadukan dengan fitur tambahan seperti upload test, ping test, grafik real-time, atau tampilan UI yang lebih interaktif. Tidak ada batasan penggunaan.
