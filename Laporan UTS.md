## **LAPORAN PRAKTIKUM UJIAN TENGAH SEMESTER**

1. **Instalasi Windows Server 2022**

   - Download terlebih dahulu ISO Windows Server 2022.

     ```markdown
     https://software-download.microsoft.com/download/sg/20348.169.210806-2348.fe_release_svc_refresh_SERVER_EVAL_x64FRE_en-us.iso
     ```

   - Buat file baru sebelum melakukan instalasi. Typer yang digunakan ialah Microsoft Windows dengan version Other Wishdows (64-bit), kemudian klik Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\1.PNG)

   - Isi RAM untuk virtual machine sesuai kebutuhan. Di sini menggunakan 2048 mb.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2.PNG)

   - Lakukan create virtual machine, pilih Create a virtual harddisk now.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\3.PNG)

   - Pilih VDI (VirtualBox Disk Image), kemudian Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\4.PNG)

   - Pilih Dynamically allocated.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\5.PNG)

   - Langkah selanjutnya yaitu mengisi besaran memori untuk VM sesuai keinginan. Rekomendasi ukuran yang digunakan adalah 20 GB, tetapi di sini menggunakan 40 GB. Setelah itu klik Create.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\6.PNG)

   - Jika file telah berhasil dibuat, maka selanjutnya klik Start untuk memulai instalasi. Masukkan file ISO terlebih dahulu, agar instalasi dapat berjalan. Jika sudah, maka klik Start.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\7.PNG)

   - Tampilan berikutnya akan terlihat seperti ini.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\8.PNG)

   - Pilih pengaturan bahasa yang digunakan, lalu klik Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\rev 1.PNG)

   - Selanjutnya, pilih Install now.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\10.PNG)

   - Pada langkah ini, pilih menu kedua atau Windows Server 2022 Standard Evaluation (Dekstop Experience) jika ingin menginstal versi GUI.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\rev 2.PNG)

   - Cetang atau setujui lisensi yang ada, lalu klik Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\12.PNG)

   - Pilih custom.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\13.PNG)

   - Next untuk menetapkan ukuran memori yang digunakan.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\14.PNG)

   - Tunggu hingga proses selesai

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\rev 3.PNG)

   - Setelah proses selesai, akan muncul tampilan untuk mengisi password yang akan digunakan untuk melakukan login.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\rev 4 isi passwd.PNG)

   - Berikut ini adalah tampilan awal sebelum login. Klik menu Input pada VirtualBox, pilih Keyboard, lalu klik pilihan Ctrl+Alt+Del, untuk melakukan unlock.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\rev 5 done.PNG)

   - Masukkan password yang telah disetting sebelumnya sebagai proses verifikasi.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\rev 6.PNG)

   - Jika berhasil, maka akan masuk ke halaman utama. Proses instalasi telah selesai.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\rev 7.PNG)

   

2. **Instalasi Active Directory Domain Services**

   - Langkah awal yaitu install VBoxWindows Additions.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\1.png)

   - Klik Next hingga tida di halaman instalasi dan klik Install. Jika sudah selesai, pilih Finish.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\6.PNG)

   - Setelah itu, run Winver untuk memvalidasi installed edition dari Windows Server.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\7.PNG)

   - Ubah terlebih dahulu nama computer melalui windows powrshell.

     ```markdown
     rename-computer -Newname Server2022
     ```

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\8.PNG)

   - Masuk ke Server Manager, klik Add roles and fatures, kemudian pilih Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\9.PNG)

   - Pilih Role-based or feature based installation untuk melanjutkan.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\10.PNG)

   - Pilih Select a server from the server pool, kemudian klik Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\11.PNG)

   - Pada menu Server Roles, klik pilihan Active Directory Domain Services, lalu akan muncul pop-up dan pilih Add Features kemudian Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\12.PNG)

   - Centang atau pilih Group Policy Management.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\13.PNG)

   - Next pada menu AD DS.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\14.PNG)

   - Pada menu Confirmation, klik Install dan tunggu hingga proses instalasi selesai. Jika sudah selesai, pilih Close sehingga bisa melanjutkan ke proses berikutnya.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\15.PNG)

3. **Instalasi DNS Server**

   - Langkah pertama, masuk ke Server Manager, dan pilih Add Roles and Features. Klik Next seperti langkah instalasi Active Directory Domain Services sebelumnya. Pada menu Server Roles, pilih DNS Server, kemudian Add Features.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\17.PNG)

4. **Instalasi Net Framework 3.5**

   - Berikutnya, pada menu Features, pilih atau centang .Net Framework 3.5 Features, untuk menginstal Net Framework 3.5, kemudian Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\18.PNG)

   - Klik Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\19.PNG)

   - Lakukan atau klik Install sehingga proses instalasi DNS dan Net Framework 3.5 bisa dijalankan.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\20.PNG)

5. **Promote Server to a Domain Controller**

   - Pada step ini, diawali dengan melakukan konfigurasi ADDS.

     - Setting IP Address Server-ADDS menggunakan IP Static.

     - Proses ini dilakukan di Command Prompt dengan mengetikkan sconfig. Jika menu sudah muncul, maka selanjutnya ketik angka 8 untuk masuk ke menu Network Setting.

       ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\22.PNG)

     - Setlanjutnya ketik 1 untuk mengatur IP Address.

       ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\23.PNG)

     - Ketik 1 lagi untuk Set network adapter address.

       ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\24.PNG)

     - Isikan IP address, netmask, serta default gateway.

       ```markdown
       192.168.1.7 untuk IP address
       255.255.255.0 untuk netmask
       192.168.1.1 untuk default gateway
       ```

       

       ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\25.PNG)

     - Jika telah berhasil, maka IP akan berganti dari yang semula DHCP, menjadi Static.

       ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\39.PNG)

   - Selanjutnya kembali ke Server Manager dan pilih Promote this server to a domain controller untuk melakukan konfigurasi ADDS.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\27.PNG)

   - Pilih "Add a new forest" dan masukkan nama domain yang akan digunakan pada Root Domain Name. Di sini menggunakan "ainin.com".

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\28.PNG)

   - Selanjutnya centang pilihan DNS Server dan Global Catalog, lalu masukkan password dan klik Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\29.PNG)

   - Klik Next untuk melanjtkan proses.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\30.PNG)

   - Pada step ini, The NetBIOS domain name biasanya akan terisi secara otomatis. Jika sudah terisi, maka klik Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\31.PNG)

   - Pada menu Paths, klik Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\32.PNG)

   - Saat masuk ke menu Review Options, cek konfigurasi apakah sudah sesuai sebelum memilih Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\33.PNG)

   - mmm

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\33.PNG)

   - Klik Install dan tunggu hingga prosesnya selesai.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\34.png)

   - Proses instalasi pada step ini akan sedikit memakan waktu dikarenakan VM akan melakukan booting atau restart secara otomatis.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\35.PNG)

   - Setelah proses selesai, maka VM akan mengarahkan proses login pada user AININ\Administrator. Masukkan password yang telah disetting sebelumnya.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\36.PNG)

   - Langkah berikutnya adalah melakukan melakukan cek konfigurasi di Command Prompt.

     ```markdown
     netdom query fsmo 
     ipconfig
     ```

     

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\37.PNG)

   - Pada pengaturan Internet Protokol Version 4, akan terlihat konfigurasi seperti ini.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\40.png)

   - Konfigurasi selesai.

     
