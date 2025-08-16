# LAB-17-ARP-dan-Static-ARP
tanggal 16 Agustus 

# Konfigurasi ARP dan static ARP
**ARP (Address Resolution Protocol**

Langkah 1: Aktifkan ARP di Interface List  

Klik menu Interfaces.  
Klik satu persatu interface yang aktif   
pilih enabled pada kolom isian ARP.  

![m]()

Langkah 2 : Cara Setting Manual ARP List MikroTik. 

Ada dua cara setting manual ARP List Mikrotik.   
1. Klik menu IP > ARP.  
   klik tanda “+” untuk menambahkan secara manual.  
   Isikan IP Address, Mac Address dan Interface. 
   kemudian klik OK.  

![m]()

![m]()

2. Jika punya banyak klien, akan repot jika meng input data satu satu.  
   maka dari itu kita gunakan cara cepat dan mudah.  
   
- Buka jendela ARP List dengan cara diatas tadi.  
- Nyalakan semua klien untuk mendeteksi IP Address, Mac Address dan Interfacenya.    
- lalu tekan Ctrl + A di keyboard.  
- Klik kanan pada salah satu data klien.

![m]()

- Terakhir, klik Make Static.    

Setelah mengaktifkan ARP List MikroTik dengan cara diatas,    
hanya IP Address dan Mac Address yang sudah kita daftarkan,    
yang akan direspon oleh router. Dengan begitu,  
jika ada klien yang mengganti IP Address dan datanya tidak cocok. 
dengan data yang ada di ARP List MikroTik,   
tidak akan mendapat respon dari router atau tidak akan terkoneksi ke internet.  

# kesimpulan   
ARP adalah protokol yang digunakan untuk menerjemahkan   
alamat IP menjadi alamat MAC pada jaringan lokal.  
sedangkan Static ARP adalah entri ARP yang ditambahkan   
secara manual dan tidak berubah-ubah.  
# sumber. 
https://mikrotikgame.blogspot.com/2017/08/cara-setting-arp-list-mikrotik.html?m=1
