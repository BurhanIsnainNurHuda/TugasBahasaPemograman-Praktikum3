# TugasBahasaPemograman-Praktikum3
# Flowchart:
﻿![WhatsApp Image 2024-10-27 at 09 03 52](https://github.com/user-attachments/assets/3b5f79df-da1b-4e95-a34f-90fd5ddbfac4)

# Python Code:
![IMG_20241027_102748](https://github.com/user-attachments/assets/44bacba6-daa0-46d1-9a10-d0257afd473c)

Penjelasan:
1. Start
2. Input N: Input jumlah angka yang akan diproses.
3. Initialize max = 0: Inisialisasi variabel max dengan nilai 0, yang akan digunakan untuk menyimpan angka terbesar yang ditemukan.
4. Loop dari i = 1 ke N: Memulai sebuah loop yang akan berulang sebanyak N kali, dengan i sebagai counter loop.
5. Input bilangan i: Pada setiap iterasi loop, program meminta input untuk angka ke-i.
6. Jika bilangan i > maks: Memeriksa apakah angka yang baru diinputkan (bilangan i) lebih besar dari nilai maks yang sudah ada.
7. Yes: Jika bilangan i lebih besar dari maks, maka:
          max = bilangan i: Nilai max diupdate menjadi bilangan i.
8. No: Jika bilangan i tidak lebih besar dari maks, maka program melanjutkan ke iterasi loop selanjutnya.
9. Print max sebagai angka terbesar: Setelah loop selesai, program akan menampilkan nilai max sebagai angka terbesar yang ditemukan dari semua angka yang diinputkan.
10. End

# Output:
![IMG_20241027_103406](https://github.com/user-attachments/assets/8fb66cbb-e558-482e-82ff-f5c153384301)

# Latihan 1

1. Penggunaan end

Dalam Python, fungsi '`print()`' memiliki parameter '`end`' yang digunakan untuk menentukan karakter yang akan ditambahkan di akhir output. Secara default, '`end`' adalah `'/n'`, yang berarti setiap panggilan '`print()`' akan diakhiri dengan baris baru. Dan, dapat diubah sesuai kebutuhan.

Input:

    print('A', end='')  # Mencetak 'A' tanpa baris baru
    print('B', end='')  # Mencetak 'B' tanpa baris baru
    print('C', end='')  # Mencetak 'C' tanpa baris baru
    print()              # Mencetak baris baru
    print('X')          # Mencetak 'X' di baris baru
    print('Y')          # Mencetak 'Y' di baris baru
    print('Z')          # Mencetak 'Z' di baris baru

Output:

    ABC
    X
    Y
    Z
    
2. Penggunaan separator
Dalam Python, parameter '`sep`' dalam fungsi '`print()`' digunakan untuk menentukan karakter yang akan digunakan sebagai pemisah antara argumen yang dicetak. Secara default, '`sep`' adalah '`' '`', yang berarti setiap argumen akan dipisahkan oleh spasi.

Input:

    w, x, y, z = 10, 15, 20, 25

    print(w, x, y, z)                # Output: 10 15 20 25 (default separator: space)
    print(w, x, y, z, sep=',')       # Output: 10,15,20,25 (separator: comma)
    print(w, x, y, z, sep='')        # Output: 10152025 (no separator)
    print(w, x, y, z, sep=':')       # Output: 10:15:20:25 (separator: colon)
    print(w, x, y, z, sep='-----')   # Output: 10-----15-----20-----25 (separator: '-----')

Output:

    10 15 20 25
    10,15,20,25
    10152025
    10:15:20:25
    10-----15-----20-----25

3. Format String (String Formatting)
String formatting di Python untuk menyajikan output dengan cara yang lebih terstruktur dan mudah dibaca. Dalam contoh dibawah, Saya mencetak angka dan pangkat dari 10. Lihat bagaimana saya bisa menggunakan string formatting untuk membuat output lebih rapi.

Input:

    Menggunakan f-string (Python 3.6+)
      for i in range(11):
      print(f"{i} {10**i}")

Output:

    0 1
    1 10
    2 100
    3 1000
    4 10000
    5 100000
    6 1000000
    7 10000000
    8 100000000
    9 1000000000
    10 10000000000      

4. Format String dengan Penyesuaian Lebar Kolom
Ini sangat berguna ketika ingin mencetak tabel atau data yang terformat dengan rapi.

Input:

    print('{0:>3} {1:>16}'.format(0, 10**0))
    print('{0:>3} {1:>16}'.format(1, 10**1))
    print('{0:>3} {1:>16}'.format(2, 10**2))
    print('{0:>3} {1:>16}'.format(3, 10**3))
    print('{0:>3} {1:>16}'.format(4, 10**4))
    print('{0:>3} {1:>16}'.format(5, 10**5))
    print('{0:>3} {1:>16}'.format(6, 10**6))
    print('{0:>3} {1:>16}'.format(7, 10**7))
    print('{0:>3} {1:>16}'.format(8, 10**8))
    print('{0:>3} {1:>16}'.format(9, 10**9))
    print('{0:>3} {1:>16}'.format(10, 10**10))

Output:

    0                1
    1                10
    2               100
    3              1000
    4             10000
    5            100000
    6           1000000
    7          10000000
    8         100000000
    9        1000000000
    10      10000000000

# Latihan 2

# Code Asli (Yang Salah atau Eror)


    a = input("masukkan nilai a:")
    b = input("masukkan nilai b:")
    print("variable a=", a)
    print("variable b=", b)
    print("hasil penggabungan (1}&{0}=%d".format(a, b) %(a+b))
    # konversi nilai variable
    a = int(a)
    b = int(b)
    print("hasil penjumlahan [1]+[0]=%d".format(a, b) %(a + b))
    print("hasil pembagian (1)/(B)=%d".format(a, b) %(a / b))

# Masalah dalam Code Asli yang eror
    1. Penggunaan `format()` dan `%` secara bersamaan: Kode ini mencoba menggunakan metode `format()` dan operator `%` pada saat yang sama, yang tidak akan berfungsi dengan baik.
    2. Tipe Data Input: Fungsi `input()` mengembalikan nilai dalam bentuk string. Anda perlu mengonversi nilai tersebut ke tipe data yang sesuai sebelum melakukan operasi aritmatika.
    3. Format String yang Tidak Sesuai: Format string tidak ditulis dengan benar, yang dapat menyebabkan kesalahan saat run.    

# Code yang benar (Tidak Eror)

    #Meminta input dari pengguna
      a = input("masukkan nilai a: ")
      b = input("masukkan nilai b: ")

    #Menampilkan nilai a dan b
      print("variable a =", a)
      print("variable b =", b)

    #Mengonversi a dan b ke tipe data yang sesuai (misalnya, int)
      try:
      a = int(a)
      b = int(b)

    # Menampilkan hasil penggabungan
      print("hasil penggabungan (1) + (0) = {}".format(a + b))

    # Menampilkan hasil penjumlahan
      print("hasil penjumlahan [1] + [0] = {}".format(a + b))

    # Menampilkan hasil pembagian
      if b != 0:  # Memastikan tidak membagi dengan nol
        print("hasil pembagian (1) / (0) = {}".format(a / b))
      else:
        print("Pembagian dengan nol tidak diperbolehkan.")
      except ValueError:
      print("Masukkan nilai yang valid (angka).")

Contoh 1: Input Valid
Input:

    masukkan nilai a: 10
    masukkan nilai b: 5
    
Output:

    variable a = 10
    variable b = 5
    hasil penggabungan (1) + (0) = 15
    hasil penjumlahan [1] + [0] = 15
    hasil pembagian (1) / (0) = 2.0
      
Penjelasan:

    Pengguna memasukkan `10` untuk variabel `a` dan `5` untuk variabel `b`.
    Program menampilkan nilai dari `a` dan `b`.
    Program mengonversi `a` dan `b` menjadi tipe data `int` dan menjumlahkannya.
    Hasil penjumlahan `10 + 5` adalah `15`.
    Hasil pembagian `10 / 5` adalah `2.0`.
