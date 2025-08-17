# LAB-17-ARP-dan-Static-ARP
tanggal 16 Agustus 

**Interface ARP Mode**

• Enable: ode ini default enable pada semua interface di MikroTik.    
  Semua ARP akan ditemukan dan secara dinamik ditambahkan dalam    
  ARP tabel.   
• Proxy ARP: Router dengan mode ARP proxy akan bertindak sebagai   
  transparan proxy ARP antara dia atau lebih jaringan yang terhubung   
  langsung.   
• Reply Only: ARP reply-only memungkinkan router hanya kan mereply   
  ARP statis ditemukan di tabel ARP, akses ke router dan ke jaringan di 
  belakang router hanya dapat diakses oleh kombinasi Ip dan mac      
  address yang ditemukan di tabel ARP.     
• Disable: permintaan ARP dari klien tidak dijawab oleh router. Oleh    
  karena itu, statis arp entri harus ditambahkan disamping disisi router   
  juga disisi client. misal pada Windows menggunakan perintah arp:     
  C: \> arp-s 192.168.2.1 00-aa-00-62-c6-09. 
  
# Konfigurasi ARP dan static ARP
**ARP (Address Resolution Protocol)**.  
**Enable**.   

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

![m](IMG_20250816_110026.jpg)

- Terakhir, klik Make Static.
  bisa di lihat semua clien sudah dapat mac address
  
![m]()

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
https://drive.google.com/file/d/1IUjPTXdBi0mH_CvpcCXSo3-hv3pX4_og/view?usp=drivesdk
