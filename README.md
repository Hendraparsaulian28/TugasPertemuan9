## NAMA : Hendra Parsaulian
## NIM : 312210689
## KELAS : TI.22.A.3

Jika sudah kita bisa memasukan kode inputan dengan benar agar tidak terjadi eror

```py
data = []
stop = False

while(not stop):
    nama = input("Nama : ")
    nim = input("NIM : ")
    tugas = int(input("Nilai Tugas : "))
    uts = int(input("Nilai UTS : "))
    uas = int(input("Nilai UAS : "))
    akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35/100)
    data.append([nama,nim,tugas,uts,uas,int(akhir)])

    tanya = input('Tambahkan Data (y/t) ? ')
    if (tanya == 't'):
        stop = True

print("==================================================================")
print("| No |    Nama      |  NIM  | Tugas |  UTS  |  UAS  |  Akhir |")
print("==================================================================")

i = 0

for nilai in data:
    i += 1
    print("| {no}  | {nama:12s} | {nim:5s} | {tugas:5d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |".format(no=i, nama=nilai[0], nim=nilai[1], tugas=nilai[2],uts=nilai[3],uas=nilai[4],akhir=nilai[5]))

print("==================================================================")
```


Jika kode yang dimasukan sudah sesuai maka hasil output dari kode tersebut adalah

![ss](https://user-images.githubusercontent.com/116443572/203241974-5fbbb41d-1089-4174-8124-1ac2c9226489.png)
