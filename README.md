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

