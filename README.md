# Latihan Responsi PBO - Praktikum PBO-I

Dokumen ini disusun untuk memenuhi tugas latihan responsi pada mata kuliah Praktikum Pemrograman Berorientasi Objek (PBO) kelas PBO-I.

---

## Deskripsi Singkat Program
Program ini adalah aplikasi desktop berbasis Java Swing yang dirancang untuk mengelola data film/video (**CRUD**: *Create, Read, Update, Delete*) dengan menerapkan arsitektur **MVC (Model-View-Controller)** serta pola **DAO (Data Access Object)** untuk menghubungkan aplikasi Java dengan database MySQL.

Secara singkat, program ini berfungsi untuk:
1. **Menyimpan & Menampilkan Data Film:** Memasukkan data film baru (Judul, Alur, Penokohan, Akting) ke database MySQL dan menampilkannya langsung ke dalam tabel aplikasi (`JTable`).
2. **Menghitung Rating Otomatis:** Menghitung nilai akhir secara otomatis di bagian *Controller* menggunakan rumus rata-rata:  
   $$\text{Nilai Rating} = \frac{\text{Alur} + \text{Penokohan} + \text{Akting}}{3}$$  
   Hasil hitungan ini otomatis mengisi kolom "Nilai" tanpa perlu diketik manual oleh pengguna.
3. **Mengubah & Menghapus Data:** Memperbarui data film yang dipilih dari tabel atau menghapusnya dengan aman lewat jendela popup konfirmasi (*Confirmation Dialog*).
4. **Membersihkan Form:** Mengosongkan seluruh kolom input teks dalam sekali klik menggunakan tombol *Clear*.
