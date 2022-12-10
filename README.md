# Nama : Roswanda Nuraini

# NIM : 312210328

# Kelas : TI.22.A.3

# Praktikum 8 

# (Penggunaan Class untuk Menampilkan Daftar Nilai Mahasiswa)

# Hasil Source Code Praktikum 8

![Screenshot (215)](https://user-images.githubusercontent.com/115516632/206838472-36064032-4621-456b-ac3c-ea702a9e2b4d.png)

![Screenshot (216)](https://user-images.githubusercontent.com/115516632/206838580-b5c2372b-a248-4da0-ae24-8f3f42d4ba47.png)

![Screenshot (217)](https://user-images.githubusercontent.com/115516632/206838673-2c3ae37e-2798-4394-ac26-fccbecbec693.png)

![Screenshot (218)](https://user-images.githubusercontent.com/115516632/206838913-9589b5fc-6f00-4ad2-85f0-7e432d00fb69.png)

![Screenshot (219)](https://user-images.githubusercontent.com/115516632/206839178-923f0803-c7c5-40df-b343-59b5f77e0ef4.png)

# Penjelasan Praktikum 8 beserta Hasil Output

1. Pertama kita mendeklarasikan sebuah class Mahasiswa yang didalamnya terdapat atribut NIM, Nama, nilai Tugas, nilai UTS dan nilai UAS.

2. Jangan lupa, untuk mendeklarasikan sebuah class didalam OOP kita harus gunakan def__init__ dan juga self.

            class mahasiswa:
                def __init__(self, nim, nama, tugas, uts, uas):
                    self.nim = nim
                    self.nama = nama
                    self.tugas = tugas
                    self.uts = uts
                    self.uas = uas
          
3. Seperti biasa, deklarasikan satu dictionary kosong sebagai tempat menyimpan data-data yang sudah kita input. Ada 5 list kosong yang nanti isinya yaitu NIM, Nama, nilai tugas, nilai UTS dan nilai UAS.

        data = mahasiswa([],[],[],[],[])

4. Kita akan buat beberapa method untuk menambahkan, menampilkan, menghapus, mengubah data mahasiswa. Pertama membuat method tambah(), method ini berfungsi untuk menambahkan data. Dalam method ini kita menggunakan append() supaya data yang terakhir ditambahkan, ada di urutan list paling akhir.

        def tambah(self,nim,nama,tugas,uts,uas):
                data.nim.append(nim)
                data.nama.append(nama)
                data.tugas.append(tugas)
                data.uts.append(uts)
                data.uas.append(uas)
          
 Ini tampilan jika kita menjalankan method Tambah() :   
 
 ![Screenshot (220)](https://user-images.githubusercontent.com/115516632/206839890-dc579c10-5a94-417e-8f46-afe1db560036.png)

5. Membuat method lihat(), gunanya untuk menampilkan seluruh data yang sudah kita tambahkan tadi. Kalau tidak ada data sama sekali, maka akan muncul tulisan TIDAK ADA DATA.

        def lihat(self):
                for i in range(len(data.nama)):
                    print("|", i+1, "  |", end="")
                    print('{0:<25}'.format(self.nama[i]), end="")
                    print("|", self.nim[i], end="")
                    print(" |", self.tugas[i], end="")
                    print("    |", self.uts[i], end="")
                    print("  |", self.uas[i], " | ", end="")
                    print(f'{((self.tugas[i]*30/100) + (self.uts[i]*35/100) + (self.uas[i]*35/100)) :.2f}', " |")

Ini tampilan jika kita menjalankan method Lihat() :          
          
![Screenshot (221)](https://user-images.githubusercontent.com/115516632/206840241-6026f3c3-bf36-4789-9151-ab65406c6938.png)
 
6. Membuat method ubah() yang fungsinya untuk mengubah data. jika method ini dipanggil, maka data Nama, NIM, nilai tugas, nilai UTS, nilai UAS index nomor - (no) akan diubah sesuai dengan inputan dari user. Index ke - (no) akan dicari secara otomatis sesuai dengan nama yang ingin diubah oleh user.       

        def ubah(self,nim,nama,tugas,uts,uas):
                self.nim[no] = nim
                self.nama[no] = nama
                self.tugas[no] = tugas
                self.uts[no] = uts
                self.uas[no] = uas
        
Ini tampilan jika kita menjalankan method Ubah() :

![Screenshot (222)](https://user-images.githubusercontent.com/115516632/206840619-1f1691c9-0cf1-4b2d-ad67-9cb7db18ee5e.png)

![Screenshot (223)](https://user-images.githubusercontent.com/115516632/206841047-1abcc9cb-5d1a-443a-a3b5-738acb2a7747.png)

7. Selanjutnya, kita buat method hapus(). Gunanya adalah menghapus data berdasarkan nama. Kita bisa menggunakan del untuk menghapus datanya. Seperti tadi, nomor index list yang akan dihapus disesuaikan dengan inputan dari user. Yaitu index nomor ke - (no).

            def hapus(self):
                    del self.nim[no]
                    del self.nama[no]
                    del self.tugas[no]
                    del self.uts[no]
                    del self.uas[no]

Ini tampilan jika kita menjalankan method Hapus() :

![Screenshot (224)](https://user-images.githubusercontent.com/115516632/206841063-3f9400dc-0c40-4546-9f52-85ed3822a945.png)

8. Terakhir, kita buat method keluar(). Gunanya adalah untuk keluar dari program yang telah kita jalankan sebelumnya.

Ini tampilan jika kita menjalankan method Keluar()

![Screenshot (225)](https://user-images.githubusercontent.com/115516632/206841453-c77fce96-e16f-475b-b8d6-10d4adba155a.png)

# Hasil Flowchart Praktikum 8

![Flowchart 8](https://user-images.githubusercontent.com/115516632/206842211-fcd752c9-d145-4e92-901b-85595ae344e2.png)



