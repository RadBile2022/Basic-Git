# Script git dasar
1. git config --global user.name "usernamekamu" => untuk konfigurasi/login username git
2. git config --global user.email "emailkamu" => untuk konfigurasi/login email git
3. git config --global --unset user.name => untuk menghapus user name konfigurasi git
4. git config --global --unset user.name => untuk menghapus email konfigurasi git
5. git config --global --unset-all => menghapus seluruh konfigurasi
6. git config --list --show-origin => melihat seluruh configurasi

7. git init => untuk initialisasi folder/membuat repo local
8. git status => untuk melihat status git

* diagram three tree / workflow git :
  * repository => jika telah ter commit
  * staging index => jika telah ter add
  * working => jika sebelum di add
  
9. git add . => memindahkan seluruh file di working area ke stagging index (jika 1 file saja ganti . dengan nama filenya)
10. git commit -m "pesan commit" => memindahkan seluruh file di stagging ke repository
11. git diff => melihat perubahan file nya
12. git restore --staged namafile => memindahkan file dari staging area ke working 
13. git restore namafile => membatalkan perubahan di working area, jika file sudah di stagging area wajib di pindahkan ke working area baru bisa
14. git log => melihat history commit
15. alias graph="git log --all --oneline --decorate --graph" => melihat history commit dengan graphic network
16. git branch => melihat semua branch
17. git branch --show-current => melihat branch saat ini
18. git checkout namabranch => pindah branch
19. git checkout hash7nomer => pindah ke suatu commit dengan 7nomer hash

* .ignore
  * untuk file yang tidak akan ter track di git
  * bisa kunjungin web ignore.io untuk melihat file yang di recommended tidak di track

20. git branch -m namabranchbaru => mengubah nama branch (harus di posisi branch yang ingin di rename)
21. git branch -d namabranch => menghapus branch (jangan di posisi branch yang ingin di hapus)
22. git merge namabranch => menggabungkan branch 
    * ada 2 jenis merge
      * fast forward => harus berada dalam jalur langsung / direct path
      * three-way merge / merge commit => membuat commit baru ketika di merge karena tidak dalam jalur langsung
23. git rebase namabrach => rebase merge, merge dengan cara yang rapih
24. git merge --squash namabranch => menggabungkan beberapa commit menjadi 1 commit

* git remote
  * git remote add origin urlnya => menambah remote repository
  * git remote => untuk melihat remote repository
  * git remote -v => untuk melihat detail remote repo
  * git remote rm namaremote => menghapus remote repo

25. git push Nremote Nbranch => mengirim perubahan dari local(git) ke server(github)
26. git push Nremote --delete Nbranch => menghapus branch yang ada di remote repo
27. git clone urlremoterepo => mendownload project di remote repo ke local, dan secara otomatis menjadi git project dan terhubung remote repo origin dari yang kita clone
28. git branch -a => melihat branch di local dan remote
29. git fetch => untuk mendapatkan perubahan terakhir dari remote repo
30. git pull => mengambil perubahan di remote repo dan di simpan di local, dengan pull kita melakukan fetch secara otomatis terlebih dahulu
31. pull request => meminta request merge ke branch yang dituju di remote repo
32. merge conflict => kondisi dimana kedua branch yang ingin di merge, ada kesamaan baris yang di ubah/berbeda, maka kita wajib memilih baris mana yang akan di gunakan
33. fork => melakukan duplikasi ke tempat kita, biasanya digunakan ketika ingin berkontribusi kepada project open source, dimana kita tidak punya akses langsung ke git repo nya, Semua perubahan nanti dilakukan di git repository profile kita Dan setelah selesai, kita bisa melakukan pull request ke repository sumber forking kita
34. code . => membuka ide code 
edit radar
