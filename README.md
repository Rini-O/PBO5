# 📚 Laporan Pratikum Pemrograman Berorientasi Objek

Selamat datang di laporan pratikum **Pemrograman Berorientasi Objek**! 🎉😄

## 📖 Deskripsi

Laporan ini membuat aplikasi menggunakan Java Swing untuk menampilkan dan mengelola data mahasiswa dalam bentuk tabel yang mencakup NIM, Nama, dan Program Studi dengan melakukan operasi CRUD  (Create, Read, Update, Delete).💻✨

## 📋 Topic
        📌 DbUtils
        . Penjelasan mengenai kelas DbUtils.
        . Metode untuk mengonversi `ResultSet` menjadi `TableModel`.
        . Langkah-Langkah 
        
        📌 Java Swing
        . Deskripsi tentang antarmuka pengguna.
        . Komponen yang digunakan dalam aplikasi.
        . Operasi CRUD menggunakan Java Swing.

## 📦DbUtils 
🔗 Kelas DbUtilsmerupakan utilitas yang diguakan untuk mengonversi objek ResultSet dari database menjadi model tabel yang dapat digunakan dalam komponen GUI, seperti tabel di Java Swing.

🔗 Metode utama dalam kelas DbUtils  yaitu resultSetToTableModel. Metode ini mengambil objek ResultSet kemudian mengonversinya menjadi objek TableModel. proses ini dilakukan untuk mengisi data dalam tabel Swing.

🔗 Langkah - langkah :
- Mengambil Metadata Menggunakan `ResultSetMetaData` untuk mendapatkan jumlah kolom dan nama kolom dari `ResultSet`.
- Melakukan Iterasi melalui kolom untuk menyimpan nama kolom dalam `Vector`.
- Melakukan loop untuk mengiterasi setiap baris dalam `ResultSet`, kemudian menyimpan nilai kolom dalam vector baru untuk setiap baris.
- Setelah semua data terkumpul, kemudian mengembalikan objek `DefaultTableModel` yang siap digunakan untuk mengisi tabel di Swing.

## 🎨Java Swing 

  
