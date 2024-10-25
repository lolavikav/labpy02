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

Jika ada yang ingin ditambahkan atau disesuaikan dalam penjelasan, silakan beri tahu!



You said:
saya pengen unduh file nya
ChatGPT said:
ChatGPT
Saat ini, saya tidak dapat membuat file untuk diunduh secara langsung. Namun, saya bisa memberi tahu cara membuat file README menggunakan teks yang telah saya berikan.

Cara Membuat File README
Buka Editor Teks:

Anda bisa menggunakan editor teks seperti Notepad, VS Code, atau editor lain yang Anda sukai.
Salin Teks:

Salin teks README yang saya berikan sebelumnya.
Tempel ke Editor:

Tempelkan teks yang telah disalin ke dalam editor.
Simpan File:

Simpan file dengan nama README.md (pastikan untuk memilih "All Files" jika menggunakan Notepad agar ekstensi .md tidak diubah menjadi .txt).
Selesai:

Sekarang Anda memiliki file README yang siap digunakan!
Jika ada langkah yang tidak jelas atau Anda memerlukan bantuan lebih lanjut, silakan beri tahu!



You said:
mana file nya
ChatGPT said:
ChatGPT
Saya tidak dapat membuat atau mengirim file langsung kepada Anda. Namun, Anda dapat dengan mudah membuat file README sendiri dengan mengikuti langkah-langkah yang saya sebutkan sebelumnya.

Teks untuk README
Berikut adalah teks yang bisa Anda salin:

markdown
Copy code
# Penjelasan Program Penilaian Siswa

## Deskripsi
Program ini meminta input dari pengguna mengenai nama dan nilai akademis (UTS, UAS, dan Tugas) untuk menghitung nilai akhir dan menentukan keterangan kelulusan serta nilai huruf. Nilai akhir dihitung berdasarkan bobot tertentu untuk masing-masing komponen.

## Cara Kerja Program

1. **Input Pengguna**:
   - Program meminta pengguna untuk memasukkan:
     - Nama siswa
     - Nilai UTS (Ujian Tengah Semester)
     - Nilai UAS (Ujian Akhir Semester)
     - Nilai Tugas

   ```python
   nama = input("Masukkan nama:")
   uts = input("Masukkan nilai UTS:")
   uas = input("Masukkan nilai UAS:")
   tugas = input("Masukkan nilai Tugas:")
Menghitung Nilai Akhir:

Nilai akhir dihitung dengan menggunakan rumus:
```
Nilai Akhir=(0.2×Tugas)+(0.4×UTS)+(0.4×UAS)
Nilai Akhir=(0.2×Tugas)+(0.4×UTS)+(0.4×UAS)
Hasil perhitungan disimpan dalam variabel akhir.
```
```python
Copy code
akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
Menentukan Keterangan Lulus:
```
Program menentukan apakah siswa lulus atau tidak dengan membandingkan nilai akhir dengan 60. Jika nilai lebih dari 60, siswa dinyatakan "LULUS", sebaliknya "TIDAK LULUS".
python
Copy code
keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
Menentukan Nilai Huruf:

Nilai akhir kemudian diubah menjadi huruf berdasarkan kriteria berikut:
A: > 80
B: > 70
C: > 50
D: > 40
E: <= 40
python
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
Menampilkan Hasil:

Program menampilkan semua informasi hasil, termasuk nama siswa, nilai UTS, UAS, Tugas, nilai akhir, nilai huruf, dan keterangan kelulusan.
python
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

Nama: "Ali"
Nilai UTS: 80
Nilai UAS: 70
Nilai Tugas: 60
Maka output program akan menunjukkan:

yaml
Copy code
Nama : Ali
Nilai UTS : 80
Nilai UAS : 70
Nilai Tugas : 60
Nilai Akhir : 70.0
Nilai Huruf : B
Keterangan : LULUS
Kesimpulan
Program ini memberikan cara yang sederhana untuk menghitung nilai akhir siswa dan menentukan kelulusan serta nilai huruf berdasarkan input yang diberikan. Hal ini memudahkan siswa untuk mengetahui hasil akademis mereka dengan cepat.
