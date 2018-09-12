# BERBAGI LAWAKAN

## Deskripsi
Suatu komunitas pelawak terdiri atas N anggota, yang dinomori dari 1 hingga N. Setiap pelawak memiliki
standar tingkat kelucuan humor masing-masing. Pelawak ke-i menyukai sebuah lawakan apabila tingkat
kelucuan lawakan tersebut berada di antara A[i] hingga B[i], inklusif.
Setiap pelawak memiliki akun media sosial. Akun media sosial setiap pelawak memiliki oleh nol atau
lebih pengikut. Terdapat M informasi pengikut akun media sosial, yang masing-masing menyatakan
bahwa akun media sosial pelawak U[i] diikuti oleh akun media sosial pelawak V[i].
Pelawak-pelawak tersebut senang menuliskan lawakan pada akun media sosial masing-masing. Setiap
kali seorang pelawak menuliskan lawakan, pengikut-pengikutnya di media sosial akan langsung membaca
lawakan tersebut. Untuk setiap pengikut, jika ia menyukai lawakan tersebut tanpa peduli apakah ia
sudah pernah menulisnya, maka ia akan menulis ulang lawakan tersebut keesokan harinya pada akun
media sosialnya.
Sebuah lawakan dikatakan abadi apabila lawakan tersebut akan terus beredar dari hari ke hari, tanpa
pernah berakhir.
Sekarang, terdapat Q buah pertanyaan. Pertanyaan ke-i berbunyi: jika pelawak X[i] menulis lawakan
dengan tingkat kelucuan H[i], apakah lawakan tersebut akan menjadi abadi?

## Format Masukan
Masukan diberikan dalam format berikut ini:

    N M
    A[1] A[2] .. A[N]
    B[1] B[2] .. B[N]
    U[1] V[1]
    U[2] V[2]
    .
    .
    U[M] V[M]
    Q
    X[1] H[1]
    X[2] H[2]
    .
    .
    X[Q] H[Q]

## Format Keluaran
Keluarkan Q buah baris. Baris ke-i berisi jawaban dari pertanyaan ke-i, yaitu salah satu dari:
• “Ya”, apabila akan menjadi abadi.
• “Tidak”, apabila tidak akan menjadi abadi.

## Contoh Masukan 1
    
    6 6
    0 0 0 0 0 0
    100 100 100 100 100 100
    1 2
    1 3
    2 4
    4 5
    5 2
    3 6
    3
    1 50
    2 30
    3 10

## Contoh Keluaran 1
   
    Ya
    Ya
    Tidak

## Penjelasan Contoh Masukan dan Keluaran 1
Pada pertanyaan pertama dan kedua, lawakan akan beredar pada pelawak-pelawak {2, 4, 5} secara
abadi.
Pada pertanyaan ketiga, lawakan akan dibaca oleh pelawak 6 dan ia tulis ulang pada keesokan harinya.
Sayangnya, tidak ada seorang pun yang membacanya. Maka, persebaran lawakan ini berakhir.

## Contoh Masukan 2

    5 5
    50 10 80 25 80
    99 90 90 90 95
    1 2
    1 3
    2 4
    4 5
    5 2
    3
    1 85
    2 50
    5 85

## Contoh Keluaran 2

    Ya
    Tidak
    Ya

Perhatikan bahwa contoh kedua ini tidak termasuk dalam contoh masukan dan contoh keluaran dari soal
versi mudah.

## Penjelasan Contoh Masukan dan Keluaran 2
Pada pertanyaan pertama, lawakan akan beredar pada pelawak-pelawak {2, 4, 5} secara abadi.
Pada pertanyaan kedua, lawakan akan dibaca oleh pelawak 4 dan ia tulis ulang pada keesokan harinya.
Pelawak 5 akan membacanya, tetapi tidak menuliskan ulang. Maka, persebaran lawakan ini berakhir.
Pada pertanyaan ketiga, lawakan akan beredar pada pelawak-pelawak {2, 4, 5} secara abadi.

## Batasan
Batasan waktu : 2s

Batasan memori : 64 MB

Batasan yang berlaku untuk versi mudah dan
versi sulit:
• 1 ≤ N ≤ 50.000
• 1 ≤ M ≤ 50.000
• 1 ≤ Q ≤ 50.000
• 1 ≤ U[i], V[i] ≤ N
• U[i] 6 = V[i]
• (U[i], V[i]) 6 = (U[j], V[j]) untuk i 6 = j
• 1 ≤ X[i] ≤ N
• 0 ≤ H[i] ≤ 100

Batasan khusus versi mudah:
• A[i] = 0
• B[i] = 100

Batasan khusus versi sulit:
• 0 ≤ A[i] ≤ B[i] ≤ 100