# LearnGit
Used for beginners to learn git

 Thư muc làm việc--------Staging Area-----------Commited
0 HelloWorld.txt---------------------------------------- branch: *Main
1-----------------------HelloWorld.txt------------------
2-------------------------------------------HelloWorld.txt                     
3 HelloWorld1.txt---------------------------------------
4-----------------------HelloWorld1.txt-----------------
5 HelloWorld1.txt---------------------------------------
6------------------------------------------------------- branch: newbranch
7-----------------------HelloWorld1.txt-----------------
8-------------------------------------------Helloworld.txt
9


Terminal:
#1 /git add HelloWorld.txt  //Lệnh này từ mục làm việc chuyển sang Staging Area
#2 /git commit -m "Add file HelloWorld" //Lệnh này đưa qua commnited với tiêu đề file 
#3 /git status 
//Kiểm tra Thư mục làm việc nếu có file HelloWorld.txt 
Thì sẽ thông báo:
Changes not staged for commit:
.Modified: HelloWorld.txt (textColor=Red)
//Kiểm tra Statging nếu có file HelloWorld.txt
Changes to be Commnited:
.Modified: HelloWorld.txt (textColor=Green)
#4 /git add HelloWorld1.txt
#5 /git restore --staged HelloWorld.txt //Lệnh này từ mục Staging Are chuyển về thư mục làm việc

#6 /git checkout -b newbranch 
#7 /git add HelloWorld1.txt
#8 /git commnit -m "Add HellWorld1.txt"

show:*main,newbranch

*Main:
Add file Helloworld.txt

newbranch:
Add file Helloworld.txt
Add file Hellowrold1.txt

#9 /git checkout main //Quay về branch *Main
*Main:
Add file Helloworld.txt

#10 /git merge newbranch
*Main:
Add file Helloworld.txt
Add file Hellowrold1.txt


@1 /git log //Xem lại history commnit
@2 /git branch //Hiển thị thông tin các nhánh
