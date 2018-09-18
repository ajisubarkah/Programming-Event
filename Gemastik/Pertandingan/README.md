# PERTANDINGAN

## Deskripsi
Dalam sebuah pertandingan olahraga, Budi diberikan kesempatan untuk memilih urutan pemain yang harus dilawannya. Asumsikan ada N orang lawan yang masing-masing memiliki tingkat kemahiran Ai. Setelah Budi berhasil mengalahkan pemain ke-i, tingkat kemahirannya akan bertambah sebanyak Bi yang akan digunakan untuk melawan pemain selanjutnya. Perlu diingat bahwa Budi hanya bisa mengalahkan pemain dengan tingkat kemahiran yang lebih rendah atau sama dengan dirinya sendiri. Jika Budi memiliki tingkat kemahiran awal M, tentukan pemain manakah yang harus dilawan Budi secara berurutan sampai dia tidak bisa lagi mengalahkan lawannya sehingga Budi mendapatkan tingkat kemahiran yang maksimal.

## Format Masukan
- Baris pertama dua buah bilangan N dan M (1≤N, M≤100)
- Baris kedua N buah bilangan Ai (1≤Ai≤1000)
- Baris ketiga N buah bilangan Bi (1≤Bi≤1000)

## Format Keluaran
Tingkat kemahiran maksimal yang akan didapatkan Budi.

## Contoh Masukan 1

    4 2
    8 9 3 2
    5 4 1 3

## Contoh Keluaran 1
    
    6

## Contoh Masukan 2
    
    5 3
    8 4 5 6 7
    9 8 7 5 6

## Contoh Keluaran 2
    
    3

## Contoh Masukan 3

    5 9
    2 3 6 7 8
    3 4 2 2 3

## Contoh Keluaran 3

    23

## Batasan
Time limit: 1 s

Memory limit: 32 MB
