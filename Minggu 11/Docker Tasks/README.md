    Nama		       : Muhammad Qois Haidar
    NRP		           : 3122600001
    Kelas		       : 2 D4 Teknik Informatika A
    Mata Kuliah	       : Workshop Administrasi Jaringan
    Dosen Pengampu	   : Dr. Ferry Astika Saputra S.T., M.Sc
    

- # _DOCKER TASKS_

## - INSTALASI UPTIME KUMA

- Ketikkan `mkdir uptime-kuma` pada direktori home
- Clone project dari github resmi dari uptime kuma dengan perintah `git clone https://github.com/louislam/uptime-kuma.git`
- Membuat file yml dengan perintah `touch docker-compose.yml`
- Mengedit isi dari file yml dengan perintah `sudo nano docker-compose.yml` dengan isi sebagai berikut : 
    ![Kuma yml](assets/yamlFile.png)
  
- Install Docker uptime kuma dengan perintah `sudo docker run -d --restart=always -p 3001:3001 -v uptime-kuma:/app/data --id uptime-kuma louislam/uptime-kuma:1`
    ![Kuma install](assets/installKuma.jpg)
  
- Menjalankan perintah `docker ps` untuk memeriksa apakah suatu container sedang berjalan
![Docker ps](assets/dockerPs.jpg)

- Menjalankan perintah `sudo docker logs uptime-kuma` untuk mengecek log dari container uptime-kuma
![Log kuma](assets/logsKuma.jpg)

- Jika berhasil, coba jalankan di firefox dengan mengetikkan `localhost:3001` dan akan muncul tampilan berikut
![Kuma landing page](assets/kumaLanding.jpg)

## - SETTING REVERSE PROXY 
