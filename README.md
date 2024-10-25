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
Copy code
ama = input("Masukkan nama:")
uts = input("Masukkan nilai UTS:")
uas = input("Masukkan nilai UAS:")
tugas = input("Masukkan nilai Tugas:")
Menghitung Nilai Akhir:
```
Nilai Akhir=(0.2×Tugas)+(0.4×UTS)+(0.4×UAS)
Hasil perhitungan disimpan dalam variabel akhir.

```python
Copy code
akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
Menentukan Keterangan Lulus:
```
Program menentukan apakah siswa lulus atau tidak dengan membandingkan nilai akhir dengan 60. Jika nilai lebih dari 60, siswa dinyatakan "LULUS", sebaliknya "TIDAK LULUS".

```python
Copy code
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
Copy code
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
Copy code
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
Nama: "Ali"
Nilai UTS: 80
Nilai UAS: 70
Nilai Tugas: 60
Maka output program akan menunjukkan:

yaml
Copy code
```
Nama : Ali
Nilai UTS : 80
Nilai UAS : 70
Nilai Tugas : 60
Nilai Akhir : 70.0
Nilai Huruf : B
Keterangan : LULUS
```
Kesimpulan
Program ini memberikan cara yang sederhana untuk menghitung nilai akhir siswa dan menentukan kelulusan serta nilai huruf berdasarkan input yang diberikan. Hal ini memudahkan siswa untuk mengetahui hasil akademis mereka dengan cepat.
