# Digital Watch – Landing Page Jam Tangan Pintar

Landing page satu halaman untuk memperkenalkan produk jam tangan pintar (smart watch). Proyek ini dibuat hanya dengan **HTML dan CSS**, tanpa framework dan tanpa JavaScript, jadi mudah dipelajari dan dimodifikasi.

<!-- Tambahkan screenshot halaman, lalu hapus tanda komentar pada baris di bawah:
![Tampilan landing page](screenshot.png)
-->

## Isi Halaman

| Bagian | Keterangan |
|---|---|
| **Navbar** | Logo dan menu: Beranda, Fitur, Tentang, FAQ, Kontak |
| **Hero** | Judul utama, deskripsi, tombol *Beli Sekarang* dan *Lihat Fitur*, serta foto jam dengan latar bergelombang |
| **Fitur Unggulan** | Empat kartu fitur dengan ikon: Kualitas Tinggi, Desain Elegan, Teknologi Terbaru, Mudah Digunakan |
| **Tentang Produk** | Foto jam dan kartu spesifikasi produk |
| **FAQ** | Empat pertanyaan umum yang bisa dibuka dan ditutup |
| **Kontak** | Ajakan memesan dengan tombol *Hubungi Kami* |
| **Footer** | Hak cipta |

## Teknologi

- **HTML5**: struktur halaman, termasuk elemen `<details>` untuk FAQ tanpa JavaScript
- **CSS3**: CSS Grid, Flexbox, CSS Variables, `clamp()`, gradient, dan media query
- **Google Fonts**: [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans)

## Struktur Folder

```
.
├── index.html     # Struktur dan isi halaman
├── style.css      # Seluruh gaya tampilan
├── jam_biru.png   # Foto produk (latar transparan)
└── README.md      # Dokumentasi proyek
```

## Cara Menjalankan

1. Unduh atau clone repositori ini:
   ```bash
   git clone https://github.com/nabilafirdausi28/Tugas_Landing_Page.git
   ```
2. Buka foldernya, lalu klik dua kali `index.html` agar terbuka di browser.

Tidak perlu instalasi apa pun. Pastikan `index.html`, `style.css`, dan `jam_biru.png` berada di folder yang sama. Koneksi internet hanya dibutuhkan untuk memuat font dari Google Fonts.

## Cara Mengubah Isi dan Tampilan

**Warna.** Semua warna utama ada di bagian atas `style.css`:

```css
:root{
  --accent:#1e6fe8;       /* warna tombol, menu aktif, dan ikon */
  --accent-dark:#1555bd;  /* warna tombol saat disentuh dan latar bagian kontak */
  --tint:#e8f1ff;         /* warna latar bagian hero */
  --soft:#f5f8fd;         /* warna latar bagian Tentang Produk */
}
```

**Foto produk.** Timpa file `jam_biru.png` dengan foto lain, atau ubah `src` pada tag `<img>` di `index.html` (ada dua tempat: bagian hero dan Tentang Produk). Gunakan PNG berlatar transparan agar menyatu dengan halaman, dan hindari spasi pada nama file.

**Spesifikasi produk.** Cari bagian `<dl class="specs">` di `index.html`. Nilai di sana (layar 1,9 inci, baterai 7 hari, IP68, Bluetooth 5.3, dan seterusnya) hanya contoh, jadi sesuaikan dengan produk yang sebenarnya.

**FAQ.** Setiap pertanyaan ada dalam satu blok `<details>`. Salin satu blok untuk menambah pertanyaan, atau hapus blok yang tidak diperlukan.

**Tombol kontak.** Ganti `halo@contoh.com` pada tombol *Hubungi Kami* di `index.html` dengan emailmu, atau ubah menjadi tautan WhatsApp.

## Responsif

Tampilan menyesuaikan lebar layar. Pada layar di bawah 820 px, layout dua kolom berubah menjadi satu kolom, foto produk tampil di atas teks, dan teks hero diratakan ke tengah.

## Deploy ke GitHub Pages

1. Unggah semua file ke repositori GitHub.
2. Buka **Settings → Pages**.
3. Pada **Build and deployment**, pilih **Deploy from a branch**.
4. Pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.
5. Tunggu beberapa menit. Situsnya akan aktif di `https://nabilafirdausi28.github.io/Tugas_Landing_Page/`.

## Catatan

- Desain terinspirasi dari contoh template landing page produk. Seluruh kode ditulis ulang.
- Pastikan kamu berhak memakai foto produk yang dipasang. Untuk situs yang dipublikasikan, gunakan foto milik sendiri atau foto berlisensi bebas.

## Rencana Pengembangan

- [ ] Menambahkan bagian testimoni pelanggan
- [ ] Menambahkan pilihan warna produk
- [ ] Menambahkan galeri foto produk

## Lisensi

Tentukan lisensi sesuai kebutuhanmu, misalnya [MIT](https://choosealicense.com/licenses/mit/).
