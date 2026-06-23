# Penjelasan Program

Program ini menggunakan perulangan **do-while** untuk menampilkan menu secara berulang hingga pengguna memilih opsi **2 (Keluar)**.

## Alur Program

1. Program mendeklarasikan variabel `pilihan` bertipe `int`.
2. Blok `do` dijalankan terlebih dahulu dan menampilkan menu:

   ```
   1. Main
   2. Keluar
   ```
3. Program meminta pengguna memasukkan pilihan melalui `cin`.
4. Setelah input diterima, kondisi pada `while (pilihan != 2)` diperiksa:

   * Jika nilai `pilihan` **bukan 2**, menu akan ditampilkan kembali.
   * Jika nilai `pilihan` **sama dengan 2**, perulangan berhenti dan program selesai.

## Struktur Perulangan

```cpp
do {
    // kode yang dijalankan
} while (kondisi);
```

Pada program ini:

```cpp
while (pilihan != 2);
```

Artinya perulangan akan terus berjalan selama pengguna tidak memilih angka `2`.

## Contoh Output

```
1.Main
2.Keluar
pilih: 1

1.Main
2.Keluar
pilih: 1

1.Main
2.Keluar
pilih: 2
```

Ketika pengguna memasukkan `2`, program akan keluar dari perulangan dan berakhir.

## Konsep yang Digunakan

* `#include <iostream>` : untuk operasi input dan output.
* `using namespace std;` : agar dapat menggunakan `cout` dan `cin` tanpa menuliskan `std::`.
* `do-while` : perulangan yang dijalankan minimal satu kali sebelum kondisi diperiksa.
* `cin` : menerima input dari pengguna.
* `cout` : menampilkan output ke layar.



