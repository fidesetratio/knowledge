# Git

Tips and Trick

Flow normal Git

* Hal yang pertama yang harus di cek

	```bash
	git config --global user.name "Patar timotius"
	git config --global user.email  "patartimotiustambunan@gmail.com"
	git config --list // ini untuk melihat semua listnya
	
	```

* Starting
	
	* Git init ==> Membuat folder baru

	
	 ```bash
 	 	mkdir source  // buat folder baru
		cd source // cd source
		git init // buat folder ini ini jadi git internal repository
         ```
 	
	 Jangan lupa buat repository di gitlab atau github 
	
	```bash
		git remote add origin https://github.com/fidesetratio/multigit.git
		git push -u origin master
	
	```




 
	* Git clone ==> Ambil dari git clone baru seperti gitlab atau github
	```bash
		git clone https://github.com/fidesetratio/knowledge.git
		cd knowledge // cd knowledge
		git status // cek statusnya
	```


* Flow day to day

	Ini merupakan flow day to daily

	```bash
		git add -A // menambahkan folder/ file to stage
		git log // cek log dengan 
		git status // bisa lihat hash commit dan juga history log
		git reflog // bisa checkout seperti log juga
	```
	Tambahan untuk melihat data repository

	```bash
		git branch // lihat branch local
		git branch -a // lihat branch local & remote
		git remote -v  // lihat remote url
	
	
	```
	
	Merge branch to master
	ex: master,test
	
	```bash
	git checkout master
	git reset --hard test
	git push --force origin master
	```
	
	
	
	Contoh day to day:
	
	1. git clone https://github.com/fidesetratio/multigit.git
	2. git status // pastikan berada di master
	3. buat source code seperti yang diinginkan
	    contoh : touch helloworld.sh
		     vim helloworld.sh
		     echo "helloworld
	4. git add -A // jangan lupa untuk kirim stage
	5. git commit -m "Hello world dengan bash"
	6. git pull origin master // ini pastikan pull latest source code aga
	7. git push origin master // push ke remote

	Note : diatas commit di master (ini bukan yang hal baik dalam software development)
	
	Day to day menggunakan branch
	1. Lihat 1-2 dari yang diatas
	2. git branch //lihat branch
	3. git branch tambahkandelete // buat branch tambahkan delete
	4. git checkout tambahkandelete // checkout branch tambahkan delete
	5. modify data dan tambahkan data tersebut 
	6. git add -A
	7. git commit -m "Tambahkan delete"
	8. git push -u origin tambahkandelete  
	9. Biasanya kompany ada test control
	10. setelah benar
	11. git checkout master
	12. git merge tambahkandelete
	13. Setelah selesai mohon delete branch nya
	14. git branch -d tambahkandelete // ini di local
	15. git branch -a // di remote masih ada
	16. git push origin --delete tambahkandelete // remote harus delete juga	
	
