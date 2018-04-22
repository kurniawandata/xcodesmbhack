# xcodesmbhack
Program untuk membantu hacking SMB Windows 7, 8.1, 10, Server 2012, Server 2016 (Bypass Firewall &amp; bypass Windows Defender).

Program ini dibuat berdasarkan exploit dari https://github.com/worawit/MS17-010 yang memanfaatkan celah bug dari MS17-10. 

Daftar file
-----------
File hackwindows.sh dibuat oleh Kurniawan dengan licensi : GNU General Public License

File dos1.py berasal dari https://github.com/worawit/MS17-010 yang disesuaikan isinya agar bisa untuk denial of service windows 7/8.1/10 

File dos2.py berasal dari  https://github.com/worawit/MS17-010 yang disesuikan isinya agar bisa untuk denial of service Windows Server 2012 dan Server 2016

File hack1.py berasal dari https://github.com/worawit/MS17-010 yang diedit agar mendukung X-code SMB Hack sekaligus bisa untuk hacking remote pada target Windows 7, 8.1 dan 10

File hack2.py berasal dari https://github.com/worawit/MS17-010 yang diedit agar mendukung X-code SMB Hack sekaligus bisa untuk hacking remote pada target Windows Server 2012, 2016

File nc.exe berasal dari https://eternallybored.org/misc/netcat

Program X-code SMB Hack ini memodifikasi exploit-exploit dari worawit sehingga bisa dipakai untuk hacking secara praktis dan jauh lebih mudah dengan memanfaatkan fitur X-code SMB Hack.

Jika Windows tidak bisa dihack maka bisa banyak penyebab dari karena sudah dipatch, share yang dipassword dan sebagainya.

Cara penggunaan :
-----------------

git clone https://github.com/kurniawandata/xcodesmbhack.git

cd xcodesmbhack

chmod 777 *

./hackwindows.sh

Jika ingin mengedit exploit dari hackwindows.sh, tekan ctrl+w lalu ketik 192.168.1.223, ganti ipnya dengan ip linux kamu atau ip pentester.

Program X-code SMB Hack ini dibuat oleh Kurniawan. trainingxcode@gmail.com. xcode.or.id
