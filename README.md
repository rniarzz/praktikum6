# Nama : Rini Ariza
# NIM : 312210337
# Kelas : TI.22.A3
# PERTEMUAN 10 (TUGAS PRATIKUM)
pada tugas praktium saya diberi soal sebagai berikut




# flowchart

![img](gambar/flowchart.png)

# jawab
pertama saya membuat looping agar program terus berjalan

    while True:
        c = input("\n(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar: ")                                

    lalu saya membuat format if untuk memasukan pilihan , sebagai contoh apabila memilih (t) akan menambah data

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

    saya juga melakukan percabangan if (elif) untuk melaksanakan pilihan yang lain

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

    dan saya juga menggunakan else untuk apabila salah memasukan pilihan inputan

        else:
        print("Pilih menu yang tersedia: ")  

 # tampilan pada visual studio code  

 ![img](gambar/vscode2.png) 


# output 
ini adalah output apabila memilih tambah(t)
 
![img](gambar/t.png)


 ini adalah output apabilah memilih  diubah

![img](gambar/U.png)

ini adalah apabilah mencari output (c)

![img](gambar/C.png)

ini adalah output apabila memilih untuk tambah lagi

![img](gambar/output/tll.png)

ini adalah output apabila memilih hapus(h) 

![img](gambar/outputH.png)

ini adalah output apabila memilih lihat (l)

![img](gambar/outputL.png)

ini adalah output apabila memilih keluar (k)

![img](gambar/outputk.png)





