## Nama : Rini Ariza
## NIM : 312210337
## Kelas : TI.22.A3
## PERTEMUAN 10 (TUGAS PRATIKUM)

### Soal

![soal pet10](https://user-images.githubusercontent.com/115542704/203807634-a7766dd8-9bf7-43ba-9684-c24d86585780.png)


# flowchart

![img](gambar/flowchart.png)

# jawab
pertama saya membuat looping agar program terus berjalan

    while True:
    c = input("\n(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar: ")
    if (c.lower() == 't'):
        print('\nTambah Data Mahasiswa Baru')
        nama= input("Masukkan Nama\t\t: ")
        nim= input("Masukkan NIM\t\t: ")
        nilaiTugas= int(input("Masukkan Nilai Tugas\t: "))
        nilaiUts= int(input("Masukkan Nilai UTS\t: "))
        nilaiUas= int(input("Masukkan Nilai UAS\t: "))
        nilaiAkhir= (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)
        dataMhs[nama]= nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir
        print("\nData Berhasil Ditambahkan!")
    elif (c.lower() == 'u'):
        print('\nMengedit Data Mahasiswa')
        nama = input("Masukkan Nama: ")
        if nama in dataMhs.keys():
            nim= input("Masukkan NIM Baru\t: ")
            nilaiTugas= int(input("Masukkan Nilai Tugas\t: "))
            nilaiUts= int(input("Masukkan Nilai UTS\t: "))
            nilaiUas= int(input("Masukkan Nilai UAS\t: "))
            nilaiAkhir= (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)
            dataMhs[nama] = nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir
            print("\nData Berhasil Di Update!")
        else:
            print("Data tidak ditemukan!")
    elif (c.lower() == 'c'):
        print('\nCari Data Mahasiswa')
        nama = input("Masukan Nama:  ")
        if nama in dataMhs.keys():
            print("\n                   DAFTAR NILAI MAHASISWA                   ")
            print("==============================================================")
            print("|     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
            print("==============================================================")
            print("| {0:12s} | {1:9s} | {2:5} | {3:5} | {4:5} | {5:6} |".format(nama, nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir))
            print("==============================================================")
        else:
            print("Datanya {0} Tidak Ada ".format(nama))
    elif (c.lower() == 'h'):
        nama = input("Masukkan Nama:  ")
        if nama in dataMhs.keys():
            del dataMhs[nama]
            print("Data Telah dihapus!")
        else:
            print("Data Mahasiswa Tidak Ada".format(nama))
    elif (c.lower() == 'l'):
        if dataMhs.items():
            print("\n                      DAFTAR NILAI MAHASISWA                    ")
            print("==================================================================")
            print("| No |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
            print("==================================================================")
            i = 0
            for x in dataMhs.items():
                i += 1
                print("| {6:2} | {0:12s} | {1:9s} | {2:5} | {3:5} | {4:5} | {5:6} |".format(x[0], x[1][0], x[1][1], x[1][2], x[1][3], x[1][4], i))
            print("==================================================================")
        else:
            print("\n                      DAFTAR NILAI MAHASISWA                    ")
            print("==================================================================")
            print("| No |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
            print("==================================================================")
            print("|                          TIDAK ADA DATA!                       |")
            print("==================================================================")
    elif (c.lower() == 'k'):
        print('\n')
        print(21*'=')
        print("Nama\t: Rini ariza\nKelas\t: TI.22.A3\nNIM\t: 312110337")
        print(21*'=')
        break

    else:
        print("Pilih menu yang tersedia: ")


# output 
ini adalah output apabila memilih tambah(t)
 
<img width="369" alt="screenshot 1" src="https://user-images.githubusercontent.com/115542704/203813454-b50123af-5d56-4807-a8e8-83196f064439.png">

ini adalah output apabilah memilih  diubah(u)

<img width="356" alt="screenshot 2" src="https://user-images.githubusercontent.com/115542704/203813676-7bcb5b81-970d-44d0-a245-05a8338ea037.png">


ini adalah apabilah mencari output (c)

<img width="392" alt="screenshot 3" src="https://user-images.githubusercontent.com/115542704/203813876-9eaac216-87e4-4f60-9c28-1fe2be7dabc0.png">

ini adalah output apabila memilih hapus(h) 

![img](gambar/outputH.png)

ini adalah output apabila memilih lihat (l)

![img](gambar/outputL.png)

ini adalah output apabila memilih keluar (k)

<img width="356" alt="screenshot 4" src="https://user-images.githubusercontent.com/115542704/203813921-7cc966e3-85a1-4170-b0b6-316094b0018d.png">




