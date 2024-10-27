### labpy02
# Nama : Lola Seftyliani
# Kelas: TI.24.A.4
# NIM  : 312410339
# Matkul : BAHASA PEMOGRAMAN

### LATIHAN 1
### Program Perhitungan Nilai Akhir Siswa
### Deskripsi

Program ini menerima input nilai UTS (Ujian Tengah Semester), UAS (Ujian Akhir Semester), dan nilai tugas dari pengguna, kemudian menghitung nilai akhir siswa berdasarkan bobot tertentu:

• 20% untuk nilai tugas
• 40% untuk nilai UTS
• 40% untuk nilai UAS

Program ini juga menampilkan nilai huruf berdasarkan nilai akhir, serta menentukan apakah siswa "LULUS" atau "TIDAK LULUS" berdasarkan kriteria nilai akhir.

### Cara Kerja Program

Input Pengguna:

Program meminta pengguna untuk memasukkan:
Nama siswa
Nilai UTS (Ujian Tengah Semester)
Nilai UAS (Ujian Akhir Semester)
Nilai Tugas
```python

ama = input("Masukkan nama:")
uts = input("Masukkan nilai UTS:")
uas = input("Masukkan nilai UAS:")
tugas = input("Masukkan nilai Tugas:")
Menghitung Nilai Akhir:
```
Nilai Akhir=(0.2×Tugas)+(0.4×UTS)+(0.4×UAS)
Hasil perhitungan disimpan dalam variabel akhir.

```python

akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
Menentukan Keterangan Lulus:
```
Program menentukan apakah siswa lulus atau tidak dengan membandingkan nilai akhir dengan 60. Jika nilai lebih dari 60, siswa dinyatakan "LULUS", sebaliknya "TIDAK LULUS".

```python

keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
Menentukan Nilai Huruf:
```
Nilai akhir kemudian diubah menjadi huruf berdasarkan kriteria berikut:
A: > 80
B: > 70
C: > 50
D: > 40
E: <= 40

```python

if akhir > 80:
    huruf = "A"
elif akhir > 70:
    huruf = "B"
elif akhir > 50:
    huruf = "C"
elif akhir > 40:
    huruf = "D"
else:
    huruf = "E"
```
Menampilkan Hasil:

Program menampilkan semua informasi hasil, termasuk nama siswa, nilai UTS, UAS, Tugas, nilai akhir, nilai huruf, dan keterangan kelulusan.
```python

print("\nNama :", nama)
print("Nilai UTS :", uts)
print("Nilai UAS :", uas)
print("Nilai Tugas :", tugas)
print("Nilai Akhir :", akhir)
print("\nNilai Huruf :", huruf)
print("Keterangan :", keterangan)
Contoh Penggunaan
Jika pengguna memasukkan:
```
Nama: "Lola"
Nilai UTS: 100
Nilai UAS: 95
Nilai Tugas: 98
Maka output program akan menunjukkan:

yaml

```
Nama : Lola
Nilai UTS : 100
Nilai UAS : 95
Nilai Tugas : 98
Nilai Akhir : 97.6
Nilai Huruf : A
Keterangan : LULUS
```

## Berikut hasil sceenshot visual code

![Screenshot 2024-10-27 142057](https://github.com/user-attachments/assets/14de41fb-b032-47c8-92a8-eaa70c9e624d)

Program ini memberikan cara yang sederhana untuk menghitung nilai akhir siswa dan menentukan kelulusan serta nilai huruf berdasarkan input yang diberikan. Hal ini memudahkan siswa untuk mengetahui hasil akademis mereka dengan cepat.

## Penjelasan

- Tugas UTS, dan UAS dimasukan oleh pengguna sebagai input dengan float.
- Nilai akhir dihitung menggunakan bobot tertentu (20% tugas, 40% UTS, 40% UAS).
- Berdasarkan nilai akhir, program menentukan nilai huruf dan keterangan kelulusan.

## Latihan 2

## Program Pengecekan gaji, status keluarga, dan kepemilikan Rumah

## Deskripsi

Program ini menerima input gaji, status keluarga (sudah berkeluarga atau belum), dan status kepemilikan rumah dari pengguna, kemudian melakukan beberapa pengecekan sebagai berikut:
1. Apakah gaji di atas UMR (Upah Minimum Regional).
2. Jika gaji di atas UMR, program akan mengecek apakah pengguna sudah berkeluarga untuk menentukan kewajiban mengikuti asuransi dan menabung.
3. Program juga mengecek apakah pengguna memiliki rumah untuk menentukan kewajiban membayar pajak rumah.

## Cara Kerja Program
1. Program meminta input dari pengguna untuk gaji, status berkeluarga, dan status kepemilikan rumah.
2. Jika gaji lebih dari 3.000.000, program akan mencetak "Gaji sudah di atas UMR". Jika tidak, akan mencetak "Gaji belum UMR".
3. Jika pengguna sudah berkeluarga, program akan mencetak "Wajib ikutan asuransi dan menabung untuk pensiun",namun jika belum berkeluarga, akan mencetak "Tidak perlu ikutan asuransi".
4. Jika pengguna memiliki rumah, program akan mencetak "Wajib bayar pajak rumah". Jika tidak memiliki rumah, akan mencetak "Tidak wajib bayar pajak rumah".

## Struktur Program 
- Input:
   - Gaji (int)
   - Status berkeluarga (Y/T)
   - Status kepemilikan rumah (Y/T)
- Output:

   - Apakah gaji sudah di atas UMR atau belum
   - Kewajiban mengikuti asuransi jika sudah berkeluarga
   - Kewajiban membayar pajak rumah jika punya rumah

## Contoh Penggunaan

## Gaji di atas UMR

```
Masukan gaji: 4000000000
Sudah Berkeluarga? (Y/T): Y
Punya Rumah? (Y/T): Y

Gaji Sudah diatas UMR
Wajib ikutan asuransi dan menabung untuk pesiun
Tidak wajib bayar pajak rumah

```

## Berikut hasil screenshot visual code

![Screenshot 2024-10-25 201521](https://github.com/user-attachments/assets/2b4e3d0f-7eea-4991-9749-6fcfded63382)

## Gaji dibawah UMR

```
Masukan gaji: 2500000
Sudah berkeluarga? (Y/T): Y
Punya rumah? (Y/T): Y

Gaji belum UMR
Tidak wajib bayar pajak rumah

```

## Berikut hasil screenshot visual studio code

![Screenshot 2024-10-25 202548](https://github.com/user-attachments/assets/df77fe5f-79aa-47d5-9174-f300562c66b0)

## Penjelasan

- Pengecekan berkaluarga dan punya rumah: Variabel berkeluarga den punya rumah dicek dengan perbandingan input terhadap "Y menggunakan input ().strip().upper() == "Y" , yang memastikan bahwa input diubah menjadi huruf kapital dan mengabellan spesi yang tidak perlu.
- Program ini menggunakan if-else untuk menentukan pesan yang akan ditampilkan berdasarkan kondisi gaji, status keluarga, dan status kepemilikan rumah.

## Latihan 3

## Menggunakan kondisi OR dengan menginputkan 3 bilangan

```
a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))
if a+b == c or b+c == a or c+a == b:
   print("BENAR")
else:
   print("SALAH")
```
operator OR dalam python merubah beberapa kondisi dan mengembalikan true jika salah satu bena

```
a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))
```
Program ini menginputkan sesuatu integer yang menggunakan variable a,b,c.

```
if a+b == c or b+c == a or c+a == b:
   print("BENAR")
else:
   print("SALAH")
```
jika (A) ditambah (B) haslnya (C) atau bahasa pemograman itu OR ,dan apabila (B) ditambah (C) hasilnya (A),dan (C) ditambah (A) maka hasilnya (B). maka output yang keluar adalah "benar"







