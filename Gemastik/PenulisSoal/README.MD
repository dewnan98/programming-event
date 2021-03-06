# PENULIS SOAL

## Deskripsi
Tim soal Gemastik 2017 terdiri atas N penulis soal. Saat ini, penulis ke-i sedang bekerja pada P [i]
perusahaan. Terdapat paling banyak 50 perusahaan tempat para penulis soal bekerja, dinomori dari 1
hingga 50. Penulis ke-i bekerja pada perusahaan-perusahaan C[i][1], C[i][2], . . . , C[i][P [i]].
Untuk paket soal penyisihan, penulis ke-i menyumbang S[i] soal. Setelah kontes berakhir, rencananya
akan diumumkan ”pemilik” dari setiap soal. Pemilik soal didefinisikan sebagai salah satu dari:
- penulis soal tersebut, atau
- salah satu dari perusahaan tempat sang penulis soal bekerja.
Tingkat keragaman paket soal didefinisikan sebagai banyaknya pemilik soal yang berbeda. Pak Chanek,
sebagai ketua tim soal, ingin agar tingkat keragaman paket soal penyisihan sebesar mungkin.
Bantulah Pak Chanek menentukan tingkat keragaman maksimum tersebut!

## Format Masukan
Baris pertama berisi sebuah bilangan bulat T yang menyatakan banyaknya kasus uji. Baris-baris berikut-
nya berisi T kasus uji, yang masing-masing diberikan dalam format berikut ini:
```xml
N
S[1] S[2] .. S[N]
P[1] C[1][1] C[1][2] .. C[1][P[1]]
P[2] C[2][1] C[2][2] .. C[2][P[2]]
.
.
P[N] C[N][1] C[N][2] .. C[N][P[N]]
```
## Format Keluaran
Untuk setiap kasus uji, keluarkan sebuah baris berisi tingkat keragaman maksimum.

## Contoh Masukan
```xml
2
3
2 2 2
1 42
2 42 7
0
3
2 2 1
1 42
1 42
0
```
## Contoh Keluaran
```xml
5
4
```

## Penjelasan
Untuk contoh pertama, salah satu cara optimal adalah:
- 2 soal dari penulis 1 dimiliki oleh {Penulis 1, Perusahaan 42}.
- 2 soal dari penulis 2 dimiliki oleh {Penulis 2, Perusahaan 7}.
- 2 soal dari penulis 3 dimiliki oleh {Penulis 3, Penulis 3}.
Himpunan pemilik soal berbeda adalah {Penulis 1, Perusahaan 42, Penulis 2, Perusahaan 7, Penulis 3},
yang memiliki tingkat keragaman 5.
Untuk contoh kedua, salah satu cara optimal adalah:
- 2 soal dari penulis 1 dimiliki oleh {Penulis 1, Perusahaan 42}.
- 2 soal dari penulis 2 dimiliki oleh {Penulis 2, Perusahaan 42}.
- 1 soal dari penulis 3 dimiliki oleh {Penulis 3}.
Himpunan pemilik soal berbeda adalah {Penulis 1, Perusahaan 42, Penulis 2, Penulis 3}, yang memiliki
tingkat keragaman 4.

## Batasan
Batasan waktu : 1s

Batasan memori : 64 MB

Batasan yang berlaku untuk versi mudah dan versi sulit:
- 1 ≤ T ≤ 10
- 1 ≤ C[i][j] ≤ 50
- Nilai-nilai dari C[i][1], C[i][2], . . . , C[i][P [i]] berbeda-beda.
Batasan khusus versi mudah:
- 1 ≤ N ≤ 10
- 1 ≤ S[i] ≤ 2
- 0 ≤ P [i] ≤ 2
Batasan khusus versi sulit:
- 1 ≤ N ≤ 50
- 1 ≤ S[i] ≤ 50
- 1 ≤ P [i] ≤ 50