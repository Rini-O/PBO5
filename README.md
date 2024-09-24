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
        . Penjelasan Java Swing
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
🔗 Java Swing adalah toolkit GUI (Graphical User Interface) yang merupakan bagian dari Java Foundation Classes (JFC). java swing juga dapat terhubung dengan database dengan mengoprasikan CRUD. 

🔗 Komponen yang digunakan  

- JFrame: jendela utama aplikasi yang menampung semua komponen lainnya.
  - Nama variabel: Mahasiswa
   
- JLabel: Menampilkan teks statis yang berfungsi sebagai label untuk field input (NIM, NAMA, PROGRAM STUDI).
  - Nama variabel: jLabel1, jLabel2, jLabel3, jLabel4
   
- JTextField: Field input untuk menerima data dari pengguna, seperti NIM, nama mahasiswa, dan program studi.
  - Nama variabel: txtNim, txtNama, txtPd

- JToggleButton : Tombol yang digunakan untuk melakukan operasi CRUD (Create, Read, Update, Delete) pada data mahasiswa.
  - Nama variabel: btnInsert, btnUpdate, btnDelete

- JTable: Menampilkan daftar mahasiswa dalam bentuk tabel, termasuk NIM, nama, dan program studi.
  - Nama variabel: tblMahasiswa
 
- JScrollPane: Menyediakan scroll bar untuk tabel mahasiswa agar pengguna dapat menggulir jika data melebihi ukuran tampilan.
  - Nama variabel: jScrollPane1
 
🔗 CRUD 
- Create (Insert)
  - Metode: btnInsertActionPerformed
  - Proses:
    1. Memeriksa apakah semua field diisi.
    2. Menghubungkan ke database menggunakan JDBC.
    3. Menyiapkan pernyataan SQL untuk menambahkan data mahasiswa baru ke tabel.
    4. Menjalankan pernyataan SQL dan melakukan commit untuk menyimpan perubahan.
    5. Menampilkan pesan sukses atau gagal kepada pengguna.
       
- Read (Show)
  - Metode: showTable
  - Proses:
    1. Menghubungkan ke database dan mengambil semua data mahasiswa.
    2. Mengatur model tabel (tblMahasiswa) untuk menampilkan hasil query.
    3. Menutup koneksi setelah data ditampilkan.
       
- Update
  - Metode: btnUpdateActionPerformed
  - Proses:
    1. Memeriksa apakah semua field diisi.
    2. Menghubungkan ke database dan menyiapkan pernyataan SQL untuk memperbarui data mahasiswa berdasarkan NIM.
    3. Menjalankan pernyataan SQL dan memberikan umpan balik kepada pengguna mengenai keberhasilan atau kegagalan pembaruan.
       
- Delete
  - Metode: btnDeleteActionPerformed
  - Proses:
    1. Mengambil NIM dari field input untuk menentukan data mana yang akan dihapus.
    2. Meminta konfirmasi dari pengguna sebelum melanjutkan penghapusan.
    3. Menghubungkan ke database dan menyiapkan pernyataan SQL untuk menghapus data mahasiswa.
    4. Menjalankan pernyataan SQL dan menutup koneksi setelah selesai.

## 📝 Kesimpulan
Laporan pratikum ini menjelaskan pengembangan aplikasi desktop menggunakan Java Swing untuk mengelola data mahasiswa. Aplikasi ini memungkinkan pengguna untuk melakukan operasi CRUD (Create, Read, Update, Delete) dengan antarmuka pengguna yang intuitif dan responsif. 
 



  
