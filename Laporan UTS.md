## **LAPORAN PRAKTIKUM UJIAN TENGAH SEMESTER**

1. **Instalasi Windows Server 2022**

   - Download terlebih dahulu ISO Windows Server 2022.

     ```markdown
     https://software-download.microsoft.com/download/sg/20348.169.210806-2348.fe_release_svc_refresh_SERVER_EVAL_x64FRE_en-us.iso
     ```

   - Buat file baru sebelum melakukan instalasi. Typer yang digunakan ialah Microsoft Windows dengan version Other Wishdows (64-bit), kemudian klik Next.

     ![1](https://user-images.githubusercontent.com/92904284/143678219-fe59f3bd-a4a2-4dcd-ac7a-fece38d38b43.PNG)

   - Isi RAM untuk virtual machine sesuai kebutuhan. Di sini menggunakan 2048 mb.

     ![2](https://user-images.githubusercontent.com/92904284/143679183-7bfefe71-ec86-4f1a-8518-4d39c0832bef.PNG)

   - Lakukan create virtual machine, pilih Create a virtual harddisk now.

     ![3](https://user-images.githubusercontent.com/92904284/143679329-70c53705-3e8a-40e0-bdc2-d8ec170a0d20.PNG)

   - Pilih VDI (VirtualBox Disk Image), kemudian Next.

     ![4](https://user-images.githubusercontent.com/92904284/143679338-809c7f95-192a-4c3e-bf87-1342a07570f7.PNG)

   - Pilih Dynamically allocated.

     ![5](https://user-images.githubusercontent.com/92904284/143679340-4e19599e-3743-4fb8-9d9e-1c8c3f65b06b.PNG)

   - Langkah selanjutnya yaitu mengisi besaran memori untuk VM sesuai keinginan. Rekomendasi ukuran yang digunakan adalah 20 GB, tetapi di sini menggunakan 40 GB. Setelah itu klik Create.

     ![6](https://user-images.githubusercontent.com/92904284/143679341-ead6cc99-ed21-4c70-8410-f633a66a1a67.PNG)

   - Jika file telah berhasil dibuat, maka selanjutnya klik Start untuk memulai instalasi. Masukkan file ISO terlebih dahulu, agar instalasi dapat berjalan. Jika sudah, maka klik Start.

     ![7](https://user-images.githubusercontent.com/92904284/143679342-087c10db-41c4-4e1c-834a-0847f54800b0.PNG)

   - Tampilan berikutnya akan terlihat seperti ini.

     ![8](https://user-images.githubusercontent.com/92904284/143679384-eebe231f-bc7c-47a6-8f35-2c2d91dba557.PNG)

   - Pilih pengaturan bahasa yang digunakan, lalu klik Next.

     ![rev 1](https://user-images.githubusercontent.com/92904284/143679376-87399ff2-de57-4e36-907b-e81ebe6d11ec.PNG)

   - Selanjutnya, pilih Install now.

     ![10](https://user-images.githubusercontent.com/92904284/143679386-2630aa39-acb1-4601-8db0-5a048c6b7f5b.PNG)

   - Pada langkah ini, pilih menu kedua atau Windows Server 2022 Standard Evaluation (Dekstop Experience) jika ingin menginstal versi GUI.

     ![rev 2](https://user-images.githubusercontent.com/92904284/143679377-27c2904a-44ca-4bd2-adba-afe602f74774.PNG)

   - Cetang atau setujui lisensi yang ada, lalu klik Next.

     ![12](https://user-images.githubusercontent.com/92904284/143679391-8d772930-24db-47ac-9990-41f91df82862.PNG)

   - Pilih custom.

     ![13](https://user-images.githubusercontent.com/92904284/143679392-63e05bbb-191b-426b-8ede-9759a835893a.PNG)

   - Next untuk menetapkan ukuran memori yang digunakan.

     ![14](https://user-images.githubusercontent.com/92904284/143679395-04f522f2-10ef-4fd2-be46-15719ef0a0eb.PNG)

   - Tunggu hingga proses selesai

     ![rev 3](https://user-images.githubusercontent.com/92904284/143679378-28d7e604-d910-4bb9-93ed-ccb5f11e0006.PNG)

   - Setelah proses selesai, akan muncul tampilan untuk mengisi password yang akan digunakan untuk melakukan login.

     ![rev 4 isi passwd](https://user-images.githubusercontent.com/92904284/143679379-7d3ab121-f8a0-4c83-aa2b-d99e0fd9e472.PNG)

   - Berikut ini adalah tampilan awal sebelum login. Klik menu Input pada VirtualBox, pilih Keyboard, lalu klik pilihan Ctrl+Alt+Del, untuk melakukan unlock.

     ![rev 5 done](https://user-images.githubusercontent.com/92904284/143679380-184bbd3d-ef9a-4673-b39e-b2608537dc85.PNG)

   - Masukkan password yang telah disetting sebelumnya sebagai proses verifikasi.

     ![rev 6](https://user-images.githubusercontent.com/92904284/143679381-0c3c5d02-3bb3-4e7e-86e2-0014f0453145.PNG)

   - Jika berhasil, maka akan masuk ke halaman utama. Proses instalasi telah selesai.

     ![rev 7](https://user-images.githubusercontent.com/92904284/143679383-d8c3dfc2-b4eb-4ba1-8af7-fc15db02653a.PNG)

   

2. **Instalasi Active Directory Domain Services**

   - Langkah awal yaitu install VBoxWindows Additions.

     ![1](https://user-images.githubusercontent.com/92904284/143679696-776a5ca0-4cf7-4df2-9191-a9dd1b805fdb.png)

   - Klik Next hingga tida di halaman instalasi dan klik Install. Jika sudah selesai, pilih Finish.

     ![6](https://user-images.githubusercontent.com/92904284/143679703-84a0421b-0e68-4b32-a8ae-adb80006ef35.PNG)

   - Setelah itu, run Winver untuk memvalidasi installed edition dari Windows Server.

     ![7](https://user-images.githubusercontent.com/92904284/143679704-5ecea86c-a6ec-4dff-8a99-165063c3d396.PNG)

   - Ubah terlebih dahulu nama computer melalui windows powrshell.

     ```markdown
     rename-computer -Newname Server2022
     ```

     ![8](https://user-images.githubusercontent.com/92904284/143679705-aeda695a-50e5-43af-a37a-5c055a708f98.PNG)

   - Masuk ke Server Manager, klik Add roles and fatures, kemudian pilih Next.

     ![](E:\ÉLITE FOLDER\Tugas\COLLEGE\TINGKAT 3\SISTEM ADMINISTRASI SERVER\windows server\2B-E\9.PNG)

   - Pilih Role-based or feature based installation untuk melanjutkan.

     ![10](https://user-images.githubusercontent.com/92904284/143679709-b8ab9c70-7cad-40ee-a6e4-36f71ea976d2.PNG)

   - Pilih Select a server from the server pool, kemudian klik Next.

     ![11](https://user-images.githubusercontent.com/92904284/143679814-05216533-5a56-4c45-bab3-55bb9334ab8c.PNG)

   - Pada menu Server Roles, klik pilihan Active Directory Domain Services, lalu akan muncul pop-up dan pilih Add Features kemudian Next.

     ![12](https://user-images.githubusercontent.com/92904284/143679816-0b777ea6-294e-460d-b910-37f1ba317891.PNG)

   - Centang atau pilih Group Policy Management.

     ![13](https://user-images.githubusercontent.com/92904284/143679819-ca74a9ad-bdd9-4c20-a662-e9363b2076fb.PNG)

   - Next pada menu AD DS.

     ![14](https://user-images.githubusercontent.com/92904284/143679820-5d9a6bf1-d3a6-44cb-bc43-09925011dc70.PNG)

   - Pada menu Confirmation, klik Install dan tunggu hingga proses instalasi selesai. Jika sudah selesai, pilih Close sehingga bisa melanjutkan ke proses berikutnya.

     ![15](https://user-images.githubusercontent.com/92904284/143679821-3a982808-35e0-4d20-aea9-3997d721e3db.PNG)

3. **Instalasi DNS Server**

   - Langkah pertama, masuk ke Server Manager, dan pilih Add Roles and Features. Klik Next seperti langkah instalasi Active Directory Domain Services sebelumnya. Pada menu Server Roles, pilih DNS Server, kemudian Add Features.

     ![17](https://user-images.githubusercontent.com/92904284/143679824-37cfcd69-d381-4b82-b3b5-7ca9b1b357b2.PNG)

4. **Instalasi Net Framework 3.5**

   - Berikutnya, pada menu Features, pilih atau centang .Net Framework 3.5 Features, untuk menginstal Net Framework 3.5, kemudian Next.

     ![18](https://user-images.githubusercontent.com/92904284/143679825-6eb2532c-c16a-41f6-8974-2759e978d99a.PNG)

   - Klik Next.

     ![19](https://user-images.githubusercontent.com/92904284/143679826-0d4ee19e-d528-45b4-96ce-20665da2df72.PNG)

   - Lakukan atau klik Install sehingga proses instalasi DNS dan Net Framework 3.5 bisa dijalankan.

     ![20](https://user-images.githubusercontent.com/92904284/143679828-4c305900-6150-4433-bca9-ca3664f18ece.PNG)

5. **Promote Server to a Domain Controller**

   - Pada step ini, diawali dengan melakukan konfigurasi ADDS.

     - Setting IP Address Server-ADDS menggunakan IP Static.

     - Proses ini dilakukan di Command Prompt dengan mengetikkan sconfig. Jika menu sudah muncul, maka selanjutnya ketik angka 8 untuk masuk ke menu Network Setting.

       ![22](https://user-images.githubusercontent.com/92904284/143679981-f038e178-ed22-4f11-8f92-6796462b200d.PNG)

     - Setlanjutnya ketik 1 untuk mengatur IP Address.

       ![23](https://user-images.githubusercontent.com/92904284/143679982-af24b380-1fa0-4c76-8fc6-bde204d09640.PNG)

     - Ketik 1 lagi untuk Set network adapter address.

       ![24](https://user-images.githubusercontent.com/92904284/143679983-9a13f9d9-0097-49d3-989b-c309390a50f4.PNG)

     - Isikan IP address, netmask, serta default gateway.

       ```markdown
       192.168.1.7 untuk IP address
       255.255.255.0 untuk netmask
       192.168.1.1 untuk default gateway
       ```

       

       ![25](https://user-images.githubusercontent.com/92904284/143679984-bba104c8-311f-4cab-89e5-3a4ad7d236d4.PNG)

     - Jika telah berhasil, maka IP akan berganti dari yang semula DHCP, menjadi Static.

       ![39](https://user-images.githubusercontent.com/92904284/143680037-ab1a4ae1-46d6-41a0-9c06-ac5195f99c63.PNG)

   - Selanjutnya kembali ke Server Manager dan pilih Promote this server to a domain controller untuk melakukan konfigurasi ADDS.

     ![27](https://user-images.githubusercontent.com/92904284/143679987-2c10ef4d-424e-44b0-a816-e6d0398ca445.PNG)

   - Pilih "Add a new forest" dan masukkan nama domain yang akan digunakan pada Root Domain Name. Di sini menggunakan "ainin.com".

     ![28](https://user-images.githubusercontent.com/92904284/143679988-f0bdd441-d261-4606-b4d7-d5f35277c15f.PNG)

   - Selanjutnya centang pilihan DNS Server dan Global Catalog, lalu masukkan password dan klik Next.

     ![29](https://user-images.githubusercontent.com/92904284/143679990-9183ea13-0cec-4fb3-86ca-c523ae9525fe.PNG)

   - Klik Next untuk melanjtkan proses.

     ![30](https://user-images.githubusercontent.com/92904284/143679992-9ec425fe-13c2-4ec2-81a1-3fd6ffa213d3.PNG)

   - Pada step ini, The NetBIOS domain name biasanya akan terisi secara otomatis. Jika sudah terisi, maka klik Next.

     ![31](https://user-images.githubusercontent.com/92904284/143680068-5789b5a9-4979-428f-89aa-46a8c6e05ba4.PNG)

   - Pada menu Paths, klik Next.

     ![32](https://user-images.githubusercontent.com/92904284/143680069-485bbe95-2412-451a-aa80-44128ad08be0.PNG)

   - Saat masuk ke menu Review Options, cek konfigurasi apakah sudah sesuai sebelum memilih Next.

     ![33](https://user-images.githubusercontent.com/92904284/143680070-7d215cca-902e-487c-b6d6-6f207631a35d.PNG)

   - Klik Install dan tunggu hingga prosesnya selesai.

     ![34](https://user-images.githubusercontent.com/92904284/143680072-ef3542de-07ef-4396-9f11-b9d1bc97acac.png)

   - Proses instalasi pada step ini akan sedikit memakan waktu dikarenakan VM akan melakukan booting atau restart secara otomatis.

     ![35](https://user-images.githubusercontent.com/92904284/143680073-491c8ae7-6c1f-4ff2-9370-1977dc3bcfae.PNG)

   - Setelah proses selesai, maka VM akan mengarahkan proses login pada user AININ\Administrator. Masukkan password yang telah disetting sebelumnya.

     ![36](https://user-images.githubusercontent.com/92904284/143680075-a4bfa848-522d-4d1d-8e9d-fa72a0a8c737.PNG)

   - Langkah berikutnya adalah melakukan melakukan cek konfigurasi di Command Prompt.

     ```markdown
     netdom query fsmo 
     ipconfig
     ```

     

     ![37](https://user-images.githubusercontent.com/92904284/143680076-978dcef5-15eb-4267-8981-3b7a68f8c13c.PNG)

   - Pada pengaturan Internet Protokol Version 4, akan terlihat konfigurasi seperti ini.

     ![40](https://user-images.githubusercontent.com/92904284/143680081-6e35d0de-7e10-423f-9f7b-dfbdd8e8394f.png)

   - Konfigurasi selesai.

     
