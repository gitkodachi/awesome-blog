# awesome-blog

This is the theme template repository! **Please** follow the installation instructions below.

Ini adalah repositori template tema! **Harap** ikuti instruksi instalasi di bawah ini.  
Jika Anda mencari repositori tema sebenarnya, ikuti [tautan ini](https://github.com/Chrede88/qubt).

## Instalasi

1) Gunakan template ini dengan menekan `Use this template`. **Jangan fork repositori ini!**  
2) Tunggu 20–30 detik lalu perbarui halaman. Workflow `Clean Template` akan berjalan secara otomatis, membuat/mengisi berkas berdasarkan pengguna Github Anda.  
3) Tambahkan LICENSE ke repositori Anda.  
4) Clone versi template Anda ke komputer lokal:  
```shell
git clone https://github.com/<username>/<reponame>
```
5) Ubah nama modul agar sesuai dengan repositori github Anda di `go.mod`.
6) Ubah `config/_default/hugo.yaml`, `config/_default/params.yaml` dan `config/_default/menus.yaml` sesuai kebutuhan Anda. Informasi lebih lanjut dapat ditemukan di [wiki tema](https://github.com/chrede88/qubt/wiki/Configuration).
7) Tambahkan postingan blog Anda ke `content/blog/`. Lihat [wiki](https://github.com/chrede88/qubt/wiki/Content) atau contoh postingan untuk referensi.
8) Ubah `content/about.md` agar sesuai dengan preferensi Anda.
9) Bangun versi lokal situs Anda dengan menjalankan hugo server. Anda dapat melihat situs dengan membuka `localhost:1313` (URL sebenarnya akan ditampilkan di CLI) di browser.

---

## Fitur

- Tema blog pribadi sederhana, dirancang untuk mobile-first.
- Mode gelap otomatis (berdasarkan pengaturan sistem).
- Dukungan emoji untuk desain yang menyenangkan.
- Endpoint healthcheck (/healthcheck.json).

---

## Konfigurasi

Lihat [wiki](https://github.com/chrede88/qubt/wiki) ntuk semua informasi tentang konfigurasi dan cara mudah melakukan deploy ke Github Pages.

---

## Perbarui Versi Tema
Versi tema yang digunakan untuk membangun situs ditentukan dalam file `go.mod`.

Praktik terbaik adalah memperbarui ke versi yang sudah dirilis dan diuji. Untuk memperbarui ke versi tertentu jalankan perintah berikut di terminal/command line (pada direktori root repositori situs Anda):

```shell
  hugo mod get github.com/chrede88/qubt@vX.Y.Z
```
Ganti X,Y & Z dengan nomor versi yang sesuai. Anda dapat menemukan rilis [disini](https://github.com/chrede88/qubt/releases). Harap periksa apakah ada perubahan besar (breaking changes) yang tercantum pada rilis yang ingin Anda perbarui sebelum melanjutkan.