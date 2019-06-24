		# golang_env-setup





		=>1 telecharger golang sur golang.org
		=>2 decompresser le ficher
une fois telechargement terminer aller ddans download et taper la commande suivante pour decompresser le
fichier dans /usr/local/ 

	$ sudo tar -xzvf go1.6.2.linux... -c /usr/local/

		=>3 configurer votre environnement

	$ mkdir go
	$ cd go
	$ mkdir src bin pkg
		
		=>4 ajouter go a votre path
	
	$ vim ~/.profile
puis ajouter juste en bas les code suivante

	==1 export GOPATH=/home/username/golang
	==2 export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin

enregstrer puis sorter
et maintenant vous pouvez taper $ go env pour voir vos midification

		=>5 creeons un projet hello world
taper les commande suivante

	$ cd $GOPATH/src
	$ mkdir -p github.com/gitubUsername/projectName

en suite deplacer vous dans le dossier en question puis taper la commande suivante
	$nano hello.go
dans laquelle vous aller copier et coller le code suivante

	============================================
		package main

		import "fmt"

		func main(){
			fmt.Println("hello world')
		}
	==============================================
maintenant taper en commande 
	
	$ go install
	$ cd $GOPATH/bin

dans lequelle vous trouverez l'executable de votre projet 
maintenant ou que vous vous trouvez vous pouvez tapez 
	
	$ hello

et votre programme fonctionne 






								Merci




