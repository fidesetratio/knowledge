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
