# PAK GRANDI

## Deskripsi
Pak Grandi memiliki papan tulis yang besar sekali.
Pak Chanek menantang Pak Grandi untuk melakukan N aksi, yang masing-masing berbentuk:

    P[i] L[i] R[i] K[i]

Makna dari aksi di atas adalah sebagai berikut:
- Jika P[i] = 1: Pak Grandi harus menuliskan bilangan x sebanyak tepat K[i] buah pada papan tulis,
untuk seluruh bilangan bulat L[i] ≤ x ≤ R[i].
- Jika P[i] = 2: Misalkan cnt(x) menyatakan banyaknya bilangan x pada papan tulis. Pak Grandi
harus menghapus bilangan x sebanyak tepat min(cnt(x), K[i]) buah dari papan tulis, untuk seluruh
bilangan bulat L[i] ≤ x ≤ R[i].
Segera setelah melakukan aksi yang diminta, Pak Grandi harus menghitung G[i], yang merupakan bi-
langan bulat positif terkecil yang tidak tertulis pada papan tulis.
Bantulah Pak Grandi untuk melakukan tantangan yang diminta Pak Chanek.

## Format Masukan
Baris pertama berisi sebuah bilangan bulat T yang menyatakan banyaknya kasus uji. Baris-baris berikut-
nya berisi T kasus uji, yang masing-masing diberikan dalam format berikut ini:

    N
    P[1] L[1] R[1] K[1]
    P[2] L[2] R[2] K[2]
    .
    .
    P[N] L[N] R[N] K[N]
    
## Format Keluaran
Untuk setiap kasus uji, keluarkan:

    G[1]
    G[2]
    .
    .
    G[N]

## Contoh Masukan
    
    2
    4
    1 1 1 1
    1 3 3 2
    1 2 2 1
    2 1 1 1
    4
    1 1 5 2
    1 11 15 1
    1 6 10 2
    2 1 15 1

## Contoh Keluaran

    2
    2
    4
    1
    6
    6
    16
    11

Perhatikan bahwa contoh kedua tidak termasuk dalam contoh masukan dan contoh keluaran dari soal
versi mudah.

## Penjelasan
Pada contoh pertama, mula-mula tidak terdapat bilangan pada papan tulis. Terdapat 4 aksi yang
dilakukan oleh Pak Grandi:
- Menuliskan 1 buah bilangan 1: di papan tulis terdapat [1], sehingga G[1] = 2.
- Menuliskan 2 buah bilangan 3: di papan tulis terdapat [1 3 3], sehingga G[2] = 2.
- Menuliskan 1 buah bilangan 2: di papan tulis terdapat [1 3 3 2], sehingga G[3] = 4.
- Menghapus 1 buah bilangan 1: di papan tulis terdapat [3 3 2], sehingga G[4] = 1.

## Batasan
Batasan waktu : 3s

Batasan memori : 256 MB

Batasan yang berlaku untuk versi mudah dan
versi sulit:
- 1 ≤ T ≤ 10
- 1 ≤ P[i] ≤ 2
- 1 ≤ L[i], R[i] ≤ 1.000.000.000
- 1 ≤ K[i] ≤ 1.000.000.000
- 1 ≤ N ≤ 50.000

Batasan khusus versi mudah:
- L[i] = R[i]

Batasan khusus versi sulit:
- L[i] ≤ R[i]