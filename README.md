# 1. penjelasan konsep array

<img width="556" height="70" alt="image" src="https://github.com/user-attachments/assets/b445997a-00bd-45ee-aaef-db8a325659a3" />

Basis kode ini digunakan untuk mendefinisikan sebuah array (list) kosong yang akan digunakan untuk menyimpan data nila mahasiswa, disini saya megunakan kalimat nilai_mahasiswa swbagai list. 

Tanda # hanya untuk menujukkan komentar penjelas.
(nilai_mahasiswa) untuk nama variabel untuk menyimpan data nilai mahasiswa dan memudahkan pengolahan data.
(=) untuk operator penugasan untuk memberikan nilai ke variabel.

<img width="642" height="83" alt="image" src="https://github.com/user-attachments/assets/41f71cd6-8f9d-4cb4-9b2e-9f4e1d7bd1a6" />

Perulangan for i in range(10) berfungsi untuk menjalankan proses sebanyak 10 kali, sehingga pengguna dapat memasukkan nilai untuk 10 mahasiswa.
Pada setiap perulangan, program meminta input menggunakan input() dengan pesan "masukkan nilai mahasiswa ke-{i+1}", di mana i+1 digunakan agar penomoran mahasiswa 	dimulai dari 1, bukan dari 0.
Nilai yang dimasukkan kemudian diubah menjadi tipe data integer menggunakan int() agar dapat diproses sebagai angka dalam program.

Setelah itu, nilai tersebut disimpan ke dalam list nilai_mahasiswa menggunakan metode append(), yang berfungsi untuk menambahkan data baru ke dalam array.
Dengan demikian, setelah perulangan selesai, list nilai_mahasiswa akan berisi 10 nilai mahasiswa yang telah dimasukkan oleh pengguna.

<img width="545" height="111" alt="image" src="https://github.com/user-attachments/assets/a55033c1-23ed-496d-a4e1-d7950f5deff0" />

Baris print("Nilai mahasiswa:", nilai_mahasiswa) berfungsi untuk menampilkan seluruh data nilai yang tersimpan di dalam array nilai_mahasiswa, sehingga pengguna dapat melihat semua nilai yang telah diinput sebelumnya.

print("Nilai Tertinggi:", max(nilai_mahasiswa)) digunakan untuk mencari dan menampilkan nilai paling besar dalam array dengan menggunakan fungsi max(). Fungsi ini akan memeriksa seluruh elemen dalam list dan mengambil nilai yang paling tinggi.

print("Nilai Terendah:", min(nilai_mahasiswa)) digunakan untuk mencari dan menampilkan nilai paling kecil dalam array dengan menggunakan fungsi min(). Fungsi ini akan memeriksa semua data dalam array dan mengambil nilai yang paling rendah.

<img width="646" height="322" alt="image" src="https://github.com/user-attachments/assets/b882147b-5ae8-45e8-90bd-0f20ad7d6bdd" />

import matplotlib.pyplot as plt berfungsi untuk mengimpor library Matplotlib, yaitu library yang digunakan untuk membuat grafik atau visualisasi data di Python.

plt.figure() digunakan untuk membuat area atau kanvas baru tempat grafik akan ditampilkan.

kategori = ["Nilai Tertinggi", "Nilai Terendah"] dibuat sebuah array (list) yang berisi dua kategori yang akan ditampilkan pada sumbu horizontal grafik, yaitu nilai tertinggi dan nilai terendah.

nilai_tertinggi = max(nilai_mahasiswa) digunakan untuk mencari nilai terbesar dari array nilai_mahasiswa, sedangkan nilai_terendah = min(nilai_mahasiswa) digunakan untuk mencari nilai terkecil dari array tersebut.

data = [nilai_tertinggi, nilai_terendah] membuat array baru yang berisi dua data yaitu nilai tertinggi dan nilai terendah yang akan digunakan sebagai tinggi batang pada grafik.

Baris plt.bar(kategori, data, color=["blue", "yellow"]) digunakan untuk membuat grafik batang, di mana kategori menjadi label pada sumbu X dan data menjadi nilai pada sumbu Y, sedangkan warna batang diatur menjadi biru dan kuning.

plt.title("Grafik Nilai Tertinggi dan Terendah") berfungsi untuk memberikan judul pada grafik agar lebih mudah dipahami.

Baris plt.ylabel("Jumlah Mahasiswa") digunakan untuk memberi label pada sumbu Y.

plt.ylim(0,100) digunakan untuk mengatur batas nilai pada sumbu Y dari 0 sampai 100, sesuai dengan rentang nilai mahasiswa.

plt.show() digunakan untuk menampilkan grafik yang telah dibuat ke layar sehingga pengguna dapat melihat visualisasi perbandingan nilai tertinggi dan nilai terendah.

<img width="676" height="89" alt="image" src="https://github.com/user-attachments/assets/a5bbc107-09dc-4560-aaca-e234d6475805" />

Baris print("nilai_mahasiswa:", nilai_mahasiswa) berfungsi untuk menampilkan semua nilai mahasiswa yang tersimpan dalam array.
sum(nilai_mahasiswa) digunakan untuk menjumlahkan seluruh nilai, dan len(nilai_mahasiswa) digunakan untuk menghitung jumlah data.
Hasil penjumlahan tersebut kemudian dibagi dengan jumlah data untuk mendapatkan nilai rata-rata mahasiswa.

<img width="500" height="265" alt="image" src="https://github.com/user-attachments/assets/d9b7480f-643c-4299-99e4-042f28777b75" />

Pertama, variabel lulus dan tidak_lulus diinisialisasi dengan nilai 0 untuk menyimpan jumlah masing-masing kategori.

Perulangan for n in nilai_mahasiswa digunakan untuk memeriksa setiap nilai yang ada di dalam array.

Jika nilai n >= 60, maka mahasiswa dianggap lulus sehingga variabel lulus akan bertambah satu (lulus += 1).

Jika nilai kurang dari 60, maka mahasiswa dianggap tidak lulus, sehingga variabel tidak_lulus akan bertambah satu (tidak_lulus += 1).

Terakhir, print() digunakan untuk menampilkan jumlah mahasiswa yang lulus dan tidak lulus berdasarkan data nilai yang ada dalam array.

<img width="530" height="285" alt="image" src="https://github.com/user-attachments/assets/59105d0f-97a4-403c-a512-350bc083e8eb" />

Baris import matplotlib.pyplot as plt berfungsi untuk mengimpor library Matplotlib yang digunakan untuk membuat visualisasi grafik.

plt.figure() digunakan untuk membuat area grafik baru sebelum menampilkan diagram.

Kategori = ["Lulus", "Tidak Lulus"] dibuat array (list) yang berisi dua kategori yang akan ditampilkan pada sumbu X grafik.

Kemudian data = [lulus, tidak_lulus] merupakan array yang berisi jumlah mahasiswa yang lulus dan tidak lulus berdasarkan perhitungan sebelumnya.

Baris plt.bar(kategori, data, color=["green", "red"]) digunakan untuk membuat grafik batang, di mana kategori menjadi label pada sumbu X dan data menjadi tinggi batang pada sumbu Y, dengan warna hijau untuk lulus dan merah untuk tidak lulus.

Selanjutnya plt.title("Grafik Data Kelulusan Mahasiswa") digunakan untuk memberikan judul pada grafik, dan plt.ylabel("Jumlah Mahasiswa") untuk memberi label pada sumbu Y.

Baris plt.ylim(0,10) digunakan untuk mengatur batas nilai pada sumbu Y dari 0 sampai 10 agar grafik lebih jelas.

Terakhir plt.show() berfungsi untuk menampilkan grafik ke layar sehingga pengguna dapat melihat visualisasi jumlah mahasiswa yang lulus dan tidak lulus.

# 2. Screenshot Hasil Eksekusi
# input 10 nilai mahasiswa

<img width="779" height="437" alt="image" src="https://github.com/user-attachments/assets/caf5f789-4bf0-4404-b7e7-2bcd1aff53f1" />


# nilai tertinggi dan terendah
<img width="777" height="218" alt="image" src="https://github.com/user-attachments/assets/bdbe937e-e676-4bba-a3fc-440e77b3f6f5" />


# Hitung rata-rata
<img width="740" height="155" alt="image" src="https://github.com/user-attachments/assets/65e5d3aa-406b-4e8a-a10a-5c22315bba4d" />


# Hitung jumlah mahasiswa lulus (>= 60)

<img width="608" height="345" alt="image" src="https://github.com/user-attachments/assets/56182e1a-d716-4827-ab5f-533a385fd642" />


# Grafik untuk menggambarkan nilai tertinggi dan terendah

<img width="707" height="330" alt="image" src="https://github.com/user-attachments/assets/0f730d93-b86c-4a75-bbaf-7b4da029b978" />

<img width="895" height="585" alt="image" src="https://github.com/user-attachments/assets/c0c06862-f6ad-492d-ae9e-3a141e16376e" />


# Grafik untuk menggambarkan data kelulusan

<img width="789" height="293" alt="image" src="https://github.com/user-attachments/assets/4963d245-349b-4832-a956-2f9d8b0e8e3a" />

<img width="982" height="582" alt="image" src="https://github.com/user-attachments/assets/973ebc44-1627-4c2f-9729-f3f38d4b2bc2" />

# 3. Analisis Kompleksitas

Pada bagian input nilai mahasiswa, program menggunakan perulangan for untuk memasukkan nilai ke dalam list. Karena proses ini dilakukan sebanyak jumlah data mahasiswa (n), maka kompleksitas waktunya adalah O(n).

Pada bagian mencari nilai tertinggi dan nilai terendah menggunakan fungsi max() dan min(). Kedua fungsi ini harus memeriksa seluruh data dalam list sehingga kompleksitas waktunya adalah O(n).

Selanjutnya pada perhitungan rata-rata, program menggunakan sum() untuk menjumlahkan semua nilai dan len() untuk menghitung jumlah data. Karena sum() memproses semua data, maka kompleksitasnya adalah O(n).

Pada proses menghitung jumlah mahasiswa yang lulus dan tidak lulus, program menggunakan perulangan untuk memeriksa setiap nilai. Karena semua data diperiksa satu per satu, maka kompleksitasnya juga O(n).

Sedangkan pada pembuatan grafik menggunakan matplotlib, data yang ditampilkan hanya beberapa kategori saja sehingga kompleksitas waktunya adalah O(1).

# 4. Refleksi Pembelajaran
Saya memahami bagaimana menggunakan array (list) untuk menyimpan dan mengelola data.

Saya juga belajar cara melakukan input data menggunakan perulangan dan menyimpan data tersebut ke dalam array dengan fungsi append().

Memahami cara melakukan pengolahan data sederhana, seperti mencari nilai tertinggi dengan max(), nilai terendah dengan min(), dan menghitung rata-rata menggunakan sum() dan len().

Belajar membuat visualisasi data menggunakan library Matplotlib, seperti grafik batang untuk menampilkan perbandingan data nilai dan kelulusan mahasiswa. Selain itu juga belajar cara merubah warna pada grafik menggunakan plt.bar(kategori, data, color=[].
