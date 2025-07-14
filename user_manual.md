🍽️ User Manual – Aplikasi Inventori Warteg
1. Deskripsi Program
Aplikasi ini merupakan program berbasis Python untuk mengelola stok bahan dan menu makanan di warteg (warung tegal). Pengguna dapat menambahkan bahan/menu, melihat daftar inventori, mengubah stok, menghapus data, serta melihat laporan stok dari yang terbanyak. Semua data disimpan ke dalam file warteg_data.json.

2. Persyaratan Sistem
Python versi 3.6 atau lebih tinggi

Dapat dijalankan melalui:

Terminal / Command Prompt (Windows, Linux, macOS)

VS Code

Google Colab

3. Struktur File
Nama File	Keterangan
warteg.py	File utama berisi seluruh kode program
warteg_data.json	File tempat penyimpanan data bahan/menu
user_manual.md	File dokumentasi penggunaan program (opsional)

4. Cara Menjalankan Program
🔹 Via Terminal / VS Code

Pastikan Python sudah terinstall.

Buka terminal/command prompt.

Arahkan ke folder tempat file warteg.py berada.

Jalankan perintah berikut:

bash
Copy
Edit
python warteg.py
🔹 Via Google Colab

Upload file warteg.py ke Colab.

Jalankan isi file baris demi baris.

File warteg_data.json akan muncul secara otomatis di direktori kerja.

5. Panduan Menu Program
Saat dijalankan, program akan menampilkan menu utama:

markdown
Copy
Edit
=== Menu Inventori Warteg ===
1. Tambah Bahan/Menu
2. Lihat Semua Data
3. Edit Stok
4. Hapus Data
5. Laporan Stok Tertinggi
6. Simpan & Keluar
No	Menu	Deskripsi
1	Tambah Bahan/Menu	Menambahkan bahan masakan atau menu harian. Kode harus unik.
2	Lihat Semua Data	Menampilkan semua data bahan/menu beserta stoknya.
3	Edit Stok	Mengubah jumlah stok suatu item berdasarkan kode.
4	Hapus Data	Menghapus bahan/menu tertentu berdasarkan kode.
5	Laporan Stok Tertinggi	Menampilkan daftar bahan/menu dari stok terbanyak ke terkecil.
6	Simpan & Keluar	Menyimpan semua data dan keluar dari program.

6. Format Input
Field	Format	Contoh
Kode	String tanpa spasi, unik	MNU001
Nama	String bebas	Ayam Goreng
Jenis	'bahan' atau 'menu' (harus valid)	menu
Jumlah Stok	Angka bulat positif	25

7. Fitur Optimasi & Error Handling
✅ File Handling menggunakan with open() dan try-except untuk menghindari crash
✅ Pengukuran performa fungsi dengan time.time()
✅ Komentar penjelas di setiap bagian kode untuk kemudahan pembelajaran
✅ Validasi data, seperti kode tidak boleh duplikat dan jenis hanya boleh 'bahan' atau 'menu'
✅ Struktur data menggunakan list of dictionaries yang fleksibel

8. Catatan Tambahan
File warteg_data.json akan terupdate otomatis saat memilih menu Simpan & Keluar.

Jangan mengedit file JSON secara manual agar tidak merusak struktur data.

Jika file tidak ditemukan saat awal program dijalankan, sistem akan mulai dengan data kosong.

9. Saran Pengembangan (Opsional)
💡 Implementasi struktur dictionary untuk pencarian cepat (O(1))
💡 Validasi tambahan agar stok tidak boleh bernilai negatif
💡 Fitur export laporan ke file .csv atau .txt
💡 Tambahkan filter laporan berdasarkan jenis: hanya menu atau hanya bahan
