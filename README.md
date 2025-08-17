# awesome-blog

Silakan ikuti instruksi di bawah ini untuk menyelesaikan pengaturan situs Qubt baru Anda.

## Instalasi

1. Tambahkan file LICENSE ke repositori Anda.  
2. Clone template ini ke komputer lokal Anda:  
   ```shell
   git clone https://github.com/<username>/<reponame>
  ```
3) Ubah file `config/_default/hugo.yaml`, `config/_default/params.yaml` dan `config/_default/menus.yaml` sesuai kebutuhan Anda. Informasi lebih lanjut dapat ditemukan di [wiki](https://github.com/chrede88/qubt/wiki/Configuration).
4) Tambahkan postingan blog Anda ke folder `content/blog/`. Lihat [wiki](https://github.com/chrede88/qubt/wiki/Content) atau contoh postingan untuk referensi.
5) Ubah `content/about.md` agar sesuai dengan preferensi Anda.
6) Jalankan `hugo server` untuk membangun versi lokal situs Anda. Situs bisa dilihat dengan membuka `localhost:1313` di browser (alamat sebenarnya akan muncul di CLI).

---

## Konfigurasi

Lihat [wiki](https://github.com/chrede88/qubt/wiki) untuk semua informasi mengenai konfigurasi.

---

## Memperbarui Versi Tema

Versi tema yang digunakan untuk membangun situs ditentukan pada file `go.mod`.

Disarankan untuk memperbarui ke versi yang sudah dirilis dan diuji. Untuk memperbarui ke versi tertentu, jalankan perintah berikut di terminal (pada direktori root repositori situs Anda):

```shell
  hugo mod get github.com/Chrede88/qubt@vX.Y.Z
```
Ganti X.Y.Z dengan nomor versi yang sesuai. Daftar rilis bisa ditemukan di [sini](https://github.com/chrede88/qubt/releases). Sebelum memperbarui, pastikan Anda memeriksa apakah ada perubahan besar (breaking changes) pada rilis yang dituju.

---

## Deploy ke GitHub Pages
Anda bisa dengan mudah melakukan deploy situs menggunakan GitHub Pages. Template ini sudah menyertakan workflow GitHub Action yang secara otomatis akan membangun dan mendeploy situs Anda ke GitHub Pages :+1:

`.github/deploymentWorkflow/buildDeploy.yml.` Untuk menggunakannya, pindahkan ke folder `.github/workflows/.`

Workflow ini sudah siap digunakan, tetapi luangkan waktu untuk membacanya dan memahami alurnya. Jika tidak, workflow ini hanya akan menjadi “kotak hitam ajaib” yang sulit diperbaiki saat terjadi masalah!

Langkah terakhir: Masuk ke Settings -> Pages -> Build and deployment -> Source, lalu atur ke GitHub Actions.

Mulai saat itu, setiap kali Anda menerbitkan rilis baru, workflow ini akan membangun dan mendeploy situs Anda :tada:

Situs Anda akan tersedia di URL berikut:
`https://gitkodachi.github.io/awesome-blog`