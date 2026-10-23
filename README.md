# Pertemuan 09 - List dan Pengolahan Data Numerik
- Nama: Tantri Widya Solehati
- NIM: 2225250114
- Kelas: 3F
## Tujuan
Mengolah kumpulan data numerik dengan list Python.
## Struktur Program
1. 01_buat_list.py
    - Tujuan:
    Membuat list dan mengetahui jumlah elemennya.
    - Penjelasan
        - nilai = [75, 80, 65, 90, 88] membuat list yang berisi 5 angka.
        - print(nilai) menampilkan seluruh isi list.
        - len(nilai) menghitung banyaknya elemen dalam list.
2. 02_indeks_slicing.py
    - Tujuan
    Mengakses elemen list menggunakan indeks dan slicing.
    - Penjelasan
        - nilai[0] → elemen pertama.
        - nilai[-1] → elemen terakhir.
        - nilai[:3] → tiga elemen pertama.
        - nilai[1:4] → elemen indeks 1 sampai 3.
3. 03_manipulasi_list.py
    - Tujuan:
    Mengubah isi list.
    - Penjelasan
        - Mengubah elemen indeks ke-1
        - Menambah data di akhir
        - Menyisipkan data pada indeks ke-1
4. 04_agregasi_nilai.py
    - Tujuan:
    Menghitung statistik sederhana.
    - Penjelasan
        - sum() menghitung total nilai.
        - len() menghitung jumlah data.
        - min() mencari nilai terkecil.
        - max() mencari nilai terbesar.
5. 05_filter_kelulusan.py
    - Tujuan:
    Melakukan seleksi data menggunakan perulangan dan percabangan.
    - Penjelasan
        - Program memeriksa setiap nilai
        - Nilai yang memenuhi syarat dimasukkan ke list lulus.
6. 06_fungsi_statistik.py
    - Tujuan:
    Membuat fungsi yang menerima parameter list.
    - Penjelasan:
        - Fungsi:
        ```Python
         def rata_rata(data):
        menerima list sebagai parameter.
        - Jika list kosong:
        ```Python
        if len(data) == 0:
        return 0
        - Jika ada isi:
        ```Python
        return sum(data) / len(data)
        Mengembalikan nilai rata-rata.
7. Praktik (analisis_nilai_mahasiswa.py)
    - List nilai digunakan untuk menyimpan data nilai siswa.
    - Banyak Data
    ```Python
    len(nilai)
    ```
    Menghitung jumlah elemen dalam list.
    - Menjumlahkan seluruh nilai dalam list.
    - Menghitung rata-rata
    - Nilai Minimum : Mencari nilai terkecil dalam list
    - Nilai Maksimum: Mencari nilai terbesar dalam list.
    - List Nilai Lulus: Menyeleksi nilai yang lebih besar atau sama dengan 60.
    - Jumlah Lulus: Menghitung banyaknya nilai yang lulus.
    - Jumlah Belum Lulus: Menghitung data yang tidak memenuhi syarat kelulusan.
## Cara Menjalankan
python3 praktik/analisis_nilai_mahasiswa.py
## Test Case
|    Data      | Yang Diperiksa                               | Hasil yang Diharapkan | Hasil Aktual | Status |
|--------------|----------------------------------------------|-----------------------|--------------|--------|
| [60, 70, 80] | Rata-rata                                    | 70.00                 | 70.00        | Sesuai |
| [60, 70, 80] | Minimum / maksimum                           | 60 / 80               | 60 / 80      | Sesuai |
| [60, 70, 80] | Jumlah lulus                                 | 3                     | 3            | Sesuai |
| [59, 60, 61] | Batas kelulusan                              | 2 lulus               | 2 lulus      | Sesuai |
| []           | Penanganan list kosong pada fungsi rata-rata | Tidak error           | Tidak error  | Sesuai |
## Refleksi
- Hal yang dipahami tentang indeks/list:
 List digunakan untuk menyimpan banyak data dalam satu variabel, dan setiap data memiliki posisi yang disebut indeks. Indeks dimulai dari 0, sehingga elemen pertama berada pada indeks 0, elemen kedua pada indeks 1, dan seterusnya. Dengan indeks, kita dapat mengambil atau mengubah data tertentu dalam list.

- Kesalahan yang berhasil diperbaiki:
 Saya sempat mengalami kesalahan pada proses pengecekan nilai lulus karena penulisan kondisi atau indentasi pada perulangan tidak tepat. Setelah diperbaiki, program dapat menyeleksi nilai yang memenuhi batas kelulusan dengan benar dan menampilkan jumlah siswa yang lulus maupun belum lulus secara akurat.