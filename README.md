# xcodesmbhack

X-code SMB Hack v0.3 for Kali Linux
-----------------------------------

Update : 09 Mei 2020

Program untuk membantu hacking SMB Windows 7, 8.1 dan Server 2012 serta DoS Windows 7, 8 dan 10.

Program ini sebagai core hacknya menggunakan exploit dari https://github.com/worawit/MS17-010 yang memanfaatkan celah bug dari MS17-10. 

Bagaimana cara kerja X-code SMB Hack?
------------------------------

X-code SMB Hack akan membuat share program netcat windows secara otomatis pada kali linux anda, dengan melalui share folder, ketika exploit dari worawit ini dijalankan dan berhasil masuk ke komputer target maka exploit ini akan menghubungi komputer anda untuk mengambil program netcat dari komputer anda.

Exploit dari hasil modifikasi selain akan menghubungi komputer anda juga akan menutup share ke komputer anda secara otomatis setelah file nc.exe disalin ke komputer target. Setelah itu di komputer target, exploit dari hasil modifikasi tersebut akan menghubungi komputer anda kembali dengan menggunakan netcat agar komputer anda sebagai penyerang atau pentester dapat terhubung dengan komputer target melalui akses command prompt.

Daftar file
-----------
File hackwindows.sh dibuat oleh Kurniawan. trainingxcode@gmail.com. xcode.or.id. Licensi : GNU General Public License

File dos1.py berasal dari https://github.com/worawit/MS17-010 yang disesuaikan isinya agar bisa untuk denial of service windows 7/8.1/10 

File hack1.py berasal dari https://github.com/worawit/MS17-010 yang diedit agar mendukung X-code SMB Hack sekaligus bisa untuk hacking remote pada target Windows 7 dan 8.1

File hack2.py berasal dari https://github.com/worawit/MS17-010 yang diedit agar mendukung X-code SMB Hack sekaligus bisa untuk hacking remote pada target Windows Server 2012

File nc.exe berasal dari https://eternallybored.org/misc/netcat

Program X-code SMB Hack ini memodifikasi exploit-exploit dari worawit sehingga bisa dipakai untuk hacking secara praktis dan jauh lebih mudah dengan memanfaatkan fitur X-code SMB Hack.

Jika Windows tidak bisa dihack maka bisa banyak penyebab dari karena sudah dipatch, share yang dipassword dan sebagainya.

Cara penggunaan :
-----------------

git clone https://github.com/kurniawandata/xcodesmbhack.git

cd xcodesmbhack

chmod -R 777 *

./hackwindows.sh

Jika ingin mengedit exploit dari hackwindows.sh, tekan ctrl+w lalu ketik 192.168.1.223 lalu enter, ganti semua ipnya dengan ip linux kamu atau ip pentester.
