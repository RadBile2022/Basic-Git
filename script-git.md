# Script git dasar
1. git config --global user.name "usernamekamu" => untuk konfigurasi/login username git
2. git config --global user.email "emailkamu" => untuk konfigurasi/login email git
3. git config --list --show-origin => melihat seluruh configurasi

4. git init => untuk initialisasi folder/membuat repo local
5. git status => untuk melihat status git

* diagram three tree / workflow git :
  * repository => jika telah ter commit
  * staging index => jika telah ter add
  * working => jika sebelum di add
  
6. git add . => memindahkan seluruh file di working area ke stagging index (jika 1 file saja ganti . dengan nama filenya)
7. git commit -m "pesan commit" => memindahkan seluruh file di stagging ke repository
8. git diff => melihat perubahan file nya
