# Uas

# Membuat Program Menggunakan Init

program menggunakan init ialah program yang berisi daftar lis

contoh:

list = [item]

list = [item2]

data = {'nama' : [], 'nilai' : []}

lalu kita membuat program method yg berisi modul daftar_nilai

dan modul view_nilai

kita bisa mengimportkan modul yang berisi daftar nilai seperti ini

from model import daftar_nilai

lalu kita importkan lagi view nilai

from view import view_nilai

kita membuat program sistem perulangan dengan menggunakan.

while True:

lalu kita membuat keys.

print("[ (l)ihat , (t)ambah, (c)ari (u)bah, (h)apus, (k)eluar ] \n")

contoh program:



from model import daftar_nilai

from view import view_nilai

data = {'nama' : [], 'nilai' : []}

while True:

    print("[ (l)ihat , (t)ambah, (c)ari (u)bah, (h)apus, (k)eluar ] \n")
    
    tanya = input("Masukkan Pilihan : ")
    
    match tanya:
    
        case "l":
        
            view_nilai.cetak_daftar_nilai(data)
            
        case "t":
        
            data = daftar_nilai.tambah_data(data)
            
        case "u":
        
            view_nilai.cetak_daftar_nilai(data)
            
            if len(data['nama']) > 0:
            
                nama = input("masukkan nama siswa yang akan diubah : ")
                
                data = daftar_nilai.ubah_data(data, nama)
                
        case "c":
        
            # view_nilai.cetak_daftar_nilai(data)
            
            
            if len(data['nama']) > 0:
            
                nama = input("masukkan nama siswa yang akan dicari : ")
                
                daftar_nilai.cari_data(data, nama)
                
        case "h":
        
            view_nilai.cetak_daftar_nilai(data)
            
            if len(data['nama']) > 0:
            
                nama = input("masukkan nama siswa yang akan dihapus : ")
                
                data = daftar_nilai.hapus_data(data, nama)
                
        case "k":
        
            print("anda sudah Keluar dari program")
            
            break
            
        case _:
        
            print("Tidak Sesuai Pilihan, Silahkan Pilih Kembali!!\n")
            
            continue
    

            
![Screenshot (92)](https://user-images.githubusercontent.com/115480539/210784305-000bb229-4239-463f-95b7-6d215babcece.png)

            
            
           
            
            
            
            

setelah kita membuat keys ya lalu kita inputkan daftar nilai kedalem modul yg kita buat
        
modul daftar_nilai yang telah kita buat lalu kita masukkan fungsi itu kedalamnya

oke tapi sebelum itu kita membuat view_nilai seperti modul yg perna kita buat

yang pertama kita harus menginstall pip tabulate seperti ini

![image](https://user-images.githubusercontent.com/115480539/210779457-39ee8592-4f01-4acf-ad02-307da15b5f5c.png)

setelah pip tabulate terinstall kita membuat modul

yang berisi

from tabulate import tabulate

lalu kita eksekusikan dengan code tersebut

![image](https://user-images.githubusercontent.com/115480539/210780671-a144aebf-f4d8-4757-b058-4bdfdb18a366.png)

Dan setelah semuanya jadi, tinggal kita lihat hasil dari program nya

![image](https://user-images.githubusercontent.com/115480539/210786084-796b2f1c-6178-4842-9d88-675aa5e6340c.png)

Sekian dari saya Trimakasih

https://drive.google.com/drive/folders/1pgYUFXKuaXgYTxSA7lCcT3SdNzkMZdiO?usp=sharing

https://youtu.be/Yjl9P-UnDoI








            
            
