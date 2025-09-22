# Lab1Web

Jawaban Pertanyaan Praktikum 1 – HTML Dasar

1. Lakukan perubahan pada kode sesuai dengan keinginan anda, amati perubahannya adakah error ketika terjadi kesalahan penulisan tag?

HTML bersifat *toleran terhadap kesalahan*. Kalau ada tag salah ketik (misalnya `<pp>` atau `<p>` tanpa penutup), browser biasanya tidak menampilkan pesan error, tapi langsung mengabaikan atau mencoba memperbaikinya. Hasilnya tampilan bisa berantakan, tapi jarang muncul error seperti di bahasa pemrograman.



2. Apa perbedaan dari tag `<p>` dengan tag `<br>`?

* `<p>` digunakan untuk membuat **paragraf baru**. Tag ini bersifat *block-level element*, jadi ada jarak (margin) atas dan bawah secara otomatis.
* `<br>` hanya untuk **pindah baris** di dalam teks. Tidak membuat paragraf baru, hanya turun satu baris.

Contoh:

```html
<p>Ini paragraf pertama.</p>
<p>Ini paragraf kedua.</p>
Teks baris pertama.<br>Teks baris kedua.
```



3. Apa perbedaan atribut `title` dan `alt` pada tag `<img>`?

* `alt` → teks alternatif yang muncul kalau gambar gagal dimuat, juga dibaca oleh screen reader (aksesibilitas).
* `title` → teks yang muncul saat kursor diarahkan ke gambar (tooltip).

Contoh:

```html
<img src="logo.png" alt="Logo Universitas" title="Ini adalah logo UPB">
```



4. Untuk mengatur ukuran gambar, digunakan atribut `width` dan `height`. Agar tampilan gambar proporsional sebaiknya kedua atribut tersebut diisi semua atau tidak?

Tidak perlu diisi semua. Cukup isi **salah satu** (`width` atau `height`), maka browser otomatis menyesuaikan sisi lainnya agar gambar tetap proporsional. Kalau keduanya diisi dengan ukuran yang tidak sesuai rasio asli, gambar bisa jadi gepeng atau melar.



5. Pada link tambahkan atribut target dengan nilai atribut bervariasi (`_blank`, `_self`, `_top`, `_parent`), apa yang terjadi pada masing-masing nilai atribut tersebut?

* `_blank` → membuka link di tab/jendela baru.
* `_self` → membuka link di tab yang sama (default).
* `_top` → membuka link di frame paling atas, berguna kalau ada nested frame.
* `_parent` → membuka link di parent frame dari frame saat ini.

Contoh:

```html
<a href="https://google.com" target="_blank">Buka di tab baru</a>
<a href="halaman.html" target="_self">Buka di tab yang sama</a>
<a href="halaman.html" target="_top">Buka di frame paling atas</a>
<a href="halaman.html" target="_parent">Buka di frame induk</a>
```
