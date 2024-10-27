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

nama = input("Masukkan nama:")
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

``` python
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

``` python 
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

```python
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

```pyhton
a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))
if a+b == c or b+c == a or c+a == b:
   print("BENAR")
else:
   print("SALAH")
````
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

## Latihan 3

## Pemesanan Tiket Bioskop

Kasus 1: Program Pemesanan Tiket Bioskop
Buat program yang menghitung harga tiket bioskop. Tiket reguler berharga Rp50.000,
sedangkan tiket VIP berharga Rp100.000. Jika user memiliki kartu member, mereka
mendapatkan diskon 20% dari harga tiket. Program ini harus meminta tipe tiket dan status
member dari user, lalu menghitung total harga yang harus dibayar.

Petunjuk:

- Gunakan if else dan operator ternary.

```python
harga_reguler = 50000
harga_vip = 100000

tipe_tiket = (input("Masukkan tipe tiket (reguler/VIP): "))
status_member = (input("Apakah Anda memiliki kartu member? (ya/tidak): "))

#Menghitung total harga
if tipe_tiket == "reguler":
    total_harga = harga_reguler
elif tipe_tiket == "vip":
    total_harga = harga_vip
else:
    print("Tipe tiket tidak valid.")
    exit()

#Menghitung diskon jika pengguna memiliki kartu member

if status_member == "ya":
        total_harga *= 0.8  # Diskon 20%
    
        print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")
elif status_member == "tidak":
            total_harga
            print(f"total harga yang harua dibayar: Rp{total_harga:.2f}")
else:
    print("Harga tidak dapat dihitung.")
````

Program ini akan menentukan harga pesanan tiket bioskop, Yang reguler/Vip, dan jika Vip harga 100.000, dan jika reguler 80.0000, dan jika memiliki kartu member pelanggan tersebut akan mendapatkan diskon 20%

```python
harga_reguler = 50000
harga_vip = 100000
````
variable ini menentukan harga tiket bioskop

```pyhton
tipe_tiket = (input("Masukkan tipe tiket (reguler/VIP): "))
status_member = (input("Apakah Anda memiliki kartu member? (ya/tidak): "))
````

memasukan inputan sesuai Output Program (Reguler/Vip) di variable (Tipe_Tiket), dan Memasukan inputan yang output tersebut Bertanya memiliki kartu member atau tidak.

```pyhton
if tipe_tiket == "reguler":
    total_harga = harga_reguler
elif tipe_tiket == "vip":
    total_harga = harga_vip
else:
    print("Tipe tiket tidak valid.")
    exit()
````
Jika tipe tiket reguler total harga proses ke Harga reguler, dan jika tiket vip Total harga proses keharga vip

dan jika Selain memasukan inputan reguler/vip Output yang keluar "Tipe tiket tidak valid" dan berproses ke fungsi exit() yang artinya program dihentikan.

```pyhton
if status_member == "ya":
        total_harga *= 0.8  # Diskon 20%
        print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")
elif status_member == "tidak":
            total_harga
            print(f"total harga yang harua dibayar: Rp{total_harga:.2f}")
else:
    print("Harga tidak dapat dihitung.")
```

desision ini menentukan mempunyai kartu member atau tidak, Jika Inputan status member menjawab "ya", maka total harga akan di kalikan dengan operator * 0,8 yang disebut diskon 20%

dan jika inputan status member "tidak", maka total harga normal

jika menginputkan selain (ya/tidak) output yang keluar "Harga tidak dapat dihitung"

Dan ini hasil program tersebut:

## Hasil program pemesenan tiket bioskop

![Screenshot 2024-10-27 151748](https://github.com/user-attachments/assets/e50115c0-02df-46d0-ab3e-debd25bdcec6)

## dan Flowchartnya:

![WhatsApp Image 2024-10-27 at 15 27 16_015035b5](https://github.com/user-attachments/assets/ce15dee4-7e7d-4149-9b30-c4837e592036)

## Kalkulator Sederhana

### Kasus 2: Program Kalkulator Sederhana

Buat program kalkulator yang menerima dua angka dan satu operator aritmatika dari pengguna (penjumlahan, pengurangan, perkalian, atau pembagian). Program akan menghitung hasil sesuai dengan operator yang dipilih.

## Petunjuk

```PYHTON

 Gunakan if elif else untuk menentukan operasi aritmatika.
angka1 = float(input("Masukkan angka pertama: "))

````

operator = input("Masukkan operator (+, -, *, /): ") angka2 = float(input("Masukkan angka kedua: "))

## Menghitung Hasil berdasarkan operator

```pyhton

if operator == '+':
    hasil = angka1 + angka2
    print(f"Hasil penjumlahan: {hasil}")
elif operator == '-':
    hasil = angka1 - angka2
    print(f"Hasil pengurangan: {hasil}")
elif operator == '*':
    hasil = angka1 * angka2
    print(f"Hasil perkalian: {hasil}")
elif operator == '/':
    if angka2 != 0:
        hasil = angka1 / angka2
        print(f"Hasil pembagian: {hasil}")
    else:
        print("Error: Pembagian dengan nol tidak diperbolehkan.")

else:
    print("Error: Operator tidak valid. Silakan gunakan +, -, *, atau /.")

````

Program kalkulator sederhana dalam Python adalah proyek yang baik untuk pemula dan programmer tingkat lanjut. Program ini memungkinkan pengguna untuk melakukan operasi matematika seperti penjumlahan, pengurangan, perkalian, dan pembagian.

```pyhton

angka1 = float(input("Masukkan angka pertama: "))
operator = input("Masukkan operator (+, -, *, /): ")
angka2 = float(input("Masukkan angka kedua: "))

````

ungsi yang digunakan dalam inputan ini menggunakan float mengubah nilai menjadi angka floating point, yaitu angka desimal atau pecahan, dan variable operator yang menginputkan suatu operator fungsi berupa (+, -, *, /) yang artinya pertambahan, perkurang, perkali, pembagian.

```pyhton

if operator == '+':
    hasil = angka1 + angka2
    print(f"Hasil penjumlahan: {hasil}")

````


Jika operator (+), maka hasil tersbur inputan variable angka1 ditambahkan angka2, dan Output akan mengeluarkan hasil program tersebut, Hingga seterusnya dengan (*) perkalian, dan (-) perkurangan

```pyhton

elif operator == '/':
    if angka2 != 0:
        hasil = angka1 / angka2
        print(f"Hasil pembagian: {hasil}")
    else:
        print("Error: Pembagian dengan nol tidak diperbolehkan.")

````

Jika oprator (/), maka Inputan Variable angka1 dibagi angka2, dan dicetak semestinya, untuk desision (angka2 !=0:) tidak diperkenankan oleh program, karna output yang keluar "Error: Pembagian dengan nol tidak diperbolehkan"

```pyhton
else:
    print("Error: Operator tidak valid. Silakan gunakan +, -, *, atau /.")

````

saya memasukan desision else ini Karna jika menjawab selain fungsi operator ini Output yang keluar "Error: Operator tidak valid. Silakan gunakan +, -, *, atau /."

dan ini hasil program tersebut:

## Hasil dari program kalkulator di visual studio code

![Screenshot 2024-10-27 184715](https://github.com/user-attachments/assets/eafc52a5-a157-4cae-8282-29f286c757af)

## Dan flowchartnya
![Screenshot 2024-10-27 153830](https://github.com/user-attachments/assets/3d99b859-6ac9-4b99-b360-b53c130d5248)

















