# golang_env-setup 





## 1 telecharger golang sur golang.org
## 2 decompresser le ficher
une fois telechargement terminer aller dans download et taper la commande suivante pour decompresser le
fichier dans /usr/local/ 
```shell
	$ sudo tar -xzvf go1.6.2.linux... -c /usr/local/
```
## 3 configurer votre environnement
```shell
	$ mkdir go
	$ cd go
	$ mkdir src bin pkg
```	
## 4 ajouter go a votre path
```shell
	$ vim ~/.profile
```
puis ajouter juste en bas les code suivante

```shell
	$ export GOPATH=/home/username/golang
	$ export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin
```
enregstrer puis sorter
et maintenant vous pouvez taper ```shell $ go env ``` pour voir vos midification

## 5 creeons un projet hello world
taper les commande suivante
```shell
	$ cd $GOPATH/src
	$ mkdir -p github.com/gitubUsername/projectName
```
en suite deplacer vous dans le dossier en question puis taper la commande suivante
```shell
	$nano hello.go
```
dans laquelle vous aller copier et coller le code suivante

	============================================
```go
		package main

		import "fmt"

		func main(){
			fmt.Println("hello world')
		}
```
	==============================================
maintenant taper en commande
```shell
	$ go install
	$ cd $GOPATH/bin
```
dans lequelle vous trouverez l'executable de votre projet
maintenant ou que vous vous trouvez vous pouvez tapez
```shell
	$ hello
```
*et votre programme fonctionne :+1:*





## thanks




