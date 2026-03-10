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
