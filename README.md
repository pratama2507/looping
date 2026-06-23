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



# Penjelasan Program

Program ini menggunakan perulangan **while** untuk meminta pengguna memasukkan angka secara berulang hingga pengguna memasukkan angka **0**.

## Alur Program

1. Program mendeklarasikan variabel `angka` dan menginisialisasinya dengan nilai `-1`.
2. Kondisi pada perulangan `while` diperiksa:

   ```cpp
   while (angka != 0)
   ```
3. Selama nilai `angka` tidak sama dengan `0`, program akan:

   * Menampilkan pesan:

     ```
     Masukkan angka (0 untuk berhenti):
     ```
   * Menerima input dari pengguna menggunakan `cin`.
4. Setelah pengguna memasukkan nilai:

   * Jika nilai yang dimasukkan **bukan 0**, perulangan akan terus berjalan.
   * Jika nilai yang dimasukkan **0**, kondisi `while` menjadi salah (`false`) dan program berhenti.

## Cara Kerja Perulangan

```cpp
int angka = -1;

while (angka != 0) {
    cout << "Masukkan angka (0 untuk berhenti): ";
    cin >> angka;
}
```

Nilai awal `angka` diatur menjadi `-1` agar kondisi `angka != 0` bernilai benar saat pertama kali diperiksa, sehingga perulangan dapat dimulai.

## Contoh Output

```text
Masukkan angka (0 untuk berhenti): 5
Masukkan angka (0 untuk berhenti): 10
Masukkan angka (0 untuk berhenti): 3
Masukkan angka (0 untuk berhenti): 0
```

Setelah pengguna memasukkan `0`, program akan berhenti.

## Konsep yang Digunakan

* `#include <iostream>` : digunakan untuk operasi input dan output.
* `using namespace std;` : agar dapat menggunakan `cout` dan `cin` tanpa menuliskan `std::`.
* `while` : perulangan yang akan terus berjalan selama kondisi bernilai `true`.
* `cin` : menerima input dari pengguna.
* `cout` : menampilkan output ke layar.
* **Kondisi penghentian (sentinel value)** : angka `0` digunakan sebagai tanda untuk mengakhiri perulangan.



